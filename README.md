# Projeto Sensorless Drive Diagnosis

##### Leonardo Martelli Oliveira, Marcello Fabrizio

# Introdução

Automóveis são uma parte crucial do mundo moderno, sendo utilizados para transporte pessoal, público, de mercadorias 
e em demais necessidades da sociedade. Com tamanha importância, um nível de segurança é exigido, garantindo o bom 
funcionamento de veículos. Com a tecnologia disponível hoje, é possível arquitetar soluções que ajudam na confiabilidade dos 
carros, como por exemplo a detecção prévia de problemas no sistema de transmissão elétrico dos mesmos. A detecção é 
tarefa que pode ser feita por monitoramento e coleta de sinais elétricos em componentes do sistema foco. Após pode se realizar 
análises e classificações de tais amostras para previsão de possíveis erros.

Este trabalho realiza a análise de classificadores paramétricos e
não-paramétricos aplicados sobre um conjunto de dados composto por
amostras de sinais elétricos de sistemas de transmissão veiculares, e
comparando com resultados obtidos por trabalhos anteriores, consultados
na literatura.

# Base de Dados

O objetivo do projeto abordado no artigo de origem é a utilização de um método para redução de complexidade para implementação 
de sistemas de controle e monitoramento do sistema de transmissão elétrica de veículos, que consiste em uma instalação composta
de várias componentes e umaparte crucial da máquina. Os autores não utilizam sensores para o monitoramento de tal sistema, eles 
abordam o uso das fases da corrente alternada do motor para isso[1].

A base de dados **Sensorless Drive Diagnosis** foi retirada do repositório online de aprendizado de máquina da **University of
California, Irvine**[2]. A base de dados origina do artigo **Sensorless Drive Diagnosis Using Automated Feature Extraction,
Signiﬁcance Ranking and Reduction**[1].

O conjunto de dados utilizado no projeto possui 58508 amostras e é
composto por 48 variáveis sendo dos sinais do sistema de transmissão, classificadas em um conjunto de 11 classes 
distintas, sendo estes os possíveis estados do sistema - 1 para sem defeitos e os 10 remanescentes, 10 defeitos 
distintos. O conjunto original não  contém dados de cabeçalho. Todas variáveis são numéricas de ponto flutuante.

Para o desenvolvimento do projeto, as colunas referentes às variáveis independentes, foram nomeadas da seguinte maneira
: **Feature*X***, sendo _X_ um número de 1 a 48; a coluna contendo as classes foi representada como **label**.

As classes no _dataset_ apresenta um balanceamento perfeito com 5319 amostras para cada classe.

# Bibliografia
[1] Christian Bayer, Olaf Enge-Rosenblatt, Martyna Bator, and Uwe Monks, “Sensorless drive diagnosis using automated 
feature extraction, significance ranking and reduction,” 2013 IEEE 18th Conference on Emerging Technologies Factory Automation (ETFA), 2013.

[2] Dheeru Dua and Casey Graff, “UCI machine learning repository,” 2017.