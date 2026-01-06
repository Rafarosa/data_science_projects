# Projeto de Segmentação de Clientes | Clustering com K-Means

Este projeto faz parte do curso **Profissão: Cientista de Dados** e tem como objetivo aplicar técnicas de análise exploratória, pré-processamento de dados e modelagem não supervisionada para segmentação de clientes utilizando o algoritmo **K-Means**.

O projeto demonstra um pipeline completo de Ciência de Dados, desde a compreensão do dataset até a interpretação dos clusters e sua aplicação prática em contextos de negócio.

## Objetivo

Desenvolver um modelo de **segmentação de clientes** baseado em comportamento de consumo e características demográficas, permitindo identificar grupos com perfis semelhantes e apoiar estratégias de marketing direcionadas, personalização de ofertas e tomada de decisão baseada em dados.

## Dataset

O conjunto de dados contém informações de **200 clientes**, com os seguintes atributos:

- **CustomerID**: Identificador único do cliente  
- **Gender**: Gênero do cliente  
- **Age**: Idade  
- **Annual Income (k$)**: Renda anual em milhares de dólares  
- **Spending Score (1–100)**: Pontuação atribuída com base no comportamento de consumo  

## Etapas do Projeto

1. **Importação e Exploração dos Dados**
   - Leitura do dataset.
   - Análise dos tipos de variáveis.
   - Identificação de valores ausentes e inconsistências.

2. **Análise Exploratória de Dados (EDA)**
   - Estatísticas descritivas.
   - Visualização da distribuição das variáveis.
   - Identificação de padrões de comportamento e possíveis outliers.

3. **Tratamento e Pré-processamento**
   - Limpeza de dados.
   - Padronização das variáveis numéricas utilizando `StandardScaler`.
   - Preparação da base para algoritmos de clusterização.

4. **Implementação do Algoritmo K-Means**
   - Aplicação do algoritmo K-Means.
   - Testes com diferentes valores de *k*.
   - Utilização do método do cotovelo (Elbow Method).

5. **Avaliação dos Clusters**
   - Avaliação da qualidade dos clusters utilizando **Silhouette Score**.
   - Análise visual da separação entre os grupos.

6. **Interpretação dos Resultados**
   - Caracterização dos clusters com base nas variáveis originais.
   - Identificação de perfis de clientes distintos.
   - Discussão sobre a utilidade prática de cada segmento.

7. **Aplicações de Negócio**
   - Sugestões de estratégias de marketing direcionadas.
   - Personalização de ofertas conforme o perfil do cluster.
   - Apoio à tomada de decisão em estratégias comerciais.

## Principais Conceitos Abordados

- Análise exploratória de dados (EDA)
- Pré-processamento e normalização de dados
- Modelagem não supervisionada
- Algoritmo K-Means
- Avaliação de clusters (Silhouette Score)
- Interpretação de resultados para negócio
- Segmentação de clientes

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Como Executar

1. Instale as dependências necessárias:
   ```
   pip install pandas matplotlib seaborn plotly scikit-learn imbalanced-learn
   ```
2. Execute o notebook `Projeto de Segmentação de Clientes K-Means.ipynb` para acompanhar todas as etapas do projeto.

## Sobre Segmentação de Clientes

A segmentação de clientes é uma técnica fundamental em Ciência de Dados e Marketing Analytics, permitindo agrupar consumidores com características semelhantes. Modelos de clusterização, como o K-Means, ajudam empresas a entender padrões de comportamento, aumentar a eficiência de campanhas e melhorar a experiência do cliente.

---

Projeto desenvolvido para fins educacionais no curso **Profissão: Cientista de Dados**, com foco na construção de portfólio em Ciência de Dados e Machine Learning.