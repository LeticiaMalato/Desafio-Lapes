# Desafio-Lapes


---
Este projeto realiza uma análise abrangente de um dataset de startups, utilizando técnicas de Machine Learning e visualização de dados. O foco está em entender o que aconteceu no passado, identificar os fatores que influenciam o sucesso ou fracasso das startups, e prever o status futuro de novas startups.

## Objetivos do Projeto

1. **O que aconteceu?**  
   Realizar uma análise descritiva do dataset.

2. **Por que aconteceu?**  
   Identificar os fatores que influenciam o sucesso ou fracasso das startups.

3. **O que vai acontecer?**  
    Fazer previsões sobre o status de futuras startups.

## Requisitos

Antes de executar o código, certifique-se de ter instalado as seguintes bibliotecas Python:

```bash
pip install pycaret
```

## Importação de Bibliotecas

As seguintes bibliotecas são utilizadas no projeto:

```python
import pandas as pd
from pycaret.classification import *
from sklearn.datasets import load_breast_cancer
from sklearn.ensemble import GradientBoostingClassifier
from sklearn.model_selection import train_test_split
from sklearn.metrics import classification_report
from sklearn import metrics
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.metrics import confusion_matrix
import folium
from folium.plugins import HeatMap
import numpy as np
from itertools import combinations
```

## Estrutura do Código

### 1. Carregamento e Análise Descritiva do Dataset

Nesta seção, o dataset será carregado e explorado para entender as principais características das startups. Serão geradas estatísticas descritivas e visualizações para identificar padrões e outliers.

### 2. Identificação dos Fatores de Sucesso ou Fracasso

Aqui, utilizamos o PyCaret e o Scikit-learn para construir modelos de classificação que ajudam a identificar os fatores que mais influenciam o sucesso ou fracasso das startups. Técnicas como Gradient Boosting e análise de importância das variáveis são aplicadas.

### 3. Previsões para Startups Futuras

Nesta etapa, usamos os modelos treinados para fazer previsões sobre o status de futuras startups, aplicando técnicas de validação cruzada e métricas de desempenho para avaliar a precisão dos modelos.

