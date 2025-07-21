# 6-Challenge-TelecomX2

Telecom X – Parte 2: Prevendo Churn


Relatório de Análise de Evasão de Clientes
1. Introdução
Este relatório apresenta a análise dos fatores que mais influenciam a evasão (churn) de clientes com base em um conjunto de dados da TelecomX. Foram avaliados diferentes modelos preditivos para identificar padrões e prever a saída de clientes, além de apontar estratégias para retenção.

2. Preparação dos Dados
As variáveis categóricas foram transformadas em variáveis numéricas utilizando One-Hot Encoding.

Dados foram balanceados por meio de undersampling para corrigir o desbalanceamento da classe evasão (aproximadamente 73% clientes ativos e 27% evadidos).

O dataset final contém X variáveis e Y amostras (incluir números reais do seu caso).

3. Modelos Avaliados
Regressão Logística: Modelo linear, interpretável, usado com normalização dos dados.

Random Forest: Modelo baseado em árvores, não requer normalização, robusto a variáveis irrelevantes.

(Se aplicável, inclua outros modelos, como KNN ou SVM)

Desempenho dos Modelos (exemplo):
Modelo	Acurácia	Precisão	Recall	F1-score
Regressão Logística	0.78	0.75	0.70	0.72
Random Forest	0.82	0.80	0.74	0.77

4. Análise dos Fatores que Influenciam a Evasão
4.1 Regressão Logística
As variáveis com maior peso positivo, que aumentam a probabilidade de evasão, incluem:

Contrato mensal (Month-to-month)

Ausência de contrato de longo prazo (One year, Two year)

Ausência de serviços de segurança online

Senior Citizen (Idade mais avançada)

Variáveis que reduzem a evasão (coeficientes negativos):

Contrato anual ou bienal

Clientes com parceiros (Partner_Yes)

Clientes com dependentes (Dependents_Yes)

4.2 Random Forest
As variáveis mais importantes para o modelo (top 5) foram:

Tempo de contrato (tenure)

Tipo de contrato (Contract)

Serviço de internet (InternetService)

Cobrança mensal (Monthly Charges)

Segurança online (OnlineSecurity)

4.3 Interpretação geral
Tempo e tipo de contrato são os fatores mais fortes associados à retenção.

Clientes em contratos curtos (mensal) apresentam maior risco de evasão.

Serviços adicionais como segurança online tendem a diminuir a evasão.

Clientes mais velhos e sem dependentes parecem mais propensos a sair.

5. Estratégias de Retenção Propostas
Com base nos fatores acima, sugerimos as seguintes estratégias:

Incentivar contratos de longo prazo: Oferecer descontos ou benefícios para clientes que optam por contratos anuais ou bienais, reduzindo churn mensal.

Promoções em serviços adicionais: Destacar serviços de segurança online, suporte e pacotes combinados que aumentam o valor percebido.

Campanhas específicas para clientes seniors: Personalizar ofertas e suporte para clientes mais velhos, buscando aumentar satisfação e retenção.

Monitoramento do tempo de contrato: Criar alertas para clientes próximos ao término do contrato mensal e oferecer vantagens para renovação.

Análise contínua e segmentação: Refinar modelos para identificar grupos de risco e ajustar ações específicas para diferentes perfis.

6. Conclusão
A análise revelou que o tipo e tempo de contrato, bem como a oferta de serviços adicionais, são determinantes para a evasão. Modelos preditivos como Random Forest forneceram boa precisão e indicaram claramente as variáveis mais relevantes. A implementação das estratégias propostas pode reduzir significativamente a evasão e aumentar a fidelidade dos clientes.

