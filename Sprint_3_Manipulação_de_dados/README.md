# Projeto Instacart – Análise de Hábitos de Compra / Instacart Project – Customer Shopping Habits

---

## 🇵🇹 Descrição do Projeto
Neste projeto, trabalhei com um subconjunto dos dados públicos da **Instacart** (conjunto originalmente disponibilizado para uma competição na Kaggle em 2017). O dataset foi reduzido e contém exemplos de valores faltantes e duplicados para simular um ambiente real de limpeza e preparação de dados.  
Minha missão foi limpar os dados, explorar padrões de comportamento dos clientes e apresentar insights acionáveis através de visualizações e um relatório em um Jupyter Notebook. Todos os gráficos incluem título, eixos rotulados e legenda quando necessário. Cada resposta às perguntas do enunciado contém uma explicação em formato Markdown no notebook.

## 🇬🇧 Project Description
In this project I worked with a subset of the public **Instacart** dataset (originally released for a Kaggle competition in 2017). The dataset was downsampled and intentionally includes missing values and duplicates to simulate a real-world cleaning task.  
My mission was to clean the data, explore customer behavior patterns, and present actionable insights through visualizations and a report in a Jupyter Notebook. All plots include a title, labeled axes, and a legend when necessary. Every answer to the project questions is written as a Markdown explanation in the notebook.

---

## 🇵🇹 Objetivos
- Limpar e pré-processar os dados (tratar valores ausentes, remover/justificar duplicados, normalizar colunas).
- Entender o comportamento de compra dos clientes (frequência, itens mais comprados, horários/dias, etc.).
- Responder às perguntas do enunciado com código e explicações em Markdown.
- Construir visualizações claras e informativas (com `plt.show()` no fim de cada célula de plot).

## 🇬🇧 Goals
- Clean and preprocess the data (handle missing values, remove/justify duplicates, normalize columns).
- Understand customer shopping behavior (frequency, top items, time/day patterns, etc.).
- Answer the project questions with code and Markdown explanations.
- Produce clear, informative visualizations (include `plt.show()` at the end of each plotting cell).

---

## 🇵🇹 Tecnologias e Bibliotecas
- Python 3.x  
- Jupyter Notebook  
- pandas, numpy  
- matplotlib, seaborn, plotly (opcional para interatividade)  
- scikit-learn (apenas se fizeres clusterização ou transformações avançadas)  

## 🇬🇧 Technologies & Libraries
- Python 3.x  
- Jupyter Notebook  
- pandas, numpy  
- matplotlib, seaborn, plotly (optional for interactivity)  
- scikit-learn (only if you perform clustering or advanced transforms)  

---

## 🇵🇹 Arquivos Fornecidos (exemplo)
- `orders.csv` — informações dos pedidos.  
- `order_products.csv` — relação pedidos × produtos (re-orders, etc.).  
- `products.csv` — catálogo de produtos.  
- `aisles.csv` / `departments.csv` — categorias.  
> *Nota: os nomes dos ficheiros podem variar conforme o material que recebeste; ajusta conforme necessário.*

## 🇬🇧 Provided Files (example)
- `orders.csv` — orders information.  
- `order_products.csv` — order × product relationships (re-orders, etc.).  
- `products.csv` — product catalog.  
- `aisles.csv` / `departments.csv` — categories.  
> *Note: filenames might vary depending on the material you received; adapt as needed.*

---

## 🇵🇹 Passo a Passo Sugerido (Notebook)
1. **Carregar bibliotecas e dados**  
   - Importar `pandas`, `numpy`, `matplotlib.pyplot as plt`, `seaborn` e definir opções (ex.: `pd.set_option('display.max_columns', None)`).

2. **Inspeção inicial**  
   - `df.head()`, `df.info()`, `df.describe()`, contagem de nulos: `df.isna().sum()`.

3. **Limpeza de Dados**  
   - Tratar valores ausentes (dependendo da coluna: imputar, remover ou sinalizar).  
   - Remover ou justificar duplicados: `df.duplicated().sum()`, `df.drop_duplicates()` quando aplicável.  
   - Conversões de tipo (datas, inteiros, categorias).  
   - Normalizar rótulos de colunas (lowercase, strip).

4. **Transformações necessárias**  
   - Criar colunas derivadas (ex.: `order_hour_of_day`, `days_since_prior_order` categorizado, número de itens por pedido).  
   - Agrupar dados para responder às perguntas (ex.: por cliente, por produto, por dia/hora).

5. **Análises / Perguntas Típicas**  
   - Quais são os 10 produtos mais pedidos? (barra horizontal).  
   - Como se distribuem os pedidos ao longo do dia/semana? (line / bar).  
   - Percentual de reorders vs. pedidos iniciais.  
   - Top departamentos/aisles por volume de vendas.  
   - Quantos pedidos por cliente (distribuição) — identificar clientes frequentes.  
   - Existe padrão sazonal ou semanal nos pedidos?  
   - (Opcional) Segmentação simples de clientes pelo número de pedidos e taxa de re-order.

6. **Visualizações**  
   - Sempre adicionar `plt.title()`, `plt.xlabel()`, `plt.ylabel()` e, quando necessário, `plt.legend()`.  
   - Coloca `plt.tight_layout()` antes de `plt.show()` para garantir apresentação limpa.

7. **Conclusões e Recomendações**  
   - Para cada análise, escreve uma célula Markdown com interpretação dos resultados e possíveis ações (ex.: promoção de produtos mais reordenados, horários para campanhas).

## 🇬🇧 Suggested Notebook Workflow
1. **Load libraries & data**  
   - Import `pandas`, `numpy`, `matplotlib.pyplot as plt`, `seaborn`, set options (e.g. `pd.set_option('display.max_columns', None)`).

2. **Initial inspection**  
   - `df.head()`, `df.info()`, `df.describe()`, count missing: `df.isna().sum()`.

3. **Data cleaning**  
   - Handle missing values (impute, drop or flag depending on column).  
   - Remove/justify duplicates: `df.duplicated().sum()`, `df.drop_duplicates()` if applicable.  
   - Type conversion (dates, integers, categories).  
   - Normalize column names (lowercase, strip).

4. **Necessary transforms**  
   - Create derived columns (e.g. `order_hour_of_day`, categorize `days_since_prior_order`, items per order).  
   - Aggregate to answer questions (by customer, product, day/hour).

5. **Analyses / Typical questions**  
   - Top 10 most ordered products (horizontal bar).  
   - Orders distribution across hours/days (line / bar).  
   - Percentage of reorders vs first orders.  
   - Top departments/aisles by volume.  
   - Orders per customer distribution — identify frequent customers.  
   - Any weekly/seasonal pattern?  
   - (Optional) Simple customer segmentation by orders count and reorder rate.

6. **Visualizations**  
   - Always add `plt.title()`, `plt.xlabel()`, `plt.ylabel()` and `plt.legend()` when needed.  
   - Use `plt.tight_layout()` then `plt.show()`.

7. **Conclusions & Recommendations**  
   - For each result, write a Markdown cell interpreting the findings and proposing actions (e.g., promote highly re-ordered products, schedule campaigns at peak hours).

---

## 🇵🇹 Entregáveis (O que deves submeter)
- Um **Jupyter Notebook** (.ipynb) com:  
  - Células de código completas e comentadas.  
  - Células Markdown com explicações após cada pergunta.  
  - Gráficos com título, eixos e `plt.show()`.  
- (Opcional) Arquivo `requirements.txt` com as dependências usadas.

## 🇬🇧 Deliverables (What to submit)
- A **Jupyter Notebook** (.ipynb) containing:  
  - Completed and commented code cells.  
  - Markdown cells with explanations after each question.  
  - Plots with titles, axis labels and `plt.show()`.  
- (Optional) `requirements.txt` listing used dependencies.

---

## 🇵🇹 Exemplo de Texto (Markdown) para cada resposta
> **Pergunta:** Quais são os 10 produtos mais pedidos?  
> **Resposta (exemplo):** Os 10 produtos mais pedidos representam X% do total de itens vendidos. Observa-se que produtos básicos de mercearia e snacks estão no topo, sugerindo que ações de cross-sell com estes itens podem aumentar o ticket médio. (Inclui a figura X com um gráfico de barras horizontais.)

## 🇬🇧 Example Markdown Text for each answer
> **Question:** What are the top 10 most ordered products?  
> **Answer (example):** The top 10 products account for X% of total items sold. Basic grocery items and snacks dominate the list, suggesting that cross-sell promotions with these items could increase average order value. (Include figure X showing a horizontal bar chart.)

---