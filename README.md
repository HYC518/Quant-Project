# Quant Project

This repository collects my quantitative finance projects, including factor modeling, return analysis, and volatility modeling.

## Projects

- [Rolling CAPM Analysis](capm_project/notebooks/capm_analysis.ipynb)
  Estimates rolling alpha, beta, and R-squared for 10 large-cap U.S. stocks across sectors using a 126-trading-day window.

- [GARCH Volatility Modeling](Garch_project/notebooks/Garch_Model.ipynb)
  Fits GARCH(1,1) models to major global equity indices, compares normal and Student-t specifications, and evaluates recursive one-step-ahead volatility forecasts.

## Project Files

- [CAPM notebook](capm_project/notebooks/capm_analysis.ipynb)
- [Processed dataset](capm_project/data/capm_data.csv)
- [Rolling regression output](capm_project/outputs/roll_results.csv)
- [Python requirements](capm_project/requirements.txt)
- [GARCH notebook](Garch_project/notebooks/Garch_Model.ipynb)
- [GARCH project README](Garch_project/README.md)
- [GARCH requirements](Garch_project/requirements.txt)

## Notes

- Each project keeps its own notebook, data, and outputs under its project folder.
- The GARCH notebook exports figures and tables to `Garch_project/outputs/` when rerun.
