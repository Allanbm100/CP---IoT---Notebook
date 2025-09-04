# Checkpoint 01 – Data Science e Machine Learning no Python, Google Colab e Orange Data Mining

Este projeto corresponde ao **Checkpoint 01** da disciplina, dividido em **4 partes**, utilizando **Google Colab (Python)** e a ferramenta **Orange Data Mining**.

---

## 📂 Estrutura da Atividade

### 🔹 Parte 1 – Exercícios iniciais com *Individual Household Electric Power Consumption*
- Análises exploratórias do dataset (estatísticas, datas, valores ausentes).
- Visualizações: linhas, histogramas, séries temporais.
- Agregações por dia, mês, estações do ano.
- Normalização de variáveis e clusterização com K-Means.
- Regressão Linear para previsão de consumo.

### 🔹 Parte 2 – Exercícios adicionais
- Reamostragem em séries temporais (hora em hora).
- Autocorrelação do consumo (lags de 1h, 24h, 48h).
- Redução de dimensionalidade com PCA.
- Visualização de clusters no espaço PCA.
- Comparação entre regressão linear e polinomial.

### 🔹 Parte 3 – Novo dataset: *Appliances Energy Prediction*
- Dataset: [Appliances energy prediction dataset](https://archive.ics.uci.edu/dataset/374/appliances+energy+prediction).
- Análises exploratórias do consumo de eletrodomésticos.
- Correlações com variáveis ambientais.
- Modelagem: Regressão Linear, Random Forest, Clustering e Classificação Binária.
- Avaliação de modelos (RMSE, métricas de classificação).

### 🔹 Parte 4 – Exercícios no Orange Data Mining
- Importação e visualização do dataset.
- Amostragem de 1% dos dados.
- Distribuição do consumo elétrico.
- Relações entre variáveis (Scatter Plot).
- Clusterização com K-Means e análise de padrões de consumo.

---

## 📊 Dataset Principal

**Nome:** Individual household electric power consumption  
**Fonte:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption)  
**Descrição:** Este dataset contém medições do consumo elétrico de uma residência em Paris, França, durante quase 4 anos.  
**Período de coleta:** dezembro de 2006 até novembro de 2010.  
**Tamanho:** ~2.075.259 registros (1 minuto de intervalo entre medições).  
**Formato:** CSV, separado por `;`.

### 🔑 Atributos principais
- **Date**: Data (dd/mm/yyyy)  
- **Time**: Horário (hh:mm:ss)  
- **Global_active_power**: Consumo global ativo em kilowatts  
- **Global_reactive_power**: Consumo global reativo em kilowatts  
- **Voltage**: Voltagem média por minuto (em volts)  
- **Global_intensity**: Intensidade da corrente elétrica (em ampères)  
- **Sub_metering_1**: Consumo de energia em watt-hora (cozinha, fogão/forno/microondas)  
- **Sub_metering_2**: Consumo de energia em watt-hora (lavanderia: máquina de lavar, secadora, etc.)  
- **Sub_metering_3**: Consumo de energia em watt-hora (aquecimento elétrico e climatização)  

---

## ▶️ Instruções de Execução

### Pré-requisitos
- Conta Google ativa para uso do **Google Colab**  
- Bibliotecas Python necessárias:  
  ```python
  import pandas as pd
  import numpy as np
  import matplotlib.pyplot as plt
  from sklearn.preprocessing import MinMaxScaler
  from sklearn.decomposition import PCA
  from sklearn.cluster import KMeans
  from sklearn.linear_model import LinearRegression
  from sklearn.metrics import mean_squared_error


  ### INTEGRANTES
  Allan Brito Moreira - RM558948
  Caio Liang - 558868
  Levi Magni - 98276
