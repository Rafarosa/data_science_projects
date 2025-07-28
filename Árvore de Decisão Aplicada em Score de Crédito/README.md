# Projeto Credit Score - Árvore de Decisão

Este projeto tem como objetivo aplicar o algoritmo de árvore de decisão para prever o score de crédito de clientes, utilizando técnicas de ciência de dados e aprendizado de máquina. O trabalho faz parte do curso Profissão: Cientista de Dados e aprofunda o uso de modelos supervisionados para classificação.

## Objetivo

Construir um modelo preditivo capaz de classificar o score de crédito dos clientes (baixo, médio ou alto) a partir de variáveis socioeconômicas e financeiras, auxiliando instituições financeiras na tomada de decisão sobre concessão de crédito.

## Etapas do Projeto

1. **Pré-processamento dos Dados**
   - Importação das bases de treino e teste.
   - Limpeza, tratamento de valores nulos e codificação de variáveis categóricas.
   - Balanceamento das classes da variável alvo.

2. **Construção do Modelo**
   - Aplicação do algoritmo DecisionTreeClassifier com critério Gini.
   - Treinamento do modelo com os dados balanceados.

3. **Avaliação do Modelo**
   - Cálculo de métricas como acurácia, precisão, recall e f1-score.
   - Análise da matriz de confusão para identificar possíveis problemas de overfitting.
   - Comparação do desempenho entre as bases de treino e teste.

4. **Interpretação e Visualização**
   - Plotagem da árvore de decisão para análise visual das regras criadas.
   - Identificação das features mais importantes para a classificação.

5. **Refinamento**
   - Teste do modelo utilizando apenas as principais features.
   - Discussão sobre o impacto da redução de variáveis e possíveis perdas de desempenho.

6. **Comparação com Outros Modelos**
   - Análise comparativa entre árvore de decisão e Naive Bayes, destacando vantagens e limitações de cada abordagem.

## Principais Conceitos Abordados

- Árvore de decisão para classificação
- Overfitting e generalização
- Importância das features
- Métricas de avaliação de modelos de classificação
- Visualização e interpretação de modelos

## Como Executar

1. Instale as dependências:
   ```
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
2. Execute o notebook `Profissao Cientista de Dados M21 Pratique.ipynb` para acompanhar todas as etapas do projeto.

## Observações

- O modelo de árvore de decisão pode apresentar overfitting se não houver limitação de profundidade ou poda.
- Bases pequenas e bem separadas podem gerar resultados artificialmente altos.
- A escolha das features e o balanceamento das classes são fundamentais para o bom desempenho do modelo.

---

Projeto desenvolvido para fins educacionais no curso Profissão: Cientista de Dados.