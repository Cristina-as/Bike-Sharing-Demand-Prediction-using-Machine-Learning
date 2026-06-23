# Bike-Sharing-Demand-Prediction-using-Machine-Learning
O objetivo deste projeto é desenvolver modelos preditivos capazes de estimar a quantidade de bicicletas alugadas com base em fatores ambientais e comportamentais, auxiliando empresas de mobilidade urbana na tomada de decisão operacional.

# Objetivo do Projeto

O objetivo deste projeto é desenvolver modelos preditivos capazes de estimar a quantidade de bicicletas alugadas com base em fatores ambientais e comportamentais, auxiliando empresas de mobilidade urbana na tomada de decisão operacional.

---

# Problema de Negócio

Sistemas de compartilhamento de bicicletas precisam prever a demanda de utilização para:

- otimizar distribuição de bicicletas
- reduzir custos operacionais
- evitar falta de bicicletas
- melhorar experiência dos usuários
- identificar padrões de comportamento

A previsão da demanda permite maior eficiência operacional e melhor planejamento estratégico.

---

# Dataset

O projeto utiliza o **Bike Sharing Dataset**, contendo dados históricos de aluguel de bicicletas da cidade de Washington D.C., EUA.

O dataset inclui informações sobre:

- temperatura
- umidade
- velocidade do vento
- estação do ano
- dia da semana
- horário
- condições climáticas
- usuários casuais e registrados

Dataset original disponibilizado por:
- Capital Bikeshare
- University of Porto

---

# Tecnologias Utilizadas

## Linguagens e Bibliotecas
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

## Machine Learning
- Linear Regression
- Random Forest Regressor

## Ferramentas
- Google Colab
- GitHub
- Power BI

---

# Estrutura do Projeto

```bash
bike-sharing-demand-prediction/
│
├── data/
│   ├── day.csv
│   └── hour.csv
│
├── notebooks/
│   └── bike_sharing_analysis.ipynb
│
├── images/
│
├── README.md
├── requirements.txt
└── .gitignore

Etapas Desenvovidas:
Importação dos Datasets;
Análise das Variáveis;
Entendimento do problema de negócio;
Definição da variável Target.

Análise Exploratória de Dados(EDA):
Foram realizadas análises estatísticas e visuais para identificar padrões e tendências da demanda.

Principais Análises:
Distribuição da Demanda;
Sazonalidade;
Impacto climático;
Horários de Pico;
Correlação entre Variáveis;
Comportamento Temporal.

Pré-Processamento:
Tratamento de dados;
Engenharia de atributos;
Seleção de features;
Separação treino e teste.

Machine Learning
Foram desenvolvidos modelos preditivos para estimar a quantidade de bicicletas alugadas.

Modelos utilizados:
Linear Regression
Random Forest Regressor

Avaliação dos Modelos:
Os modelos foram avaliados utilizando:

MAE (Mean Absolute Error)
RMSE (Root Mean Squared Error)
R² Score

Principais Insights:
Temperaturas mais altas aumentam a demanda;
Condições climáticas ruins reduzem os alugueis;
Horários de pico possuem maior volume de utilização;
Dias úteis apresentam maior número de usuários registrados;
Existe forte sazonalidade na demanda.

Resultado:
O modelo Random Forest Regressor apresentou melhor desempenho preditivo em relação à Regressão Linear, demonstrando maior capacidade de capturar padrões complexos presentes nos dados.

