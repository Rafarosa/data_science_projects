# Projeto de Previsão de Intenção de Compra em E-commerce

Este projeto aplica algoritmos de Machine Learning para prever se um visitante de uma loja virtual realizará uma compra ou não. O objetivo é otimizar estratégias de marketing digital e aumentar a taxa de conversão através da identificação antecipada de leads qualificados.

## Contexto de Negócio
No comércio eletrônico, a taxa de conversão média é baixa. Identificar usuários com alta propensão de compra em tempo real permite:
- Otimizar o budget de campanhas de remarketing.
- Personalizar ofertas (ex: cupons) para indecisos.
- Reduzir o Custo de Aquisição de Cliente (CAC).

## Objetivo
Construir e comparar modelos de classificação para prever a variável `Revenue` (Venda: Sim/Não) com base em métricas de navegação (tempo na página, *bounce rate*, *page values*) e características do visitante.

## Tecnologias e Ferramentas
- **Linguagem:** Python 3
- **Manipulação de Dados:** Pandas, Numpy
- **Visualização:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-Learn (Regressão Logística, Random Forest)
- **Ambiente:** Jupyter Notebook

## Metodologia
O projeto seguiu um pipeline estruturado de Ciência de Dados:
1. **Análise Exploratória (EDA):** Estudo de correlações e comportamento de navegação.
2. **Pré-processamento:** - Codificação de variáveis categóricas (*Label Encoding* e *One-Hot Encoding*).
   - Padronização de variáveis numéricas (*StandardScaler*).
   - Divisão em treino e teste.
3. **Modelagem:** Treinamento comparativo entre um modelo linear (Regressão Logística) e um modelo de conjunto (Random Forest).
4. **Avaliação:** Uso de métricas de Acurácia e Matriz de Confusão.

## Resultados e Performance
O modelo **Random Forest** apresentou desempenho superior, demonstrando maior capacidade de generalização para este problema.

| Modelo | Acurácia | Observação |
| :--- | :--- | :--- |
| **Random Forest** | **91.96%** | Melhor capacidade de capturar padrões não-lineares. |
| Regressão Logística | 85.49% | Boa baseline, mas limitada pela linearidade. |

> **Conclusão de Negócio:** Com uma assertividade próxima de 92%, o modelo é viável para implementação em motores de recomendação e segmentação de campanhas em tempo real.

## Como Executar
1. Clone o repositório.
2. Instale as dependências:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn