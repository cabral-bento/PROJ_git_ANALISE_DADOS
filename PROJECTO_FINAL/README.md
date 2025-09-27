# Projeto Final – Teste A/B e Análise SQL  
# Final Project – A/B Test and SQL Analysis  

---

## 🇵🇹 Descrição  
Este projeto consolida as habilidades adquiridas nos módulos anteriores, aplicando análise de dados em **teste A/B, consultas SQL e visualização**.  

Principais tarefas:  
1. **Analisar teste A/B**: `recommender_system_test` com grupos A (controle) e B (novo funil de pagamentos); avaliação do funil `product_page → product_cart → purchase`.  
2. **Realizar Análise Exploratória de Dados (AED)**: conversão por etapa do funil, distribuição de eventos por usuário e por dia, identificação de particularidades antes do teste A/B.  
3. **Avaliar estatisticamente o teste A/B**: z-test para diferenças de proporções e conclusões sobre impacto do novo sistema de recomendação.  
4. **Consultar banco de dados SQL**: análise de livros, autores, editoras e avaliações de usuários.  
5. **Gerar conclusões e recomendações**: insights sobre comportamento de usuários e recomendações para estratégias de marketing e produto.  

---

## 🇬🇧 Description  
This project consolidates skills from previous modules by applying **data analysis in A/B testing, SQL queries, and visualization**.  

Main tasks:  
1. **Analyze A/B test**: `recommender_system_test` with groups A (control) and B (new payment funnel); evaluation of the funnel `product_page → product_cart → purchase`.  
2. **Perform Exploratory Data Analysis (EDA)**: conversion per funnel step, distribution of events per user and per day, identify data peculiarities before the A/B test.  
3. **Statistically evaluate A/B test**: z-test for proportion differences and conclusions about the impact of the new recommendation system.  
4. **Query SQL database**: analysis of books, authors, publishers, and user ratings.  
5. **Draw conclusions and recommendations**: insights into user behavior and suggestions for marketing and product strategies.  

---

## 🇵🇹 Dados Utilizados  
- **Teste A/B**  
  - `/datasets/final_ab_new_users_upd_us.csv` – novos usuários  
  - `/datasets/final_ab_events_upd_us.csv` – eventos dos usuários  
  - `/datasets/final_ab_participants_upd_us.csv` – participantes do teste  

- **SQL / Livros e autores**  
  - `/datasets/books.csv`  
  - `/datasets/authors.csv`  
  - `/datasets/publishers.csv`  
  - `/datasets/ratings.csv`  
  - `/datasets/reviews.csv`  

---

## 🇬🇧 Data Used  
- **A/B Test**  
  - `/datasets/final_ab_new_users_upd_us.csv` – new users  
  - `/datasets/final_ab_events_upd_us.csv` – user events  
  - `/datasets/final_ab_participants_upd_us.csv` – test participants  

- **SQL / Books and authors**  
  - `/datasets/books.csv`  
  - `/datasets/authors.csv`  
  - `/datasets/publishers.csv`  
  - `/datasets/ratings.csv`  
  - `/datasets/reviews.csv`  

---

## 🇵🇹 Análise Exploratória e AED  
- Conversão em cada etapa do funil: `product_page`, `product_cart`, `purchase`.  
- Distribuição de eventos por usuário e por dia; verificação de dados inconsistentes.  
- Garantia da presença de usuários em ambos os grupos do teste.  

---

## 🇬🇧 Exploratory Data Analysis (EDA)  
- Conversion at each funnel step: `product_page`, `product_cart`, `purchase`.  
- Distribution of events per user and per day; check for inconsistencies.  
- Ensure users are present in both test groups.  

---

## 🇵🇹 Avaliação do Teste A/B  
- Uso do **z-test** para identificar diferenças estatisticamente significativas entre grupos.  
- Comparação das proporções de conversão em cada etapa do funil.  
- Identificação de impacto do novo sistema de recomendação no comportamento do usuário.  

---

## 🇬🇧 A/B Test Evaluation  
- Use of **z-test** to identify statistically significant differences between groups.  
- Comparison of conversion rates at each funnel step.  
- Assessment of the new recommendation system impact on user behavior.  

---

## 🇵🇹 Análise SQL  
- Número de livros lançados após 01/01/2000.  
- Número de avaliações e classificação média por livro.  
- Editoras com mais livros (>50 páginas).  
- Autor com maior média de classificação (mínimo 50 avaliações).  
- Usuários com mais de 50 avaliações: média de avaliações realizadas.  

---

## 🇬🇧 SQL Analysis  
- Number of books published after 01/01/2000.  
- Number of ratings and average rating per book.  
- Publishers with the most books (>50 pages).  
- Author with highest average rating (min. 50 ratings).  
- Users with more than 50 ratings: average ratings per user.  

---

## 🇵🇹 Conclusões e Recomendações  
- Resultados do teste A/B indicam variação de conversão entre grupos; insights para estratégias de recomendação.  
- Consultas SQL revelam padrões de comportamento de leitores e tendências de publicações.  
- Recomendação: ajustar estratégias de marketing e priorizar autores/editoras com melhor engajamento.  

---

## 🇬🇧 Conclusions and Recommendations  
- A/B test results indicate conversion differences between groups; insights for recommendation strategies.  
- SQL queries reveal reading behavior patterns and publication trends.  
- Recommendation: adjust marketing strategies and prioritize authors/publishers with higher engagement.  
