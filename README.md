# Python Insights - Análise de Cancelamento de Clientes

## Sobre o Projeto
Este projeto foi desenvolvido para uma empresa com mais de 800 mil clientes que estava enfrentando um alto índice de cancelamentos. O objetivo principal foi analisar os dados dos clientes para identificar os principais motivos que levam ao cancelamento do serviço e propor soluções eficientes para reduzir esse número.

## Contexto
A empresa percebeu que a maioria dos seus clientes são inativos (já cancelaram o serviço) e precisa entender:
- Principais causas dos cancelamentos
- Ações mais eficientes para reduzir a taxa de cancelamento
- Padrões de comportamento dos clientes que cancelam

## Fonte de Dados
Os dados utilizados neste projeto foram obtidos do Kaggle e estão disponíveis no [Google Drive](https://drive.google.com/drive/folders/1uDesZePdkhiraJmiyeZ-w5tfc8XsNYFZ?usp=drive_link).

## Tecnologias Utilizadas
- **Python** (Linguagem principal)
- **Pandas** (Manipulação e análise de dados)
- **Plotly Express** (Visualização de dados)
- **Jupyter Notebook** (Ambiente de desenvolvimento)

## Estrutura do Projeto

### Passo 1: Importação da Base de Dados
```python
import pandas as pd
tabela = pd.read_csv('cancelamentos.csv')
```

### Passo 2: Visualização Inicial dos Dados
- Análise das informações disponíveis
- Identificação de problemas na base
- Remoção de colunas desnecessárias (CustomerID)

### Passo 3: Tratamento de Dados
- Verificação de valores nulos
- Limpeza dos dados inconsistentes
- Preparação para análise

### Passo 4: Análise Exploratória
- Identificação da taxa de cancelamento atual
- Análise estatística inicial

### Passo 5: Análise Detalhada com Visualizações
Utilização de gráficos interativos para cada coluna, segmentando por clientes que cancelaram ou não.

## Principais Descobertas

### Causas Críticas de Cancelamento:
1. **Contrato Mensal**: 100% dos clientes com contrato mensal cancelaram
2. **Ligações para o Call Center**: Clientes com mais de 4 ligações cancelaram
3. **Atraso no Pagamento**: Atrasos superiores a 20 dias resultaram em cancelamento

### Soluções Propostas:

| Problema | Solução | Ação |
|----------|---------|------|
| Contrato Mensal | Incentivar planos mais longos | Oferecer descontos em planos anual/quadrimestral |
| Muitas ligações | Melhorar atendimento | Alerta vermelho com 3+ ligações |
| Atraso no pagamento | Prevenir inadimplência | Alerta vermelho com 15+ dias de atraso |

## Resultados Obtidos

### Antes da Intervenção:
- Taxa de cancelamento: **56,5%**

### Após as Medidas Corretivas:
- Taxa de cancelamento: **18,4%**

**Redução de 38,1 pontos percentuais na taxa de cancelamento!**

## Principais Insights

1. **Segmentação de Contratos**: Clientes em contratos mensais são mais propensos a cancelar
2. **Atendimento ao Cliente**: Qualidade do suporte influencia diretamente na retenção
3. **Gestão de Inadimplência**: Atrasos prolongados são fortes preditores de cancelamento

## Como Executar o Projeto

1. Clone este repositório
2. Instale as dependências:
   ```bash
   pip install pandas plotly
   ```
3. Baixe a base de dados do [Google Drive](https://drive.google.com/drive/folders/1uDesZePdkhiraJmiyeZ-w5tfc8XsNYFZ?usp=drive_link)
4. Execute o notebook Jupyter

## Recomendações Finais

- Implementar sistema de alertas preventivos
- Criar programa de fidelidade para contratos longos
- Investir em treinamento da equipe de suporte
- Estabelecer políticas de cobrança mais eficientes

---
**Nota**: Este projeto demonstra como a análise de dados pode gerar insights valiosos para tomada de decisão e redução de custos com cancelamentos.
