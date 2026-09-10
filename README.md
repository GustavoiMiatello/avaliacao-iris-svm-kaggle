# Avaliação do Dataset Iris com SVM no Kaggle

## Sobre o projeto

Este projeto foi desenvolvido como uma atividade acadêmica de Machine Learning utilizando o dataset Iris obtido diretamente do Kaggle.

O objetivo é realizar uma Análise Exploratória dos Dados (EDA), preparar os dados e desenvolver um modelo de classificação utilizando exclusivamente o algoritmo Support Vector Machine (SVM).

## Dataset

O dataset utilizado é o **Iris Species**, disponibilizado no Kaggle.

Dataset:
https://www.kaggle.com/datasets/menegidio/iris-species

Os dados utilizados foram obtidos diretamente do arquivo `Iris.csv` disponibilizado pelo dataset.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook
- Kaggle

## Etapas realizadas

O projeto foi desenvolvido seguindo as seguintes etapas:

1. Importação das bibliotecas necessárias.
2. Importação do dataset Iris.
3. Análise exploratória dos dados.
4. Verificação da estrutura e das características do dataset.
5. Verificação de valores ausentes.
6. Análise da distribuição das espécies.
7. Preparação dos dados para o treinamento.
8. Divisão dos dados em conjuntos de treinamento e teste.
9. Criação do modelo de classificação utilizando SVM.
10. Treinamento do modelo.
11. Realização das previsões.
12. Avaliação do modelo utilizando métricas de classificação.
13. Análise da matriz de confusão.
14. Interpretação dos resultados.

## Preparação dos dados

A coluna `Id` foi retirada por representar apenas o identificador dos registros.

A coluna `Species` foi utilizada como variável alvo, enquanto as características:

- SepalLengthCm
- SepalWidthCm
- PetalLengthCm
- PetalWidthCm

foram utilizadas como variáveis de entrada do modelo.

Os dados foram divididos em:

- 80% para treinamento
- 20% para teste

Foi utilizado `stratify=y` para manter a proporção das classes durante a divisão dos dados.

## Modelo utilizado

O único algoritmo de classificação utilizado no projeto foi o **Support Vector Machine (SVM)**.

Foi utilizado o `SVC` da biblioteca Scikit-learn com **kernel linear**.

```python
model = SVC(kernel='linear')
