# TelecomX_pt2_Alura

Relatório de Análise de Evasão de Clientes (Churn) - Alura - Challenge 3

📌 Visão GeralEste projeto realiza uma análise preditiva dos fatores que influenciam a evasão de clientes (churn) no setor de telecomunicações. Utilizando técnicas de machine learning, identificamos os principais determinantes do churn e propomos estratégias baseadas em dados para redução da rotatividade de clientes.

📊 Métricas dos Modelos
ModeloAcuráciaROC AUCPrecisãoRecallRegressão Logística79%0.8364%52%Random Forest81%0.8668%57%

🔍 Principais Fatores de Churn
Tipo de Contrato: Contratos mensais aumentam o risco de churn em 3.2 vezes.
Tempo como Cliente: Relação inversamente proporcional; clientes com pouco tempo são mais propensos à evasão.
Valor Mensal: Clientes com cobranças mais altas têm maior churn, indicando possível insatisfação com o valor percebido.
Serviços Adicionais: A falta de serviços como segurança online e suporte técnico é um forte indicador de evasão.
Tipo de Internet: Clientes com serviço de Fibra Óptica apresentam maior churn que os de DSL, possivelmente devido a altas expectativas não atendidas.

🛠️ Como Usar
Pré-requisitos: Python 3.8 + Bibliotecas 

💡 Estratégias PropostasIncentivos para contratos de longo prazoProgramas de fidelização para novos clientesOtimização de planos e preçosPromoção de serviços de valor agregadoMelhoria do serviço de fibra óptica
