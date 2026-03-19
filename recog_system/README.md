Sistema de Reconhecimento e Laboratório de Visão Computacional

Este projeto consiste em um sistema completo para reconhecimento de gestos em tempo real, utilizando técnicas de visão computacional e machine learning. Além disso, o repositório também inclui notebooks exploratórios voltados para diferentes aplicações na área, como classificação, detecção e segmentação de imagens.

Sobre o Projeto

O principal objetivo do projeto é implementar um pipeline completo, desde a coleta de dados até a inferência em tempo real. Diferente de soluções baseadas apenas em modelos prontos, este sistema permite a criação de um conjunto de dados próprio, possibilitando ao usuário treinar um modelo personalizado para reconhecer gestos específicos.

Essa abordagem torna o sistema mais flexível e aplicável a diferentes contextos.

Tecnologias Utilizadas

O projeto foi desenvolvido utilizando as seguintes ferramentas:

Python como linguagem principal

OpenCV para captura e processamento de imagens

MediaPipe para extração dos pontos da mão (landmarks)

Scikit-Learn para treinamento do modelo de classificação

Pandas e NumPy para manipulação de dados

uv para gerenciamento de dependências

Funcionamento do Pipeline

O sistema é dividido em três etapas principais:

1. Coleta de Dados

Nesta etapa, é utilizado o script collect_landmarks.py, que permite capturar os pontos da mão em tempo real. Esses dados são armazenados e utilizados posteriormente no treinamento do modelo.

Durante a execução:

A tecla “s” salva um único frame

A tecla “r” inicia ou interrompe a gravação contínua

A tecla “q” encerra o programa

2. Treinamento do Modelo

O script train_model.py processa os dados coletados e treina um modelo de classificação utilizando o algoritmo Random Forest.

Como resultado, são gerados arquivos que armazenam o modelo treinado e os rótulos dos gestos. Além disso, são exibidas métricas de desempenho, como precisão, recall e F1-score, permitindo avaliar a qualidade do modelo.

3. Reconhecimento em Tempo Real

Na etapa final, o script webcam_recog.py utiliza a webcam para capturar imagens em tempo real. O sistema detecta a mão, extrai os pontos e realiza a classificação do gesto com base no modelo previamente treinado.

O resultado é exibido diretamente na tela, permitindo uma interação dinâmica com o sistema.

Notebooks Exploratórios

O projeto também inclui notebooks que exploram outras aplicações de visão computacional:

Classificação de imagens utilizando modelos da biblioteca timm

Detecção de objetos com o modelo YOLO-S

Segmentação de imagens com CLIPSeg

Análise multimodal utilizando a API do Google Gemini

Esses materiais complementam o projeto, ampliando a compreensão sobre diferentes técnicas da área.

Instalação e Execução

Para utilizar o sistema, é necessário:

Acessar a pasta do projeto:

cd recog_system

Instalar as dependências:

uv sync

Baixar os modelos necessários e colocá-los na raiz do projeto

Executar os scripts conforme a etapa desejada (coleta, treinamento ou reconhecimento)

Considerações Finais

Este projeto permite compreender, de forma prática, como funciona um sistema de visão computacional aplicado ao reconhecimento de gestos. Além disso, evidencia a importância da coleta de dados, do treinamento de modelos e da integração entre diferentes tecnologias para construção de soluções baseadas em inteligência artificial.