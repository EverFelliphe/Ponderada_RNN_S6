# Time Series Forecasting with Simple RNN - Jena Climate Dataset

Este repositório contém o notebook **`RNNs.ipynb`**, que realiza previsão de séries temporais utilizando uma **RNN simples (SimpleRNN)** no **Jena Climate Dataset**.

## Dataset

O dataset contém medições meteorológicas coletadas a cada 10 minutos em Jena, Alemanha, incluindo:  

- Temperatura (`T (degC)`)  
- Umidade, pressão, vento, entre outras variáveis climáticas  

🔗 [Link do dataset no Kaggle](https://www.kaggle.com/datasets/mnassrib/jena-climate)

## Objetivo

Prever a temperatura futura utilizando uma **Rede Neural Recorrente simples (Simple RNN)**, comparando os resultados de treinamento e avaliação com os valores reais da série temporal.

## Pré-processamento

- Conversão da coluna de datas para `datetime`  
- Seleção da variável alvo `T (degC)`  
- Normalização da variável para a RNN  
- Criação de janelas de tempo (sequências) para treinar o modelo  

## Modelo

- **Simple RNN** com uma camada recorrente e uma camada densa de saída  
- Função de perda: **MSE (Mean Squared Error)**  
- Otimizador: **Adam**  

## Resultados

- Métrica utilizada: **RMSE (Root Mean Squared Error)**  

O notebook apresenta **gráficos comparando valores reais e previstos** da temperatura.

## Como usar

1. Abra o notebook **`RNNs.ipynb`** na raiz do repositório.  
2. Execute as células em ordem para reproduzir os resultados.

## Referências

- [Understanding Simple RNNs — Colah’s Blog](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)  
- [Time Series Forecasting with RNN — Medium](https://towardsdatascience.com/time-series-forecasting-using-rnn-4b4e775151e3)  
- [Jena Climate Dataset — Kaggle](https://www.kaggle.com/datasets/mnassrib/jena-climate)
