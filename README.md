<h1 align="center">
🚀 Rockit Vision — Reconhecimento de Gestos com IA
</h1>

<p align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00c6ff,100:0072ff&height=120&section=header"/>
</p>

<p align="center">
Sistema de visão computacional em tempo real utilizando Inteligência Artificial para reconhecimento de gestos.
</p>

---

<p align="center">
<img src="https://img.shields.io/badge/Python-3.11+-blue?style=for-the-badge&logo=python"/>
<img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-green?style=for-the-badge&logo=opencv"/>
<img src="https://img.shields.io/badge/MediaPipe-ML-orange?style=for-the-badge&logo=google"/>
<img src="https://img.shields.io/badge/Scikit--Learn-ML-yellow?style=for-the-badge&logo=scikit-learn"/>
</p>

---

## 💡 Sobre o Projeto

O **Rockit Vision** é um sistema desenvolvido para reconhecer gestos das mãos em tempo real utilizando a webcam.

A ideia principal foi entender na prática como funciona um pipeline completo de visão computacional, desde a captura de dados até a classificação com machine learning.

Esse projeto não usa apenas modelos prontos, ele permite criar seus próprios gestos e treinar o modelo, tornando tudo mais flexível e aplicável.

---

## ⚙️ Como Funciona

O sistema segue um fluxo simples:

1. A câmera captura os frames em tempo real  
2. Os dados são enviados para o backend  
3. O MediaPipe identifica os pontos da mão  
4. O modelo de ML classifica o gesto  
5. O resultado é exibido na tela  

---

## 🛠️ Tecnologias Utilizadas

- Python  
- OpenCV  
- MediaPipe  
- Scikit-Learn  
- NumPy / Pandas  
- WebSockets  

---

## 🚀 Como Executar

```bash
cd computer_vision_app
uv sync
uv run app.py

Acesse:

http://localhost:5001
🧠 O que eu aprendi

No começo, esse projeto foi bem desafiador pra entender, principalmente por envolver várias partes ao mesmo tempo:

Comunicação em tempo real (WebSocket)

Processamento de imagem

Machine Learning

Integração entre frontend e backend

Mas com o tempo tudo foi fazendo sentido.

Hoje consigo entender melhor como a IA funciona na prática, e isso foi muito importante pra minha evolução.

🔥 O que mais achei interessante

Reconhecimento em tempo real

Ver os pontos da mão sendo detectados

Criar meus próprios gestos

Controle de qualidade e FPS

📌 Conclusão

Esse projeto foi uma experiência muito boa, porque saiu da teoria e foi direto pra prática.

Mostra como a inteligência artificial pode ser usada em aplicações reais e como diferentes tecnologias trabalham juntas.

<p align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=0:00c6ff,100:0072ff&height=120&section=footer"/> </p> ```
