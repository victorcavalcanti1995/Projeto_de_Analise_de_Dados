# Python Insights — Análise de Cancelamento de Clientes

## Visão Geral

Este projeto apresenta uma análise exploratória de dados completa com o objetivo de identificar os principais fatores de cancelamento (churn) em uma empresa com mais de 800.000 clientes. O foco foi transformar dados brutos em recomendações estratégicas acionáveis capazes de reduzir o churn e melhorar a retenção de clientes.

---

## Contexto de Negócio

A empresa identificou um alto número de clientes inativos e precisava responder três questões principais:

• Quais fatores estão mais associados ao cancelamento?
• Quais ações podem reduzir o churn de forma efetiva?
• Qual o impacto estimado dessas ações?

---

## Metodologia

1. Ingestão de dados com Pandas
2. Limpeza e validação da base
3. Análise Exploratória de Dados (EDA)
4. Visualização das variáveis com Plotly
5. Identificação de padrões de churn
6. Simulação de cenários para estimar impacto de mudanças operacionais

A base utilizada é pública, originalmente disponibilizada no Kaggle, em formato CSV.

---

## Principais Descobertas

Três variáveis apresentaram forte correlação com cancelamento:

1. Clientes com contrato mensal apresentaram maior taxa de churn.
2. Clientes com mais de quatro ligações ao suporte tiveram probabilidade elevada de cancelamento.
3. Clientes com atraso superior a vinte dias no pagamento quase sempre cancelaram o serviço.

---

## Recomendações de Negócio

• Incentivar contratos anuais ou de longo prazo por meio de estratégia de preços.
• Implementar alerta operacional após três ligações ao suporte.
• Criar notificações preventivas antes de quinze dias de atraso no pagamento.

---

## Simulação de Impacto

Após filtrar clientes afetados pelos três principais fatores, a taxa de cancelamento caiu de **56% para 18%**, indicando alto potencial de impacto com melhorias direcionadas.

---

## Tecnologias Utilizadas

• Python
• Pandas
• Plotly
• Jupyter Notebook

Conceitos aplicados: Limpeza de Dados, Análise Exploratória de Dados, Visualização de Dados, Analytics para Negócios.

---

## Estrutura do Repositório

```
project/
 ├── cancelamentos.csv
 ├── analysis.ipynb
 └── README.md
```

---

## Possíveis Evoluções

• Modelo preditivo de churn com Machine Learning
• Pipeline automatizado de dados
• Dashboard interativo com Streamlit ou ferramentas de BI
• Testes A/B para estratégias de retenção

---

## Autor

Victor Cavalcanti
