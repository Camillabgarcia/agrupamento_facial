**Agrupamento Facial por Semelhança**

Este projeto é uma aplicação para agrupar imagens de rostos semelhantes utilizando técnicas de aprendizado de máquina e processamento de imagem. A aplicação lê um dataset de rostos, gera embeddings usando a 
biblioteca **DeepFace** e utiliza o algoritmo KMeans para agrupar as imagens de acordo com a similaridade.

**Estrutura do projeto**

agrupamento_facial/

- faces/                    # Diretório com as imagens de entrada

- agrupamento_por_semelhança.ipynb    # Notebook principal

- README.md                # Este arquivo

## Pré-requisitos

Antes de executar o projeto, certifique-se de que você possui as seguintes dependências instaladas:

- Python 3.6 ou superior.
- pip (gerenciador de pacotes do Python).
- Bibliotecas Python a serem instaladas: `numpy`, `deepface`, `opencv-python`, `Pillow`, `scikit-learn`, `matplotlib`.

## Instalação
1. Baixe o repositório do projeto diretamente do GitHub:
   
   Acesse o link:(https://github.com/Camillabgarcia/agrupamento_facial)
   
3. Faça o download do código pelo link: [Notebook Principal](https://github.com/Camillabgarcia/agrupamento_facial/blob/main/agrupamento_por_semelhan%C3%A7a.ipynb)

4. Instale as dependências necessárias:
   ```bash
   pip install numpy deepface opencv-python Pillow scikit-learn matplotlib

## Uso
1. Coloque as imagens a serem agrupadas no diretório ./faces.
   
2. Execute o script agrupamento_por_semelhanca.ipynb no Google Colab ou em um ambiente Jupyter Notebook.

3. Importações necessária:
   
import os

import numpy as np

import git

from deepface import DeepFace

import cv2

from PIL import Image, ImageEnhance

from sklearn.cluster import KMeans

from sklearn.metrics.pairwise import cosine_similarity

import matplotlib.pyplot as plt

5. O script irá:

-Clonar o repositório do projeto, caso não exista localmente.

-Carregar e melhorar as imagens do diretório ./faces.

-Gerar os embeddings das imagens usando o modelo DeepFace.

-Agrupar os embeddings usando o algoritmo KMeans com 10 clusters.

-Reorganizar os grupos para garantir 10 grupos(0-9) com exatamente 4 imagens similares.

-Exibir a visualização dos grupos finais.

5. Exemplo de Saída
   
![Sáida](https://github.com/Camillabgarcia/agrupamento_facial/blob/main/Resultado.jpg?raw=true)
