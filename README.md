# Previsão de Churn

![image](https://user-images.githubusercontent.com/69591172/198397728-2c98c166-9154-4984-9ffa-75d086e68f64.png)

O **Churn Rate** é a taxa de cancelamento, ou de abandono, registrada em sua base de clientes.

Esta é uma métrica básica para avaliar o sucesso do negócio em alguns setores uma vez que apresenta impacto direto no faturamento. A exemplo dos serviços de assinatura.

## Descrição do Projeto:

Neste projeto foi implementado um modelo de machine learning utilizando algoritmo de classificação para prever possíveis casos de Churn em uma empresa de Telecomunicações. Através da identificação dos possíveis casos de Churn se torna possível utilizar algumas estratégias de marketing com objetivo de reter aqueles clientes. Além da criação do modelo foi realizado também o deploy utilizando Flask.

Para desenvolver o projeto foram necessárias algumas etapas: entendimento do negócio, entendimento dos dados, modelagem, avaliação e deployment.

Foram testados 5 algoritmos de machine learning (Logistic Regression, Random Forest, XGBoost, LightGBM e Catboost) com o objetivo de verificar qual possuia o melhor desempenho de acordo com a métrica técnica escolhida. No processo de escolha, além de considerar os critérios técnicos, foi considerada também o grau de explicabilidade do modelo.

## Comparações entre os Modelos utilizando a métrica ROC-AUC

![dataframe_roc_auc_churn](https://user-images.githubusercontent.com/69591172/207106690-c99c7725-c325-41f9-8970-07148d3c5311.png)

A Regressão Logística além de apresentar o maior grau de explicabilidade dentre estes algoritmos teve também o melhor desempenho de acordo com o parâmetro ROC-AUC, dessa forma, a Regressão Logística foi o algoritmo escolhido.

Em seguida, houve um processo de tunagem visando maximizar o desempenho tendo como parâmetro a métrica técnica escolhida (ROC-AUC).

## Resultado do Modelo não tunado:

![image](https://user-images.githubusercontent.com/69591172/207106387-04597a4f-70b3-4eaa-b275-f6bb9e523fc7.png)


## Resultado do Modelo tunado:

![image](https://user-images.githubusercontent.com/69591172/207107080-6f89abe3-47a9-4eb4-a5fb-0a184c544bbc.png)

## Percentual de Churn por Faixa de Score

![churn_score](https://user-images.githubusercontent.com/69591172/207646725-0ae16c15-d1a1-43ef-80be-2d2c8608af5d.png)

Pode-se notar que:

* Faixa 0: Aproximadamente 0,32% de Churn
* Faixa 1: Aproximadamente 7,28% de Churn
* Faixa 2: Aproximadamente 15,22% de Churn
* Faixa 3: Aproximadamente 17,65% de Churn
* Faixa 4: Aproximadamente 31,19% de Churn
* Faixa 5: Aproximadamente 54,33% de Churn
* Faixa 6: Aproximadamente 67,80% de Churn
* Faixa 7: Aproximadamente 87,88% de Churn

-------------------------------------------------------

Para visualizar melhor o notebook [clique aqui](https://nbviewer.org/github/gustavolenin/Previsao_Churn/blob/main/notebook.ipynb).
