
# Sales-Forecasting-TSA
Designing a Time Series forecasting model to assess and predict the pattern of Sales of an online E-commerce website. Involves in-depth data analysis along with exploration and implementation of various important Time Series Analysis (TSA) techniques.

## Models Over view
### SARIMA

SARIMA (Seasonal AutoRegressive Integrated Moving Average) extends the ARIMA model by including seasonal components. It is especially useful for time series data that exhibits repeating patterns over fixed periods (such as monthly or yearly seasonality).

- **Model Components**:
  - AR (AutoRegressive): Uses past values to predict future values.
  - I (Integrated): Applies differencing to remove trends.
  - MA (Moving Average): Uses past forecast errors to make predictions.
  - S (Seasonality): Captures seasonal patterns in the data.

**SARIMA Notation**: 

(p, d, q) x (P, D, Q, m)
where:
- `p, d, q` are the non-seasonal parameters.
- `P, D, Q` are the seasonal parameters.
- `m` is the number of time steps in a seasonal period (e.g., 12 for monthly data).

### Prophet

Prophet, developed by Facebook, is a forecasting tool designed for time series data with daily observations that display seasonality, trend shifts, and holidays. It’s user-friendly, handling missing data and outliers, and it automatically detects change points in the data.

- **Model Components**:
  - Trend: Linear or logistic growth models.
  - Seasonality: Handles multiple seasonalities (e.g., weekly, yearly).
  - Holidays/Events: Models the effect of holidays or events that impact the time series.

**Prophet** uses an additive or multiplicative model structure where trends, seasonality, and holiday effects are combined.

## How to run

1. Data : ``` ecommerce.csv ```
2. Run ```forecasting.ipynb``` for entire workflow from EDA to Model Implementation
