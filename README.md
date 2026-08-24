# Credit_risk_analisys_Data_Science

Este projeto simula o ciclo de vida de dados e modelagem de uma carteira de crédito PJ, desde o dado bruto até a sustentação de um modelo em produção. A arquitetura segue o padrão medalhão (Bronze → Silver → Gold) no Databricks, com PySpark e Spark SQL tratando qualidade e consistência dos dados. 

A camada analítica inclui KPIs de carteira (volume, ticket médio, inadimplência por segmento) e uma vintage analysis com window functions, acompanhando a maturação de risco por safra de originação. 

Sobre essa base, foi treinado um modelo de Regressão Logística para probabilidade de inadimplência (PD), avaliado com AUC e KS — métricas padrão de mercado em crédito — e registrado no MLflow para versionamento e auditoria. 

Por fim, o projeto simula 6 meses de operação em produção, monitorando a degradação de performance do modelo (drift) ao longo do tempo, cenário usado para justificar decisões de retreinamento.

[Dashboards SQL no Databricks] (https://dbc-defb6b12-aeca.cloud.databricks.com/dashboardsv3/01f1958762161dbaac6e671e7bb222c8/published?o=7474649354120297)

[Notebook Databricks] (https://dbc-defb6b12-aeca.cloud.databricks.com/editor/notebooks/2429712571117867?o=7474649354120297)
