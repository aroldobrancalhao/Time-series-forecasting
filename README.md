# Time-series-forecasting

## Problema de negócio
- Trata-se de uma empresa de venda de commodites que busca prever qual será a porcentagem da meta atigida em janeiro de 2024.
- Meu objetivo como Cientista de Dados é realizar uma Análise Exploratória dos Dados e identificar oportunidades ocultas nos dados.
- Além disso, será desenvolvido um Modelo de Machine Learning capaz de prever a meta para janeiro de 2024.

## Prever a porcentagem da meta de vendas em janeiro de 2024, para Colômbia/Equador, Peru e Brasil
## Temos 23 meses (fevereiro de 2022 a dezembro de 2023) com a porcentagem da meta para cada país

### Dados Disponíveis:

- Month/Year - Mês e ano.
- Value - Valor da meta atingida.
- Country - Paises  

## Foram desenvolvidos alguns modelos para fazer a previsão de Janeiro de 2024
- Baseline
- ARIMA
- SARIMA
- LSTM
- Prophet

  ## Tabela comparativa com todos os dados do baseline e dos outros modelos separados por país

  ![image](https://github.com/user-attachments/assets/49c6059f-9802-4da8-925c-3a561967d5d5)

  ### o modelo escolhido foiu o Prophet, segue os graficos da previsão para cada pais

  - Colômibia - Ecuador
    
  ![image](https://github.com/user-attachments/assets/9dc91349-1db8-429a-8a9a-c771c7a709b0)

  - Peru

  ![image](https://github.com/user-attachments/assets/9fd9f4e7-383e-40f2-a071-25d38b1fdb67)

  - Brasil

  ![image](https://github.com/user-attachments/assets/e97feab3-b880-4acb-8e59-795cdfe45adc)
  
  ## Com poucos dados no total 23 meses para cada país, não temos uma boa base de dados, mas acredito que o modelo que melhor generalizou foi Prophet, está melhor que baseline, sendo assim as previsões que consideraria para janeiro de 2024 seriam
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

## Tabela comparativa da previsão com Dezembro de 2023 para verificar a evolução sequencial
| Country            | Relação a dezembro 2023 |
|--------------------|-------------------------|
| Colombia/Ecuador   |  acréscimo   de  3.74%  |
| Peru               |  decréscimo  de -5.13%  |
| Brasil             |  acréscimo   de  3.23%  |

## Proximos passos

- 


