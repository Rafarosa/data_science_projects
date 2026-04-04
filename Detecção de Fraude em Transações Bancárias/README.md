# Projeto Final — Detecção de Fraude em Transações Bancárias

Este projeto faz parte do curso **Profissão: Cientista de Dados** e tem como objetivo aplicar técnicas avançadas de pré-processamento, balanceamento de classes e modelagem preditiva para identificar fraudes em transações de cartão de crédito.

O projeto demonstra um pipeline completo de Ciência de Dados voltado para o setor financeiro, traduzindo resultados técnicos (métricas de avaliação) em recomendações de negócio sólidas para a gestão de risco.

## Objetivo

Desenvolver um modelo preditivo capaz de identificar fraudes em transações bancárias lidando com um cenário de **dados altamente desbalanceados**. A métrica prioritária de negócio é a **minimização de falsos negativos** (fraudes não detectadas pelo sistema). As métricas de avaliação do modelo incluem F1-Score, Recall, Precision e AUC-ROC.

## Dataset

O conjunto de dados analisado pertence ao Banco Global Trust (setembro de 2023) e contém informações de **284.807 transações de cartão de crédito**, com os seguintes atributos principais:

- **Class**: A variável alvo, indicando se a transação é legítima (0) ou fraudulenta (1). O cenário é extremamente desproporcional, com **apenas 0,173% das transações (492) classificadas como fraude**.
- **Time**: Tempo decorrido em segundos desde o início da coleta.
- **Amount**: Valor da transação.
- **V1 a V28**: Features anonimizadas resultantes de uma transformação PCA (Principal Component Analysis) por questões de confidencialidade dos dados dos clientes.

## Etapas do Projeto

1. **Importação e Configuração do Ambiente**
   - Configuração de reprodutibilidade total (`RANDOM_STATE = 42`).
   
2. **Carregamento e Entendimento dos Dados**
   - Verificação da integridade do dataset e validação de valores nulos.

3. **Análise Exploratória de Dados (EDA)**
   - Visualização das distribuições financeiras e estimativa de impacto do prejuízo potencial gerado pelas fraudes.

4. **Pré-processamento e Escalonamento**
   - Normalização da variável `Amount` (altamente assimétrica) utilizando `RobustScaler`.

5. **Tratamento do Desbalanceamento**
   - Aplicação da técnica combinada **SMOTETomek** para gerar amostras sintéticas da classe minoritária e limpar a fronteira de decisão.

6. **Modelagem Baseline**
   - Treinamento inicial e comparação usando três algoritmos distintos: Regressão Logística, Random Forest e XGBoost.

7. **Otimização de Hiperparâmetros**
   - Sintonia fina (Tuning) utilizando `RandomizedSearchCV` com validação cruzada otimizada para o F1-Score.

8. **Comparação e Validação Final**
   - Seleção do modelo vencedor com o melhor equilíbrio entre Recall e Precision.

9. **Conclusões e Recomendações ao Stakeholder**
   - Sugestões de políticas de aprovação baseadas no *score*, calibração do threshold financeiro e regras de retreinamento do modelo.

## Principais Conceitos Abordados

- Lidar com Dados Altamente Desbalanceados (Imbalanced Learning)
- Técnicas de Oversampling/Undersampling híbridas (SMOTETomek)
- Escalonamento robusto a outliers (RobustScaler)
- Algoritmos Baseados em Árvores e Gradient Boosting (Random Forest, XGBoost)
- Otimização de hiperparâmetros (RandomizedSearchCV)
- Avaliação de modelos através do Recall, Precision, F1-Score e Curvas ROC/PR
- Tradução de métricas técnicas em recomendações de negócio

## Tecnologias Utilizadas

- Python
- Pandas & NumPy
- Scikit-learn
- Imbalanced-learn (imblearn)
- XGBoost
- Matplotlib & Seaborn
- Kagglehub
- Jupyter Notebook

## Como Executar

1. Instale as dependências necessárias executando:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost kagglehub