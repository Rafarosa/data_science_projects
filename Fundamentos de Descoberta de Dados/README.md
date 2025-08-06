# Projeto Supermercado - Fundamentos da Descoberta de Dados

## Descrição

Este projeto tem como objetivo aplicar conceitos estatísticos e de visualização de dados utilizando uma base de produtos de um supermercado do Chile. O trabalho faz parte do Módulo 13 do curso de Ciência de Dados e explora técnicas de análise exploratória, estatística descritiva e gráficos interativos.

## Etapas do Projeto

1. **Leitura dos Dados**
   - Importação da base de dados de produtos via arquivo CSV.
   - Exploração inicial do dataframe e suas colunas.

2. **Análise Estatística**
   - Cálculo da média e mediana dos preços normais (`Preco_Normal`) por categoria.
   - Identificação de categorias com média acima ou abaixo da mediana.
   - Cálculo do desvio padrão dos preços por categoria.

3. **Visualização de Dados**
   - Boxplot da distribuição de preços para a categoria com maior desvio padrão.
   - Gráfico de barras com a média de descontos por categoria.
   - Mapa interativo (treemap) agrupando categoria, marca e média de desconto.

4. **Interpretação**
   - Discussão sobre comportamento dos preços, presença de outliers e dispersão dos dados.
   - Avaliação dos descontos aplicados por categoria e marca.

## Principais Conceitos Abordados

- Estatística descritiva (média, mediana, desvio padrão)
- Agrupamento e análise por categoria
- Visualização com matplotlib e plotly (boxplot, barras, treemap)
- Interpretação de gráficos e insights sobre os dados

## Como Executar

1. Instale as dependências:
   ```
   pip install pandas matplotlib plotly
   ```
2. Execute o notebook `Projeto Supermercado - Fundamentos da Descoberta de Dados.ipynb` para acompanhar todas as etapas do projeto.

## Sobre a Base de Dados

A base contém informações de produtos, marcas, preços (normal, desconto, anterior) e descontos aplicados. As categorias estão em espanhol.

---

Projeto desenvolvido para fins educacionais no curso Profissão: Cientista de Dados.