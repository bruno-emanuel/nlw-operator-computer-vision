Explicação do Projeto

O projeto Rockit Vision consiste em um sistema de reconhecimento de gestos das mãos em tempo real, utilizando inteligência artificial integrada a tecnologias de visão computacional. A aplicação captura imagens por meio da webcam, processa esses dados no backend e retorna ao usuário a identificação dos gestos detectados.

Inicialmente, a compreensão do funcionamento do sistema pode ser complexa, pois envolve a integração de múltiplas ferramentas e conceitos. No entanto, ao analisar seu funcionamento por etapas, torna-se mais claro.

Funcionamento do Sistema

O sistema opera em diferentes etapas:

Captura de imagem
O navegador acessa a webcam do usuário e captura os frames de vídeo em tempo real.

Transmissão dos dados
Esses frames são enviados ao servidor por meio de WebSockets, permitindo uma comunicação contínua e de baixa latência.

Processamento com visão computacional
No backend, o MediaPipe é responsável por detectar a mão e identificar pontos específicos (landmarks).

Classificação do gesto
Os pontos identificados são utilizados como entrada para um modelo de machine learning, desenvolvido com scikit-learn, que classifica o gesto realizado.

Retorno dos resultados
O sistema envia de volta ao navegador o frame processado, juntamente com a identificação do gesto.

Exibição ao usuário
O frontend exibe os resultados em tempo real, permitindo a visualização dinâmica do reconhecimento.

Como Utilizar o Sistema

Para executar o projeto, é necessário seguir os seguintes passos:

Acessar a pasta do projeto:

cd computer_vision_app

Instalar as dependências:

uv sync

Baixar o modelo do MediaPipe e colocá-lo no diretório:

computer_vision_app/models/

Executar a aplicação:

uv run app.py

Acessar o sistema pelo navegador:

http://localhost:5001

Permitir o uso da webcam quando solicitado.

Dificuldades Encontradas

Durante o desenvolvimento e compreensão do projeto, alguns pontos se mostraram mais complexos, como o funcionamento dos WebSockets, a interpretação dos dados gerados pelo MediaPipe e a integração desses dados com o modelo de classificação.

Considerações Finais

O projeto demonstra de forma prática a aplicação de inteligência artificial em tempo real, integrando diferentes tecnologias para resolver um problema específico. Além disso, evidencia a importância da compreensão dos dados e da integração entre frontend e backend para o desenvolvimento de sistemas interativos.