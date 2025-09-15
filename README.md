# Análise de Crédito - Projeto Ciência de Dados

## Descrição
Projeto para prever a **inadimplência de clientes** usando o dataset [UCI Credit Card](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients).  
O objetivo principal é identificar clientes **adimplentes** (`DEFAULT=0`) para oferecer crédito de forma segura.

## Estrutura do Projeto

data/
  ├── raw/          # Dados originais
  └── processed/    # Dados tratados e escalonados
models/             # Modelos treinados
notebooks/          # Notebooks de exploração, pré-processamento, EDA, modelagem e avaliação
requirements.txt
Dockerfile
docker-compose.yml

## Execução com Docker
```
docker-compose up --build -d
```

Acesse o Jupyter em: http://localhost:8888

## Notebooks

1. 01_exploracao.ipynb – Exploração inicial dos dados.  
2. 02_preprocessamento.ipynb – Limpeza, feature engineering, seleção de features e escalonamento.  
3. 03_eda.ipynb – Visualização e análise exploratória.  
4. 04_modelagem.ipynb – Treinamento de Random Forest e Logistic Regression, com otimização de hiperparâmetros.  
5. 05_avaliacao.ipynb – Avaliação dos modelos, ajuste de threshold e comparação das métricas.

## Resultados
- Identificação das **features mais importantes** para prever adimplência.  
- Comparação de métricas (Precisão, Recall, F1) entre treino e teste.  
- Modelos treinados salvos em `models/`.

## Dependências
pandas, numpy, scikit-learn, matplotlib, seaborn, imbalanced-learn, statsmodels, joblib, jupyter
