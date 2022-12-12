# Previsão de Churn

![image](https://user-images.githubusercontent.com/69591172/198397728-2c98c166-9154-4984-9ffa-75d086e68f64.png)

O **Churn Rate** é a taxa de cancelamento, ou de abandono, registrada em sua base de clientes.

Esta é uma métrica básica para avaliar o sucesso do negócio em alguns setores uma vez que apresenta impacto direto no faturamento. A exemplo dos serviços de assinatura.

## Descrição do Projeto:

Neste projeto foi implementado um modelo de machine learning utilizando algoritmo de classificação para prever possíveis casos de Churn em uma empresa de Telecomunicações. Através da identificação dos possíveis casos de Churn se torna possível utilizar algumas estratégias de marketing com objetivo de reter aqueles clientes. Além da criação do modelo foi realizado também o deploy utilizando Flask.

Para desenvolver o projeto foram necessárias algumas etapas: entendimento do negócio, entendimento dos dados, modelagem, avaliação e deployment.

Foram testados 5 algoritmos de machine learning (Logistic Regression, Random Forest, XGBoost, LightGBM e Catboost) com o objetivo de verificar qual possuia o melhor desempenho de acordo com a métrica técnica escolhida. No processo de escolha, além de considerar os critérios técnicos, foi considerada também o grau de explicabilidade do modelo.

## Comparações entre os Modelos utilizando a métrica ROC-AUC

![dataframe_roc_auc_churn](https://user-images.githubusercontent.com/69591172/206979210-b67fee73-bbb9-4734-869b-4dedeec416bd.png)

A Regressão Logística além de apresentar o maior grau de explicabilidade dentre estes algoritmos teve também o melhor desempenho de acordo com o parâmetro ROC-AUC, dessa forma, a Regressão Logística foi o algoritmo escolhido.

Em seguida, houve um processo de tunagem visando maximizar o desempenho tendo como parâmetro a métrica técnica escolhida (ROC-AUC).

## Resultado do Modelo não tunado:

![image](https://user-images.githubusercontent.com/69591172/206980307-46309cb2-88b0-4dcf-9f44-65e0f8b24585.png)

## Resultado do Modelo tunado:

![image](https://user-images.githubusercontent.com/69591172/206981056-30d6843c-5aac-4098-9888-66adc11f22bd.png)
