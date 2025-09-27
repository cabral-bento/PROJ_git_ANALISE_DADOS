# Sprint 11 – Projeto de Análise de Funil e Teste A/A/B  
# Sprint 11 – Funnel Analysis and A/A/B Test  

---

## 🇵🇹 Descrição  
Você trabalha em uma startup de produtos alimentícios e seu objetivo é **analisar o comportamento dos usuários no aplicativo**.  

O projeto envolve duas etapas principais:  
1. **Análise do funil de vendas:** identificar como os usuários avançam pelas etapas do aplicativo até a compra, quais fases apresentam maior perda e qual a proporção de usuários que completa todo o funil.  
2. **Análise de teste A/A/B:** comparar dois grupos de controle com fontes antigas e um grupo de teste com novas fontes, verificando qual conjunto gera melhores resultados e se os grupos foram distribuídos corretamente.  

O foco é analisar métricas de comportamento, construir visualizações e aplicar testes estatísticos para decisões de design.  

---

## 🇬🇧 Description  
You work at a food products startup, and your goal is to **analyze user behavior in the app**.  

The project has two main parts:  
1. **Funnel analysis:** identify how users progress through app stages to purchase, which stages have the highest drop-off, and the proportion of users completing the full funnel.  
2. **A/A/B test analysis:** compare two control groups with the old fonts and one test group with new fonts, evaluating which fonts produce better outcomes and whether groups were assigned correctly.  

The focus is on behavior metrics, visualizations, and statistical tests to support design decisions.  

---

## 🇵🇹 Dados Utilizados  
- `/datasets/logs_exp_us.csv`  
  - EventName — nome do evento  
  - DeviceIDHash — identificador único do usuário  
  - EventTimestamp — data e hora do evento  
  - ExpId — identificador do experimento (246, 247: controle; 248: teste)  

---

## 🇬🇧 Data Used  
- `/datasets/logs_exp_us.csv`  
  - EventName — event name  
  - DeviceIDHash — unique user identifier  
  - EventTimestamp — event timestamp  
  - ExpId — experiment identifier (246, 247: control; 248: test)  

---

## 🇵🇹 Objetivos do Projeto  
- Preparar e limpar os dados do registro de eventos.  
- Explorar o número de eventos, usuários e frequência de ações.  
- Construir histogramas e analisar o período de dados confiáveis.  
- Estudar o funil de eventos: proporção de usuários em cada etapa, identificar perdas e calcular a taxa de conversão do funil completo.  
- Analisar resultados do teste A/A/B:  
  - Comparar grupos de controle para verificar semelhança estatística.  
  - Comparar o grupo de teste com os grupos de controle para cada evento.  
  - Determinar se a mudança de fontes gera impacto positivo ou negativo.  
- Aplicar testes estatísticos e definir nível de significância adequado.  
- Tirar conclusões e recomendações baseadas em dados.  

---

## 🇬🇧 Project Goals  
- Prepare and clean event log data.  
- Explore the number of events, users, and action frequency.  
- Build histograms and analyze the period of reliable data.  
- Study the event funnel: user proportion at each stage, identify drop-offs, and calculate full funnel conversion rate.  
- Analyze A/A/B test results:  
  - Compare control groups to verify statistical similarity.  
  - Compare the test group to control groups for each event.  
  - Determine if the font change has a positive or negative impact.  
- Apply statistical tests and set an appropriate significance level.  
- Draw conclusions and recommendations based on the data.  

---

## 🇵🇹 Tecnologias Utilizadas  
- **Python**  
- **Pandas / NumPy** – manipulação e limpeza de dados  
- **Matplotlib / Seaborn / Plotly** – visualização de funil e comparações  
- **Scipy / Statsmodels** – testes estatísticos (significância)  
- **Jupyter Notebook** – documentação da análise  

## 🇬🇧 Technologies Used  
- **Python**  
- **Pandas / NumPy** – data cleaning and manipulation  
- **Matplotlib / Seaborn / Plotly** – funnel and comparison visualizations  
- **Scipy / Statsmodels** – statistical significance tests  
- **Jupyter Notebook** – analysis documentation  

---

## 🇵🇹 Principais Resultados  
- Número total de eventos e usuários analisados.  
- Distribuição de eventos por frequência e proporção de usuários que executaram cada ação.  
- Identificação de etapas com maior perda de usuários no funil.  
- Taxa de conversão do funil completo.  
- Comparação estatística entre grupos de controle (246 e 247) para verificar confiabilidade.  
- Comparação do grupo de teste (248) com os controles para medir impacto da mudança de fontes.  
- Conclusões sobre quais fontes apresentam melhor desempenho.  

## 🇬🇧 Main Results  
- Total number of events and users analyzed.  
- Event distribution by frequency and proportion of users performing each action.  
- Identification of funnel stages with highest user drop-off.  
- Full funnel conversion rate.  
- Statistical comparison between control groups (246 and 247) to ensure reliability.  
- Test group (248) comparison with controls to measure font change impact.  
- Conclusions on which fonts perform better.  

---

## 🇵🇹 Aprendizados  
- Capacidade de análise de funil de vendas e comportamento do usuário.  
- Experiência em testes A/A/B e interpretação de significância estatística.  
- Extração de insights acionáveis para decisões de design e UX.  

## 🇬🇧 Learnings  
- Ability to analyze sales funnels and user behavior.  
- Experience with A/A/B tests and interpreting statistical significance.  
- Extracting actionable insights for design and UX decisions.  
