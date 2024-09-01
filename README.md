# Time-series-forecasting

## 1.0 Contexto
- Trata-se de uma empresa de venda de commodites que busca prever qual será a porcentagem da meta atigida em janeiro de 2024.

## 2,0 Problema de Negócio
- Prever a porcentagem da meta de vendas em janeiro de 2024, para Colômbia/Equador, Peru e Brasil.

## 3.0 Resumo
- Meu objetivo como Cientista de Dados é realizar uma Análise Exploratória dos Dados (EDA) e identificar oportunidades ocultas nos dados.
- Além disso, será desenvolvido um Modelo de Machine Learning capaz de prever a porcentagem da meta para janeiro de 2024.

## 4.0 Descrição dos Dados

### Temos 23 meses (fevereiro de 2022 a dezembro de 2023) com a porcentagem da meta para cada país
- Month/Year - Mês e ano.
- Value - Valor da meta atingida.
- Country - Paises  

## 5.0 Solução

Para a solução foi aplicada o método CRISP-DS, onde começamos com o acordo do negócio, descobrimos para coleta dos dados, limpeza dos dados, EDA (Análise Exploratória dos dados), modelagem, avaliação do modelo.

Foram desenvolvidos alguns modelos para fazer a previsão de Janeiro de 2024:
- Baseline
- ARIMA
- SARIMA
- LSTM
- Prophet

  ## Tabela comparativa com todos os dados do baseline e dos outros modelos separados por país

  ![image](https://github.com/user-attachments/assets/49c6059f-9802-4da8-925c-3a561967d5d5)

  ### O modelo escolhido foi o Prophet. Segue os graficos da previsão para cada pais:

  - Colômbia - Equador
    
  ![image](https://github.com/user-attachments/assets/9dc91349-1db8-429a-8a9a-c771c7a709b0)

  - Peru

  ![image](https://github.com/user-attachments/assets/9fd9f4e7-383e-40f2-a071-25d38b1fdb67)

  - Brasil

  ![image](https://github.com/user-attachments/assets/e97feab3-b880-4acb-8e59-795cdfe45adc)

## 6.0 Considerações finais
  
Com poucos dados no total 23 meses para cada país, a base de dados não é ideal, mas acredito que o modelo que melhor generalizou foi o Prophet, superando o baseline. Sendo assim, as previsões que considero para janeiro de 2024 são:
| Model   | Country            | Forecast | MAE       | MSE          | RMSE     |
|---------|--------------------|----------|-----------|--------------|----------|
| Prophet | Colombia/Ecuador   | 75.83%   | 3.363194  | 2.478807e+01 | 4.978762 |
| Prophet | Peru               | 79.69%   | 5.017532  | 3.843222e+01 | 6.199373 |
| Prophet | Brasil             | 76.39%   | 2.896693  | 1.638389e+01 | 4.047701 |

## Tabela comparativa da previsão com Janeiro de 2023 para verificar a evolução depois de 12 meses
| Country            | Relação a Janeiro de 2023 |
|--------------------|---------------------------|
| Colombia/Ecuador   |   acréscimo  de  28.52%   |
| Peru               |   acréscimo   de  7.69%   |
| Brasil             |   acréscimo  de  12.34%   |

- Colômbia/Equador: Houve um aumento significativo de 28.52% na meta atingida em relação a janeiro de 2023, indicando um desempenho substancialmente melhor ao longo do ano.
- Peru: Apresenta um crescimento mais moderado, com um acréscimo de 7.69% em relação ao mesmo período do ano anterior.
- Brasil: Registrou um crescimento de 12.34% em relação a janeiro de 2023, mostrando uma tendência de melhoria, embora menos acentuada do que a Colômbia/Equador.


## Tabela comparativa da previsão com Dezembro de 2023 para verificar a evolução sequencial
| Country            | Relação a dezembro 2023 |
|--------------------|-------------------------|
| Colombia/Ecuador   |  acréscimo   de  3.74%  |
| Peru               |  decréscimo  de -5.13%  |
| Brasil             |  acréscimo   de  3.23%  |

- Colômbia/Equador e Brasil: Ambos os países mostram um crescimento em relação a dezembro de 2023, com acréscimos de 3.74% e 3.23%, respectivamente. Isso indica uma tendência positiva para janeiro de 2024.
- Peru: Apresenta uma queda de -5.13% em relação a dezembro de 2023, sugerindo uma possível desaceleração nas vendas para janeiro de 2024.

## 7.0 Proximos passos

- Realizar novos ciclos afim de melhorar o modelo.
- Colocar o modelo em produção.
- Definir como será disponibilizado o acesso ao modelo pelo usuário.
- Melhorar a base de dados.


