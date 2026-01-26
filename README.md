# Análise de Queda nas Vendas

## Objetivo
Investigar possíveis causas da queda nas vendas usando dados históricos
e gerar insights que possam orientar decisões de negócio.

## Perguntas Principais
- Quando a queda começou?
- A queda foi em volume, valor ou ambos?
- Quais categorias ou produtos mais impactaram a queda?
- A queda é generalizada ou concentrada em regiões/clientes específicos?

## Status
Projeto em desenvolvimento.

## Dataset

Este projeto utiliza um conjunto de dados fictício de vendas criado para projetos de portfólio.

Fonte:[(https://www.kaggle.com/datasets/vinothkannaece/sales-dataset)]

Linhas: 1.000

Colunas: 15

### Tratamento de Anomalias Temporais

Durante a exploração inicial dos dados, foi identificado que o dataset continha registros isolados em janeiro de 2024 (apenas 3 linhas, totalizando 77 unidades vendidas), enquanto todo o restante dos dados se concentrava ao longo de 2023.

Esses registros não representavam um mês completo e distorciam a análise temporal, criando uma queda artificial nas métricas de receita e volume de vendas.

Por esse motivo, os dados de 2024 foram removidos da análise principal, garantindo comparabilidade entre os meses e maior consistência nos resultados apresentados ao longo do projeto.
