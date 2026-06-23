# Bike Sharing Demand Prediction

Projeto de Ciência de Dados e Machine Learning para previsão de demanda de bicicletas compartilhadas utilizando dados climáticos e temporais.

---

## Sobre o Projeto

O sistema de bike sharing registra automaticamente cada aluguel — horário, duração e localização. Este projeto utiliza esses dados para **prever a quantidade de bicicletas alugadas por hora**, permitindo que o sistema antecipe a demanda e faça o reposicionamento preventivo de bicicletas nas estações.

**Fonte dos dados:** [Capital Bikeshare System](http://capitalbikeshare.com/system-data) — Washington D.C., EUA (2011–2012)

---

## Objetivo

Desenvolver um modelo preditivo capaz de estimar a demanda horária de bicicletas com base em variáveis climáticas, temporais e de comportamento do usuário.

---

## Dataset

| Arquivo | Descrição | Registros |
|---------|-----------|-----------|
| `day.csv` | Aluguéis agregados por dia | 731 dias |
| `hour.csv` | Aluguéis agregados por hora | 17.379 horas |

**Principais variáveis:**
- `hr` — Hora do dia (0–23)
- `temp` — Temperatura normalizada
- `hum` — Umidade normalizada
- `weathersit` — Condição climática
- `season` — Estação do ano
- `cnt` —  **Target:** total de bicicletas alugadas

---

## Análise Exploratória (EDA)

Principais insights identificados:

- **Horários de pico:** maior demanda às 8h e entre 17h–18h nos dias úteis (deslocamento urbano)
- **Temperatura:** forte correlação positiva com a demanda
- **Clima:** condições severas reduzem drasticamente os aluguéis
- **Sazonalidade:** Outono e Verão concentram maior volume de aluguéis
- **Dias úteis:** maior uso por usuários registrados

---

## Modelos Utilizados

| Modelo | MAE | RMSE | R² |
|--------|-----|------|----|
| Regressão Linear | 104.80 | 139.21 | 0.39 |
| **Random Forest** | **24.90** | **42.07** | **0.94** |

**Melhor modelo: Random Forest** com R² de 0.94, explicando 94% da variância da demanda e erro médio de apenas 24 bicicletas por hora.

---

## Principais Resultados

- O **Random Forest** superou amplamente a Regressão Linear, evidenciando a natureza não-linear dos dados
- A variável **hora do dia (`hr`)** foi a mais importante para o modelo
- Variáveis climáticas como **temperatura** e **umidade** também tiveram alto impacto preditivo
- O modelo é capaz de antecipar picos de demanda com alta precisão, o que pode otimizar a operação do sistema

---

## Tecnologias Utilizadas

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-lightblue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-green)
![Google Colab](https://img.shields.io/badge/Google%20Colab-notebook-yellow)

- **Manipulação de dados:** Pandas, NumPy
- **Visualização:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Ambiente:** Google Colab

---

## Estrutura do Projeto

```
bike-sharing-demand/
│
├── Projeto_1.ipynb     # Notebook principal com todo o desenvolvimento
├── day.csv             # Dataset diário
├── hour.csv            # Dataset horário
└── README.md           # Documentação do projeto
```

---

## Como Executar

1. Acesse o [Google Colab](https://colab.research.google.com)
2. Faça upload do arquivo `Projeto_1.ipynb`
3. Faça upload dos arquivos `day.csv` e `hour.csv` quando solicitado
4. Execute todas as células: **Ambiente de execução → Executar tudo**

---

## Próximos Passos

- [ ] Testar modelos XGBoost e LightGBM
- [ ] Otimização de hiperparâmetros
- [ ] Aplicar split temporal correto para séries temporais
- [ ] Deploy do modelo com Streamlit ou FastAPI

---

## 👩‍💻 Autora

**Cristina Almeida da Silva**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Cristina%20Almeida-blue?logo=linkedin)](https://www.linkedin.com/in/cristina-almeida-da-silva-011603324/)
[![GitHub](https://img.shields.io/badge/GitHub-Cristina--as-black?logo=github)](https://github.com/Cristina-as)




