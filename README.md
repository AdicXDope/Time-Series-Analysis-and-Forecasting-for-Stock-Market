# Time-Series Analysis & Forecasting for Apple (AAPL)

**Author:** AdicXDope  
**GitHub:** https://github.com/AdicXDope

---

## Project Overview

This repository analyzes historical Apple (AAPL) stock prices (2015–2024) and compares multiple time-series forecasting approaches:

- **ARIMA** / **SARIMA** (classical)
- **Prophet** (additive + seasonality)
- **LSTM** (deep learning — univariate and multivariate)

The aim is to evaluate each model on the same hold-out test set and compare using MAE, MAPE and RMSE.

---

## Results (test set metrics)

| Model                                 | MAE       | MAPE (%) | RMSE     |
|--------------------------------------:|:---------:|:--------:|:--------:|
| ARIMA                                | 50.767992 | 25.824747| 55.401633|
| Prophet                              | 29.283033 | 14.485761| 36.274686|
| LSTM (Univariate)                    | 4.290082  | 2.185195 | 5.429949 |
| LSTM (Multivariate - Price Only)     | 10.819635 | 5.340848 | 12.552523|

**Key takeaway:** For this experiment and preprocessing, the univariate LSTM produced the lowest test errors.

---
