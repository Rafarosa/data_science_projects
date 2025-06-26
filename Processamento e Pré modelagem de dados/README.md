# Projeto de Credit Score | Processamento dos dados

Este projeto faz parte do curso Profissão: Cientista de Dados e tem como objetivo aplicar técnicas de pré-processamento, análise exploratória, tratamento de dados e balanceamento de classes para construção de um modelo preditivo de Score de Crédito.

## Objetivo

Desenvolver um pipeline de análise e preparação de dados para prever o risco de inadimplência de clientes, utilizando como variável alvo o Credit Score. O modelo auxilia instituições financeiras na tomada de decisão sobre concessão de crédito.

## Etapas do Projeto

1. **Importação e Exploração dos Dados**
   - Leitura da base de dados de clientes.
   - Análise dos tipos de dados e identificação de valores faltantes.

2. **Tratamento de Dados**
   - Conversão de tipos de dados (ex: renda para float, idade para int).
   - Substituição de valores nulos pela média.
   - Verificação e tratamento de possíveis outliers.

3. **Análise Exploratória**
   - Análise univariada (describe, boxplots, gráficos de barras).
   - Análise bivariada (relações entre idade, renda, escolaridade, número de filhos, score de crédito, etc).
   - Geração de insights sobre o comportamento dos clientes.

4. **Codificação de Variáveis Categóricas**
   - Aplicação de Label Encoder para transformar variáveis categóricas em numéricas.

5. **Análise de Correlação**
   - Avaliação da correlação entre variáveis numéricas e categóricas codificadas.

6. **Divisão da Base**
   - Separação dos dados em conjuntos de treino e teste.

7. **Balanceamento das Classes**
   - Aplicação do SMOTE para balancear as classes da variável alvo no conjunto de treino.

## Principais Conceitos Abordados

- Pré-processamento de dados
- Análise exploratória (EDA)
- Tratamento de valores nulos e outliers
- Codificação de variáveis categóricas
- Análise de correlação
- Balanceamento de classes (SMOTE)
- Preparação de dados para Machine Learning

## Como Executar

1. Instale as dependências necessárias:
   ```
   pip install pandas matplotlib seaborn plotly scikit-learn imbalanced-learn
   ```
2. Execute o notebook `Profissao Cientista de Dados M17 Projeto.ipynb` para acompanhar todas as etapas do projeto.

## Sobre o Credit Score

O Credit Score é uma pontuação que representa a credibilidade de um indivíduo em relação ao cumprimento de obrigações financeiras. Modelos de Credit Score são fundamentais para bancos e instituições financeiras avaliarem o risco de inadimplência de clientes.

---

Projeto desenvolvido para fins educacionais no curso Profissão: Cientista de Dados.