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
 
O conjunto de dados contém 1000 registros e inclui as seguintes colunas principais:

- Data da venda (`Sale_Date`)
- Região (`Region`)
- Valor da venda (`Sales_Amount`)
- Quantidade vendida (`Quantity_Sold`)
- Categoria do produto (`Product_Category`)
- Representante de vendas (`Sales_Rep`)
- Canal de vendas (`Sales_Channel`)
- Método de pagamento, desconto e tipo de cliente

---

## 🧹 Tratamento Inicial dos Dados

### Remoção de registros isolados em 2024

Durante a exploração inicial, foram encontrados poucos registros em Janeiro de 2024 (apenas 3 linhas).

Esses dados não representavam um mês completo e distorciam a análise temporal, criando uma queda artificial nas métricas.

Por isso, os registros de 2024 foram removidos para manter consistência:

- Período analisado: **Janeiro a Dezembro de 2023**

---

## 📈 Análise Temporal

Ao agrupar as vendas mensalmente, observou-se que:

- A receita se manteve relativamente estável ao longo do ano
- A maior queda de unidades ocorreu em **Julho/2023**

---

## 🌍 Queda por Região

A região com maior impacto foi:

### **South**

- Maior queda absoluta de unidades
- Maior queda percentual

**Queda percentual em Julho: 41,39%**

Enquanto outras regiões apresentaram quedas médias entre 20% e 25%.

---

## 🪑 Queda por Categoria (South)

Ao segmentar a região South por categoria, foi identificado que a queda foi altamente concentrada em:

### **Mobília (Furniture)**

- Junho: 226 unidades  
- Julho: 91 unidades  
- Queda: −135 unidades (**−59,73%**)

Outras categorias tiveram quedas menores:

- Comida: −41%
- Roupa: −29%
- Eletrônicos: −13%

➡️ Isso indica que o colapso nas vendas de Mobília foi o principal fator da queda na região South.

---

## Investigação do Representante David (Mobília — South)

Inicialmente, observou-se que David teve uma queda expressiva nas vendas de Mobília entre Junho e Julho.

Porém, ao analisar suas vendas totais, foi identificado que ele continuou ativo em Julho, com crescimento em categorias como Food e Electronics.

O que ocorreu foi uma forte mudança no mix de vendas:

- Mobília caiu de 158 para 31 unidades (−127)
- Enquanto outras categorias aumentaram ou se mantiveram

Isso indica que a queda não foi causada pela ausência do representante, mas sim por uma redução específica na categoria Mobília, possivelmente relacionada a fatores como desconto, preço médio ou canal de vendas.


---

## ✅ Conclusões Parciais

Até o momento, os principais insights foram:

- Julho/2023 teve a maior retração de unidades vendidas
- A região South foi a mais afetada
- A categoria Mobília concentrou a maior parte da queda
- Representantes específicos podem ter contribuído para o colapso

---

## 🚀 Próximos Passos

- Analisar impacto por canal de vendas
- Avaliar efeito de descontos e tipo de cliente
- Construir recomendações finais para o negócio

---

## 🛠️ Tecnologias Utilizadas

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

---

## ✍️ Autor

Pedro Henrique  
Projeto desenvolvido para portfólio e preparação para vagas de Analista de Dados Júnior.


Colunas: 15

### Tratamento de Anomalias Temporais

Durante a exploração inicial dos dados, foi identificado que o dataset continha registros isolados em janeiro de 2024 (apenas 3 linhas, totalizando 77 unidades vendidas), enquanto todo o restante dos dados se concentrava ao longo de 2023.

Esses registros não representavam um mês completo e distorciam a análise temporal, criando uma queda artificial nas métricas de receita e volume de vendas.

Por esse motivo, os dados de 2024 foram removidos da análise principal, garantindo comparabilidade entre os meses e maior consistência nos resultados apresentados ao longo do projeto.
