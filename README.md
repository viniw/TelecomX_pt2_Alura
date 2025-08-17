Relatório (como "Empresa") de Análise de Evasão de Clientes - TelecomX


Resumo Executivo

A análise teve como objetivo identificar os fatores que levam os clientes da TelecomX a cancelarem seus serviços (churn). Foram utilizados dois modelos preditivos, Regressão Logística e Random Forest, para prever a probabilidade de um cliente evadir. Os resultados indicam que o modelo Random Forest obteve o melhor desempenho, sendo mais eficaz na identificação de clientes em risco. A principal descoberta é que a cobrança mensal (MonthlyCharges), o tempo de serviço (Tenure) e o tipo de serviço (ServiceType) são os fatores mais relevantes para a evasão.


Análise e Desempenho dos Modelos

Os modelos foram avaliados por diversas métricas, como acurácia, ROC AUC e relatório de classificação, com um foco especial na capacidade de identificar corretamente os clientes que realmente evadiriam (classe 'Yes' ou 1).



Regressão Logística

Acurácia: 81.33%

ROC AUC: 84.72%

Relatório de Classificação:

Precisão (Precision): 76% (A cada 10 clientes que o modelo previu que iriam evadir, 7.6 realmente evadiram).

Recall: 47% (O modelo identificou apenas 47% de todos os clientes que realmente evadiram).

Random Forest
Acurácia: 83.17%

ROC AUC: 87.16%

Relatório de Classificação:

Precisão (Precision): 75% (A cada 10 clientes que o modelo previu que iriam evadir, 7.5 realmente evadiram).

Recall: 57% (O modelo identificou 57% de todos os clientes que realmente evadiram).

Conclusão sobre os Modelos
O modelo Random Forest demonstrou um desempenho superior em todas as métricas-chave, especialmente no ROC AUC e no Recall para a classe de evasão ('Yes'). A curva ROC do Random Forest está mais próxima do canto superior esquerdo do gráfico, indicando uma melhor capacidade de distinguir entre clientes que evadem e que não evadem. A maior taxa de Recall (57%) significa que o modelo Random Forest é mais eficaz em encontrar os clientes "escondidos" que estão prestes a evadir, o que é crucial para uma estratégia de retenção.

Fatores de Evasão (Análise de Importância das Variáveis)
A análise de importância das variáveis, extraída do modelo Random Forest, revelou os seguintes fatores como os mais influentes na decisão de um cliente de cancelar o serviço:

MonthlyCharges (Cobrança Mensal): Este é o fator mais relevante. Clientes com mensalidades mais altas têm uma probabilidade significativamente maior de evadir. Isso pode estar relacionado à percepção de valor do serviço em relação ao custo ou a ofertas mais competitivas no mercado.

Tenure (Tempo de Serviço): A duração do relacionamento do cliente com a empresa é o segundo fator mais importante. A evasão tende a ser maior entre clientes com baixo tempo de serviço (novos clientes) ou aqueles com contratos de longa duração que podem estar procurando por uma mudança ou melhores ofertas.

ServiceType (Tipo de Serviço): O tipo de serviço contratado também é um fator crítico. É provável que um dos tipos de serviço, como "Fibra", tenha uma taxa de churn mais alta devido a problemas de qualidade, instabilidade de rede ou concorrência mais acirrada.

Age (Idade): Embora menos impactante que os três primeiros, a idade do cliente também contribui para a decisão de evadir.

Gender (Gênero): O gênero do cliente foi o fator menos relevante na análise, indicando que não há uma correlação significativa entre gênero e evasão.

Estratégias de Retenção Propostas
Com base nas descobertas, propomos as seguintes estratégias para mitigar a evasão de clientes:

Revisar a Política de Preços:

Focar em clientes com altas cobranças mensais. A empresa pode oferecer planos mais flexíveis, descontos para fidelidade ou pacotes personalizados que justifiquem o custo mais elevado.

Criar ofertas especiais ou bônus para clientes de longa data, garantindo que eles se sintam valorizados e evitem a busca por alternativas.

Priorizar a Retenção de Clientes Novos:

Focar em clientes que têm um curto tempo de serviço (Tenure baixo). O processo de onboarding deve ser aprimorado para garantir que novos clientes tenham uma experiência positiva e completa desde o início.

Oferecer um acompanhamento proativo nos primeiros meses de serviço, como ligações de verificação ou suporte dedicado para resolver quaisquer problemas iniciais.

Melhorar a Qualidade do Serviço:

Realizar uma análise aprofundada do ServiceType mais problemático para identificar as causas da alta taxa de evasão. Isso pode envolver a melhoria da infraestrutura, o aumento da velocidade ou a resolução de problemas de conectividade.

Comunicar de forma clara os benefícios do serviço para o cliente e destacar o valor do produto em relação ao seu preço.

Implementar um Sistema de Alerta Precoce:

Utilizar o modelo Random Forest para criar uma pontuação de risco para cada cliente. Clientes com alta probabilidade de evasão podem ser sinalizados para a equipe de retenção, permitindo que a empresa entre em contato de forma proativa.

A equipe de retenção pode usar esta informação para fazer ofertas personalizadas, resolver problemas pendentes ou simplesmente reforçar o valor do serviço.
