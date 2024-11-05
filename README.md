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

- NumPy: pip install numpy
- DeepFace: pip install deepface
- OpenCV: pip install opencv-python
- Pillow: pip install Pillow
- scikit-learn: pip install scikit-learn
- Matplotlib: pip install matplotlib
- Google Colab: Se você estiver executando este código no Google Colab, algumas bibliotecas específicas do Colab serão necessárias.

## Executando o Código   
- Faça o download do código completo pelo link: [Notebook Principal](https://github.com/Camillabgarcia/agrupamento_facial/blob/main/agrupamento_por_semelhan%C3%A7a.ipynb)
- Certifique-se de ter todas as dependências instaladas e execute o código em um ambiente Python.
- O pipeline executa todas as etapas descritas, desde a clonagem do repositório até a visualização dos grupos finais de imagens.

## Descrição do Código

1. Clonagem do Repositório: O código clona um repositório do GitHub que contém imagens de rostos para serem processadas..

2. Carregamento e Melhoria das Imagens: As imagens são carregadas de um diretório específico, redimensionadas para 250x250 pixels, e o contraste é aumentado para melhorar a qualidade visual.

3.Geração de Embeddings: Utiliza a biblioteca DeepFace para gerar embeddings (representações vetoriais) de cada imagem. O modelo Facenet é empregado para capturar características faciais relevantes..

4. Agrupamento de Embeddings: Os embeddings são agrupados utilizando o algoritmo KMeans para formar 10 clusters, permitindo a identificação de imagens similares.

5. Reorganização dos Grupos: Os grupos são reorganizados para garantir que cada um contenha exatamente 4 imagens similares, baseando-se na similaridade de cosseno entre os embeddings. 

6. Visualização dos Grupos: As imagens agrupadas são visualizadas em um gráfico, onde cada grupo de imagens é exibido em uma linha separada, facilitando a análise visual dos resultados

## Exemplo de Saída
   
![Sáida](https://github.com/Camillabgarcia/agrupamento_facial/blob/main/Resultado.jpg?raw=true)
