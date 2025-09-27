# Sprint 13 – Projeto de Predição de Rotatividade de Clientes  
# Sprint 13 – Customer Churn Prediction Project  

---

## 🇵🇹 Descrição  
O objetivo deste projeto é **analisar o comportamento dos clientes da rede de academias Model Fitness** e prever a probabilidade de rotatividade para o próximo mês.  

Principais tarefas:  
1. **Carregar e explorar dados** do arquivo `gym_churn_us.csv`.  
2. **Realizar Análise Exploratória de Dados (AED):** estatísticas descritivas, histogramas, correlações e análise de diferenças entre clientes que ficaram e que saíram.  
3. **Construir modelos de predição de rotatividade:** regressão logística e floresta aleatória; comparar desempenho usando acurácia, precisão e sensibilidade.  
4. **Criar agrupamentos de clientes:** análise de clusters via K-means e dendrograma; explorar padrões de características e rotatividade.  
5. **Gerar conclusões e recomendações:** identificar grupos-alvo, sugerir ações para reduzir a rotatividade e otimizar a retenção.  

---

## 🇬🇧 Description  
The goal of this project is to **analyze customer behavior at Model Fitness gyms** and predict the probability of churn for the next month.  

Main tasks:  
1. **Load and explore data** from the `gym_churn_us.csv` file.  
2. **Perform Exploratory Data Analysis (EDA):** descriptive statistics, histograms, correlations, and analysis of differences between retained and churned customers.  
3. **Build churn prediction models:** logistic regression and random forest; compare performance using accuracy, precision, and recall.  
4. **Create customer clusters:** clustering analysis via K-means and dendrogram; explore patterns of features and churn.  
5. **Draw conclusions and provide recommendations:** identify target groups, suggest retention strategies, and optimize customer loyalty.  

---

## 🇵🇹 Dados Utilizados  
- `/datasets/gym_churn_us.csv`  
  - Contém dados demográficos, contratuais e comportamentais de clientes.  
  - Variáveis principais: `Churn`, `gender`, `Near_Location`, `Partner`, `Promo_friends`, `Phone`, `age`, `Lifetime`, `Contract_period`, `Month_to_end_contract`, `Group_visits`, `Avg_class_frequency_total`, `Avg_class_frequency_current_month`, `Avg_additional_charges_total`.  

---

## 🇬🇧 Data Used  
- `/datasets/gym_churn_us.csv`  
  - Contains demographic, contractual, and behavioral data of customers.  
  - Main variables: `Churn`, `gender`, `Near_Location`, `Partner`, `Promo_friends`, `Phone`, `age`, `Lifetime`, `Contract_period`, `Month_to_end_contract`, `Group_visits`, `Avg_class_frequency_total`, `Avg_class_frequency_current_month`, `Avg_additional_charges_total`.  

---

## 🇵🇹 Análise Exploratória (AED)  
- Estatísticas descritivas, médias e desvios padrão por grupo (`Churn`).  
- Histogramas e distribuições de características para clientes que saíram e que permaneceram.  
- Matriz de correlação entre as variáveis para identificar fatores relevantes para rotatividade.  

---

## 🇬🇧 Exploratory Data Analysis (EDA)  
- Descriptive statistics, mean and standard deviation by group (`Churn`).  
- Histograms and feature distributions for churned and retained customers.  
- Correlation matrix among variables to identify relevant factors for churn.  

---

## 🇵🇹 Modelos de Predição  
- **Regressão Logística**: classificação binária para rotatividade.  
- **Floresta Aleatória**: comparação de desempenho com regressão logística.  
- Avaliação: acurácia, precisão e sensibilidade.  
- Random state definido para garantir reprodutibilidade.  

---

## 🇬🇧 Prediction Models  
- **Logistic Regression**: binary classification for churn.  
- **Random Forest**: compared with logistic regression.  
- Evaluation metrics: accuracy, precision, recall.  
- Random state set for reproducibility.  

---

## 🇵🇹 Agrupamento de Clientes (Clusters)  
- Padronização dos dados antes de aplicar o K-means.  
- Dendrograma para estimar o número de clusters.  
- K-means definido com 5 clusters para análise comparativa.  
- Exploração de características médias e distribuição de rotatividade por cluster.  

---

## 🇬🇧 Customer Clustering  
- Data standardized before applying K-means.  
- Dendrogram used to estimate the number of clusters.  
- K-means set to 5 clusters for comparison purposes.  
- Analysis of average features and churn distribution per cluster.  

---

## 🇵🇹 Conclusões e Recomendações  
- Identificação de grupos-alvo com alta probabilidade de rotatividade.  
- Estratégias sugeridas para retenção: promoções, acompanhamento personalizado e incentivos para participação em grupos e aulas.  
- Recomendações sobre comunicação e engajamento de clientes.  

---

## 🇬🇧 Conclusions and Recommendations  
- Target groups with high churn probability identified.  
- Suggested retention strategies: promotions, personalized follow-ups, incentives for group participation and classes.  
- Recommendations on customer communication and engagement.  
