# GARCH Volatility Modeling

This project studies volatility dynamics for four major equity indices:

- `^GSPC`: S&P 500
- `^STOXX50E`: EURO STOXX 50
- `^N225`: Nikkei 225
- `^FTSE`: FTSE 100

The main notebook is [notebooks/Garch_Model.ipynb](notebooks/Garch_Model.ipynb). It:

- downloads adjusted close prices from Yahoo Finance
- computes log returns
- checks stationarity with the ADF test
- explores price, return, rolling-volatility, and distribution patterns
- fits GARCH(1,1) models under normal and Student-t distributions
- evaluates recursive one-step-ahead volatility forecasts from 2022 onward

## Structure

```text
garch_project/
|-- data/
|-- notebooks/
|-- outputs/
|-- src/
|-- README.md
|-- requirements.txt
```

## Outputs

When the notebook is rerun, it writes figures and tables to `outputs/`, including:

- `price_plot.png`
- `log_return_plot.png`
- `rolling_volatility_plot.png`
- `rolling_volatility_series.csv`
- `rolling_volatility_correlation.csv`
- `return_distribution.png`
- `garch_normal_parameters.csv`
- `residuals_plot.png`
- `standardized_residuals_plot.png`
- `acf_standardized_residuals_<index>.png`
- `garch_student_t_parameters.csv`
- `garch_model_comparison.csv`
- `recursive_forecast_<index>.csv`
- `forecast_summary.csv`
- `recursive_one_step_ahead_volatility_forecasts.png`

## Notes

- The notebook assumes it is run from `garch_project/notebooks/`, so exports are written to `../outputs/`.
- Recursive forecast outputs are saved per index to make later report writing easier.
