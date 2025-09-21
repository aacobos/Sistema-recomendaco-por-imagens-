# 🖼️ Image Recommendation System

Este projeto implementa um **sistema de recomendação baseado em imagens** utilizando redes neurais pré-treinadas (ResNet50).
O modelo identifica a similaridade visual entre produtos (como relógios, camisetas, sapatos, etc.) e recomenda itens semelhantes pela aparência, sem usar dados textuais como preço ou marca.

---

## 🚀 Tecnologias

* Python 3
* TensorFlow / Keras
* OpenCV
* Scikit-learn
* Matplotlib

---

## 📌 Como funciona

1. **Extração de features**: cada imagem é convertida em um vetor de características usando **ResNet50 pré-treinada no ImageNet**.
2. **Indexação**: os vetores são armazenados em uma matriz de embeddings.
3. **Busca por similaridade**: dado um produto de entrada, o sistema encontra os mais próximos com **KNN (cosine similarity)**.
4. **Recomendação**: retorna imagens visualmente semelhantes ao item buscado.

---

## 📂 Estrutura de diretórios

```
/imagens
   ├── relogio1.jpg
   ├── relogio2.jpg
   ├── camisa1.jpg
   ├── camisa2.jpg
   ├── sapato1.jpg
   └── teste.jpg   # imagem de entrada
```

---

## ▶️ Como usar no Google Colab

1. Clone este repositório ou copie o código do notebook.
2. Crie uma pasta `imagens/` e adicione seus arquivos `.jpg`.
3. Execute o notebook no Colab.
4. Rode o exemplo de teste:

```python
recommend("imagens/teste.jpg")
```

O sistema exibirá a imagem de entrada e suas recomendações mais similares.

---

## 📊 Exemplo de saída

* Input: relógio de pulseira preta
* Output: recomenda relógios de formatos e cores semelhantes.

---

## 🎯 Objetivo

Este projeto tem caráter educacional e demonstra a aplicação de **Deep Learning em sistemas de recomendação visual**.
