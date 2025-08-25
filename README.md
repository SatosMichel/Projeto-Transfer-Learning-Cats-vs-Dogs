# Projeto de Transfer Learning: Gatos vs. Cachorros 🐱🐶

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=for-the-badge&logo=tensorflow)
![Google Colab](https://img.shields.io/badge/Google_Colab-Ready-yellow?style=for-the-badge&logo=google-colab)

## 📖 Sobre o Projeto

Este repositório contém a implementação de um modelo de Deep Learning que utiliza a técnica de **Transfer Learning** para resolver um problema de classificação de imagens. O objetivo é treinar uma rede neural capaz de diferenciar imagens de gatos e cachorros com alta acurácia.

O projeto foi desenvolvido inteiramente no ambiente Google Colab e faz parte de um desafio proposto pela [Digital Innovation One (DIO)](https://github.com/digitalinnovationone) para colocar em prática os conhecimentos sobre redes neurais e aprendizado por transferência.

---

## 🚀 Desafio Proposto

O desafio consiste em aplicar o método de Transfer Learning em uma rede de Deep Learning na linguagem Python. A base do projeto foi inspirada em um notebook que realiza a mesma técnica com o dataset MNIST, adaptando-a para o famoso dataset "Cats vs Dogs".

### Principais Diretrizes:
- **Tecnologia:** Utilizar Python e bibliotecas de Deep Learning (como TensorFlow/Keras).
- **Ambiente:** Desenvolver no Google Colab para aproveitar o poder das GPUs.
- **Dataset:** Empregar o dataset de Gatos e Cachorros, que é um padrão para problemas de classificação binária de imagens.

---

## 🧠 O que é Transfer Learning?

A Transferência de Aprendizado (Transfer Learning) é uma técnica de Machine Learning onde um modelo desenvolvido para uma tarefa é reutilizado como ponto de partida para um modelo em uma segunda tarefa. Em vez de construir um modelo do zero, aproveitamos os "conhecimentos" (pesos e features) de uma rede já treinada em um grande volume de dados (como a ImageNet) e a adaptamos para nosso problema específico, que geralmente possui um conjunto de dados menor. Isso acelera o treinamento e frequentemente leva a resultados melhores.

---

## 📊 O Dataset: Cats vs. Dogs

O conjunto de dados utilizado foi o "Cats vs. Dogs", originalmente disponibilizado pela Microsoft. Ele contém milhares de imagens de gatos e cachorros, sendo ideal para treinar e validar modelos de visão computacional.

- **Descrição oficial do dataset:** [TensorFlow Datasets - cats_vs_dogs](https://www.tensorflow.org/datasets/catalog/cats_vs_dogs)
- **Link para download:** [Microsoft - Cats vs Dogs Dataset](https://www.microsoft.com/en-us/download/details.aspx?id=54765)

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3
- **Ambiente:** Google Colab
- **Bibliotecas Principais:**
  - TensorFlow e Keras para a construção e treinamento do modelo.
  - Matplotlib e Seaborn para visualização de dados.
  - NumPy para manipulação de arrays.
  - Scikit-learn para métricas de avaliação.

---

## 📈 Etapas do Projeto

1.  **Carregamento e Pré-processamento:** As imagens foram carregadas e preparadas para o modelo (redimensionamento, normalização, etc.).
2.  **Carregamento do Modelo Pré-treinado:** Um modelo robusto (como MobileNetV2, VGG16 ou outro) treinado na base ImageNet foi carregado, sem suas camadas de topo (classificação).
3.  **Congelamento das Camadas:** As camadas do modelo base foram "congeladas" para que seus pesos não fossem atualizados durante o treinamento inicial.
4.  **Adição de Novas Camadas:** Novas camadas de classificação foram adicionadas no topo do modelo base para adaptá-lo ao nosso problema (gatos vs. cachorros).
5.  **Treinamento (Fine-Tuning):** O modelo foi treinado com o nosso dataset, ajustando apenas os pesos das novas camadas.
6.  **Avaliação:** A performance do modelo final foi avaliada em um conjunto de dados de teste para medir sua acurácia e outras métricas.

---

## 👨‍💻 Autor

Projeto desenvolvido por **Michel Rebouças**.

- **LinkedIn:** [Michel Santos Rebouças](https://www.linkedin.com/in/michel-santos-rebou%C3%A7as-5a81b561/)
- **Instagram:** [@satosmichel_oficial](https://www.instagram.com/satosmichel_oficial/)

---

## 🙏 Agradecimentos

Agradecimento especial à [Digital Innovation One (DIO)](https://dio.me/) pela oportunidade de aprendizado e pelo desafio proposto.
