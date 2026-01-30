# Análise de Queda nas Vendas — Julho/2023
 Análise de queda de vendas em Julho/2023 usando Python e Pandas 
 
## Resumo Executivo
Investigamos a queda observada em Julho/2023. A retração foi concentrada na **região South**, puxada pela **categoria Mobília (Furniture)**, que caiu ~60% nas unidades. A evidência indica que o aumento do preço médio (de R$2.466 → R$3.331) foi o principal fator associado à redução da demanda.

---

## Objetivo
Identificar por que as vendas caíram, apontando período, regiões, categorias e causas prováveis para gerar recomendações acionáveis.

---

## Dataset
Conjunto fictício (1.000 linhas). Principais colunas: `Sale_Date`, `Region`, `Sales_Amount`, `Quantity_Sold`, `Product_Category`, `Sales_Rep`, `Sales_Channel`, `Discount`, `Unit_Price`.  
Fonte: Kaggle (dataset usado para portfólio).

---

## Tratamento de Dados
Removidos registros isolados de Janeiro/2024 (3 linhas) por não representarem mês completo e distorcerem a comparação temporal. Análise concentrada em **2023**.

---

## Principais Achados
- **Ponto de ruptura:** Julho/2023.  
- **Região mais impactada:** South (queda percentual ≈ **41,39%** em unidades).  
- **Categoria principal:** Mobília (226 → 91 unidades; **−59,73%**).  
- **Causa provável:** aumento do **preço médio** da categoria (R$2.466 → R$3.331); desconto médio manteve-se ≈ 14%.

---

## Interpretação
A queda foi localizada e explicável: aumento de preço/mudança de mix em Mobília na região South reduziu a demanda. Não foi um problema apenas de representante — afetou a região inteira.

---

## Recomendações (prioridade)
1. Revisar política de preços/mix para Mobília no South (testes A/B antes de mudanças amplas).  
2. Implementar alertas de queda por categoria/região (detecção rápida).  
3. Verificar disponibilidade de SKU e estratégia de portfólio (itens acessíveis vs. premium).  
4. Analisar canais e desempenho de representantes para ações localizadas.  
5. Construir dashboard mensal por região × categoria.

---

## Próximos passos técnicos
- Validar impacto por canal (`Sales_Channel`) e tipo de cliente.  
- Checar estoque/rotatividade de SKUs em Mobília.  
- Produzir 2 gráficos finais para relatório: (1) evolução mensal da receita; (2) comparação Junho vs Julho — Mobília (South).

---
## 📊 Gráficos principais

### Queda por região
![Queda por região](images/grafico_regiao.png)

### Queda percentual por categoria (South)
![Queda por categoria](images/grafico_categoria.png)

## Tecnologias
Python, Pandas, Jupyter Notebook, Matplotlib.

---

## Autor
Pedro Henrike — análise para portfólio (vagas de Analista de Dados Júnior).
