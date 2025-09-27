# Sprint 4 – Megaline: Análise Estatística de Planos Pré-pago  
# Sprint 4 – Megaline: Statistical Analysis of Prepaid Plans

---

## 🇵🇹 Descrição do Projeto
Trabalhei como analista para a empresa fictícia **Megaline**, que oferece dois planos pré-pagos (Surf e Ultimate). O objetivo foi analisar o comportamento dos 500 clientes disponíveis (chamadas, mensagens, tráfego web em 2018) e determinar qual plano gera **mais receita média**. O notebook contém limpeza de dados, análise exploratória, visualizações e testes estatísticos para validar diferenças entre grupos.

## 🇬🇧 Project Description
I worked as an analyst for the fictional company **Megaline**, which offers two prepaid plans (Surf and Ultimate). The goal was to analyze the behavior of 500 clients (calls, messages, web traffic in 2018) and determine which plan generates **higher average revenue**. The notebook includes data cleaning, exploratory analysis, visualizations and statistical tests to validate group differences.

---

## 🇵🇹 Objetivos
- Preparar os dados para análise: tipos, nulos, duplicados, correções.  
- Calcular o **uso mensal por usuário** (minutos, número de chamadas, mensagens, dados).  
- Calcular a **receita mensal por usuário** respeitando as regras de arredondamento e preços dos planos.  
- Comparar receitas médias por plano e por região (NY-NJ vs resto) usando testes estatísticos apropriados.  
- Gerar visualizações claras e conclusões acionáveis.

## 🇬🇧 Goals
- Prepare data for analysis: types, missing values, duplicates, corrections.  
- Compute **monthly usage per user** (minutes, call count, messages, data).  
- Compute **monthly revenue per user** following rounding rules and plan prices.  
- Compare mean revenues by plan and by region (NY-NJ vs others) using appropriate statistical tests.  
- Produce clear visualizations and actionable conclusions.

---

## 🇵🇹 Dados (dicionário resumido)
- `users.csv`: user_id, first_name, last_name, age, reg_date, churn_date, city, plan  
- `calls.csv`: id, call_date, duration (minutos), user_id  
- `messages.csv`: id, message_date, user_id  
- `internet.csv`: id, mb_used, session_date, user_id  
- `plans.csv`: plan_name, usd_monthly_fee, minutes_included, messages_included, mb_per_month_included, usd_per_minute, usd_per_message, usd_per_gb

## 🇬🇧 Data (short dictionary)
- `users.csv`: user_id, first_name, last_name, age, reg_date, churn_date, city, plan  
- `calls.csv`: id, call_date, duration (minutes), user_id  
- `messages.csv`: id, message_date, user_id  
- `internet.csv`: id, mb_used, session_date, user_id  
- `plans.csv`: plan_name, usd_monthly_fee, minutes_included, messages_included, mb_per_month_included, usd_per_minute, usd_per_message, usd_per_gb

---

## 🇵🇹 Observações importantes / Regras de arredondamento  
- Chamadas: cada chamada é arredondada **para cima** ao minuto (ex.: 0.2 min → 1 min).  
- Dados móveis: **somatório mensal por usuário em MB → converter para GB** (1 GB = 1024 MB) e o total mensal em GB é arredondado para cima (ex.: 1025 MB → 2 GB).  
- Preços extras: aplicar as tarifas do plano para os excedentes (minutos, mensagens, GB).  
- Verifica se as colunas de data estão em `datetime` e cria coluna `month` para agregação mensal.

## 🇬🇧 Important notes / Rounding rules  
- Calls: each call is **rounded up** to the next minute (e.g., 0.2 min → 1 min).  
- Mobile data: **sum monthly MB per user → convert to GB** (1 GB = 1024 MB) and round up the monthly GB total (e.g., 1025 MB → 2 GB).  
- Apply overage tariffs from the plan for minutes, messages and GB.  
- Ensure date columns are `datetime` and create a `month` column for monthly aggregation.

---

## 🇵🇹 Fluxo de trabalho sugerido (passos)
1. Carregar arquivos e bibliotecas (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy.stats`).  
2. Conversão de tipos e inspeção inicial (`.info()`, `.describe()`, `.isna().sum()`, duplicados).  
3. Limpeza: tratar nulos (documentar decisões), remover duplicados inválidos, padronizar nomes de colunas.  
4. Agregação mensal por usuário: chamadas (count + sum durations arredondadas), mensagens (count), internet (sum mb).  
5. Converter MB → GB e aplicar arredondamento mensal.  
6. Juntar com tabela `users` para obter plano por usuário e com `plans` para preços/limites.  
7. Calcular excedentes e receita mensal por usuário (ver snippet abaixo).  
8. Análises descritivas: média, variância, desvio padrão; histogramas e boxplots por plano.  
9. Testes de hipótese (ver secção abaixo).  
10. Conclusão — sumarizar resultados e recomendações.

## 🇬🇧 Suggested workflow (steps)
1. Load files and libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy.stats`).  
2. Convert types and run initial inspection (`.info()`, `.describe()`, `.isna().sum()`, duplicates).  
3. Cleaning: handle missing values (document decisions), drop invalid duplicates, normalize column names.  
4. Monthly aggregation per user: calls (count + sum durations rounded), messages (count), internet (sum mb).  
5. Convert MB → GB and apply monthly rounding.  
6. Merge with `users` to get each user plan and with `plans` to get prices/limits.  
7. Compute overages and monthly revenue per user (see snippet).  
8. Descriptive analysis: mean, variance, std; histograms and boxplots by plan.  
9. Hypothesis testing (see section below).  
10. Conclusion — summarize results and recommendations.

---
