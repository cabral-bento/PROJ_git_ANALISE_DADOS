# Projeto Sprint 9 – Priorização de Hipóteses e Teste A/B  
# Sprint 9 Project – Hypotheses Prioritization and A/B Testing  

---

## 🇵🇹 Descrição  
Neste projeto, você atuou como analista em uma grande loja online, trabalhando junto ao departamento de marketing. O objetivo foi **priorizar hipóteses de melhorias para aumentar a receita** e **analisar os resultados de um teste A/B** para tomar decisões baseadas em dados.  

O projeto foi dividido em duas partes:  
1. Priorização de hipóteses usando os frameworks **ICE** e **RICE**.  
2. Análise detalhada de um teste A/B com os resultados de pedidos e visitas de usuários.  

---

## 🇬🇧 Description  
In this project, I acted as a business analyst for a large online store, working with the marketing department. The goal was to **prioritize revenue-increasing hypotheses** and **analyze the results of an A/B test** to make data-driven decisions.  

The project was divided into two parts:  
1. Hypotheses prioritization using **ICE** and **RICE** frameworks.  
2. Detailed analysis of an A/B test with user order and visit data.  

---

## 🇵🇹 Dados Utilizados  
**Parte 1 – Hipóteses**  
- `/datasets/hypotheses_us.csv`  
  - Hypotheses — descrição breve  
  - Reach — alcance (1 a 10)  
  - Impact — impacto (1 a 10)  
  - Confidence — confiança (1 a 10)  
  - Effort — esforço necessário (1 a 10)  

**Parte 2 – Teste A/B**  
- `/datasets/orders_us.csv`  
  - transactionId — identificador do pedido  
  - visitorId — identificador do usuário  
  - date — data do pedido  
  - revenue — receita do pedido  
  - group — grupo do teste A/B  
- `/datasets/visits_us.csv`  
  - date — data  
  - group — grupo do teste A/B  
  - visits — número de visitas  

---

## 🇬🇧 Data Used  
**Part 1 – Hypotheses**  
- `/datasets/hypotheses_us.csv`  
  - Hypotheses — brief description  
  - Reach — user reach (1 to 10)  
  - Impact — expected impact (1 to 10)  
  - Confidence — confidence in hypothesis (1 to 10)  
  - Effort — effort required (1 to 10)  

**Part 2 – A/B Test**  
- `/datasets/orders_us.csv`  
  - transactionId — order ID  
  - visitorId — user ID  
  - date — order date  
  - revenue — order revenue  
  - group — A/B test group  
- `/datasets/visits_us.csv`  
  - date — date  
  - group — A/B test group  
  - visits — number of visits  

---

## 🇵🇹 Objetivos do Projeto  
- Priorização de hipóteses:  
  - Aplicar **ICE** e **RICE** para classificar hipóteses por prioridade.  
  - Comparar os resultados dos frameworks e explicar diferenças.  
- Análise de teste A/B:  
  - Visualizar receita acumulada e tamanho médio dos pedidos por grupo.  
  - Calcular taxas de conversão diárias e cumulativas.  
  - Identificar anomalias nos pedidos por usuário e valores de receita.  
  - Testes estatísticos de significância para conversão e tamanho médio do pedido.  
  - Tomar decisão com base nos resultados (parar teste ou continuar).  

---

## 🇬🇧 Project Goals  
- Hypotheses prioritization:  
  - Apply **ICE** and **RICE** frameworks to rank hypotheses by priority.  
  - Compare results and explain differences between frameworks.  
- A/B Test Analysis:  
  - Visualize cumulative revenue and average order value per group.  
  - Calculate daily and cumulative conversion rates.  
  - Identify anomalies in orders per user and revenue values.  
  - Perform statistical significance tests for conversion and average order value.  
  - Make data-driven decision (stop test or continue).  

---

## 🇵🇹 Tecnologias Utilizadas  
- **Python**  
- **Pandas / NumPy** – pré-processamento e análise de dados  
- **Matplotlib / Seaborn / Plotly** – visualização de dados  
- **SciPy / Statsmodels** – testes estatísticos  
- **Jupyter Notebook** – documentação e análise  

## 🇬🇧 Technologies Used  
- **Python**  
- **Pandas / NumPy** – data preprocessing and analysis  
- **Matplotlib / Seaborn / Plotly** – data visualization  
- **SciPy / Statsmodels** – statistical testing  
- **Jupyter Notebook** – documentation and analysis  

---

## 🇵🇹 Principais Resultados  
- Hipóteses classificadas por prioridade usando ICE e RICE.  
- Diferenças identificadas entre priorizações ICE e RICE com justificativas.  
- Visualização da receita acumulada e tamanho médio do pedido por grupo.  
- Cálculo e interpretação da taxa de conversão diária e cumulativa.  
- Identificação de anomalias e outliers nos pedidos.  
- Testes estatísticos indicando significância ou não nas métricas analisadas.  
- Decisão final sobre o teste A/B baseada nos dados.  

## 🇬🇧 Main Results  
- Hypotheses ranked by priority using ICE and RICE.  
- Differences between ICE and RICE prioritizations explained.  
- Visualization of cumulative revenue and average order value per group.  
- Daily and cumulative conversion rates calculated and interpreted.  
- Anomalies and outliers in orders identified.  
- Statistical tests showing significance (or not) in metrics.  
- Final A/B test decision based on data.  

---

## 🇵🇹 Aprendizados  
- Aplicação prática de frameworks de priorização de hipóteses (ICE/RICE).  
- Experiência completa em análise e visualização de resultados de testes A/B.  
- Capacidade de interpretar resultados estatísticos para tomar decisões de negócio.  
- Comunicação clara de insights e recomendações estratégicas baseadas em dados.  

## 🇬🇧 Learnings  
- Practical application of hypotheses prioritization frameworks (ICE/RICE).  
- End-to-end experience in analyzing and visualizing A/B test results.  
- Ability to interpret statistical results for business decisions.  
- Clear communication of insights and data-driven strategic recommendations.  
