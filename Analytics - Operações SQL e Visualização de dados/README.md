# Projeto de Análise de E-commerce com SQL e Business Intelligence

Este projeto tem como objetivo consolidar e demonstrar habilidades essenciais de análise de dados, utilizando técnicas avançadas de **SQL** e ferramentas de **Business Intelligence (BI)** em um cenário prático de e-commerce. A análise abrange a integração de dados de clientes e transações para gerar insights de negócio e visualizações interativas.

---

## Conhecimentos Aplicados

Este trabalho foi desenvolvido como parte do módulo de Aprofundamento de Analytics do curso "Profissão: Cientista de Dados" e engloba uma série de conceitos e ferramentas essenciais para a área:

* **Visualização de Dados:** Uso de ferramentas de BI como **Looker Studio** e **Power BI** para criar dashboards.
* **Bancos de Dados e SQL:** Fundamentos e operações avançadas em SQL, incluindo a manipulação de tabelas (`CREATE TABLE`), junções complexas e consultas avançadas.
* **Análise de Dados:** Criação de queries eficientes, filtros, ordenações, cálculos agregados e uso de funções como `DISTINCT` para extração de insights.

---

## Estrutura e Objetivo do Projeto

O projeto se concentra na aplicação prática de técnicas para responder a perguntas de negócio e gerar indicadores relevantes para a tomada de decisões.

### Estrutura dos Dados

O projeto utiliza duas tabelas reais:
* **Tabela de Transações:** Contém registros de vendas, incluindo ID da transação, valor, categoria, e tipo de cartão.
* **Tabela de Clientes:** Armazena informações pessoais como nome, gênero, cidade, estado e profissão.
* **Chave de Ligação:** As tabelas são conectadas pela coluna `ID_CLIENT`.

### Etapas e Análises Realizadas

1.  **Integração de Dados:** As tabelas de clientes e transações foram unidas usando um `RIGHT JOIN` para garantir que todas as transações fossem consideradas na análise, mesmo aquelas sem um cliente cadastrado.
2.  **Exportação e Preparação:** Os dados consolidados foram exportados para um arquivo CSV, facilitando a importação em ferramentas de visualização de dados.
3.  **Construção do Dashboard:** Um dashboard interativo foi criado no **Looker Studio** ou **Power BI** para apresentar as principais métricas e insights, incluindo:
    * Total de vendas e número de transações.
    * Distribuição geográfica e perfil demográfico dos clientes.

### Ferramentas e Tecnologias

* **Linguagens:** Python (com bibliotecas como pandas e sqlite3) e SQL.
* **Ferramentas de BI:** Looker Studio ou Power BI.
* **Base de Dados:** Banco de dados SQLite (`projeto.db`) e arquivos CSV (`dados_ecommerce_final.csv`, `TB_CLIENTES_PROJETO_ECOMM.csv`, `TB_TRANSACOES_PROJETO_ECOMM.csv`).

---

## Como Utilizar o Projeto

Para replicar ou explorar este projeto, siga as etapas:

1.  Instale as bibliotecas Python necessárias (pandas, sqlite3, matplotlib).
2.  Execute o notebook do projeto (`Projeto Analytics e SQL.ipynb`) para seguir o pipeline de análise completo.
3.  Visualize o dashboard final em PDF para ver os principais insights extraídos e as visualizações criadas.