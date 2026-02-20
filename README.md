📊 Telecom X – Análise de Evasão de Clientes (Churn)

Projeto desenvolvido como parte do desafio Telecom X - Análise de Churn, com o objetivo de identificar fatores associados à evasão de clientes e gerar insights que possam ajudar a empresa a reduzir cancelamentos.

🎯 Objetivo

A empresa Telecom X enfrenta um alto índice de cancelamentos de clientes (churn). Este projeto tem como objetivo:

Coletar e tratar os dados

Realizar análise exploratória (EDA)

Identificar padrões de evasão

Gerar insights estratégicos

Apoiar futuras análises preditivas

🛠️ Tecnologias utilizadas

Python

Pandas

NumPy

Matplotlib

Seaborn

Google Colab / Jupyter Notebook

📂 Estrutura do Projeto
telecom-x-churn/
│
├── challenge_telecom_x.ipynb
├── README.md
🔄 ETL – Extração, Transformação e Limpeza
Extração

Os dados foram importados a partir de uma API contendo informações de clientes da Telecom X.

Transformação

Foram realizados os seguintes tratamentos:

Padronização de nomes de colunas

Conversão de variáveis numéricas:

charges_monthly

charges_total

tenure

Tratamento de valores inválidos

Criação de variáveis categóricas (faixas de valores)

Exemplo:

df.loc[:, 'charges_total'] = pd.to_numeric(df['charges_total'], errors='coerce')
Limpeza

Verificação de valores ausentes

Ajuste de tipos de dados

Remoção de inconsistências

📊 Análise Exploratória de Dados

Foram realizadas análises descritivas e visuais para identificar padrões de evasão.

Análise Descritiva
df.describe(include='all')

Principais variáveis analisadas:

Churn

Tipo de contrato

Método de pagamento

Tempo de contrato

Valor mensal

Valor total gasto

📈 Principais Análises
Churn por Tipo de Contrato

Clientes com contrato mensal (Month-to-month) apresentaram maior taxa de evasão.

Clientes com contrato anual ou bianual apresentaram menor churn.

Churn por Valor Mensal

Foi analisada a taxa de churn em diferentes faixas de valor mensal.

Observação:

Clientes com valores mensais mais altos apresentaram maior tendência de cancelamento.

Churn por Valor Total

Clientes com baixo valor total gasto apresentam maior churn, indicando cancelamento precoce.

Clientes com maior valor total tendem a permanecer mais tempo.

Tempo de Contrato vs Churn

Foi observada uma forte relação entre tempo de contrato e evasão:

Clientes com pouco tempo de contrato cancelam mais.

Clientes antigos tendem a permanecer.

Variáveis Categóricas

Foram analisadas:

Gênero

Contrato

Método de pagamento

Serviços contratados

Principais observações:

Contrato mensal apresenta maior churn

Pagamento via Electronic Check apresenta maior evasão

Contratos mais longos reduzem churn

💡 Principais Insights

Clientes com contrato mensal cancelam mais

Clientes novos apresentam maior churn

Valores mensais altos aumentam a evasão

Clientes com baixo gasto total cancelam mais

Métodos de pagamento influenciam o churn

🚀 Recomendações

Com base na análise, recomenda-se:

1️⃣ Incentivar contratos mais longos

Clientes com contratos anuais ou bianuais apresentam menor churn.

Sugestão:

Oferecer descontos para contratos longos

2️⃣ Melhorar retenção de clientes novos

Clientes com pouco tempo de contrato cancelam mais.

Sugestão:

Programas de boas-vindas

Suporte inicial

3️⃣ Revisar preços e planos

Valores mensais altos estão associados a maior churn.

Sugestão:

Planos intermediários

Descontos progressivos

4️⃣ Melhorar experiência de pagamento

Métodos específicos apresentam maior evasão.

Sugestão:

Incentivar pagamento automático

Facilitar cobrança

📌 Conclusão

A análise exploratória permitiu identificar fatores importantes relacionados à evasão de clientes.

Os resultados obtidos podem servir como base para:

Modelos preditivos de churn

Estratégias de retenção

Tomada de decisão

👩‍💻 Autora

Gabrielle Corteze

Projeto desenvolvido para fins educacionais.
