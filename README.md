# 📊 Previsão de Consumo Energético com Modelos de Machine Learning

Este repositório corresponde ao projeto final da Licenciatura em Engenharia Informática (ESTG | P.PORTO).

Este projeto tem como objetivo prever o **consumo energético horário** com base em séries temporais e variáveis exógenas, utilizando algoritmos de Machine Learning tradicionais e modelos especializados em séries temporais.

---

## 🧠 Tecnologias e Bibliotecas

- Python 3.10+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- statsmodels
- autogluon.timeseries
- holidays
- joblib

---

## 🗂️ Estrutura do Projeto

```
datasets/
    consumo_eredes_normalizado_4610.parquet
    ...
figuras/
    boxplot-consumo-energetico.png
    ...
notebooks/
    1recolha-e-limpeza.ipynb
    2preprocessamento-dos-dados.ipynb
    ...
predicts/
    ARIMA/
    ARIMA_lag/
    AutoML/
    AutoML_lag/
    ...
```

---

## 📈 Dataset

Os dados foram obtidos da [e-Redes](https://e-redes.opendatasoft.com/pages/homepage/), referentes ao código postal **4610**, com granularidade **horária**, entre **2022-11-01 e 2023-09-30**.

Principais variáveis utilizadas:
- `EnergyNormalized` (target)
- `Hour`, `TimeOfDay`, `DayOfTheWeek` (temporais)
- `Temperature` (meteorológica)
- `PopulationDensity` (estática)
- `lag_168` (lags do target)

---

## ⚙️ Modelos Treinados (sem lag e com lag)

### Baseline
- ARIMA

### Machine Learning
- Random Forest
- XGBoost
- Extra Trees
- AutoML

### Deep Learning
- LSTM
- CNN
- NARX

---

## 📌 Como Executar

1. Clonar o repositório:
```bash
git clone https://github.com/heyliceeee/previsao-do-consumo-energetico-com-ml.git
cd previsao-do-consumo-energetico-com-ml
```

2. Executar os notebooks disponíveis em `notebooks/` por ordem crescente:
```text
1recolha-e-limpeza.ipynb
2preprocessamento-dos-dados.ipynb
...
```

---

## 🤝 Autora

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/heyliceeee">
        <img src="https://github.com/heyliceeee.png" width="100px;" alt="Foto da Alice Dias no GitHub"/><br>
        <sub><b>Maria Alice Dias</b></sub>
      </a>
    </td>
  </tr>
</table>

---

## 🏫 Instituição

📍 Instituto Politécnico do Porto - Escola Superior de Tecnologia e Gestão <br/>
📅 2024/2025  
👩‍🏫 Projeto Final – Licenciatura em Engenharia Informática