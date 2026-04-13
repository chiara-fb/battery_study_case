## Case study: battery revenues on Day-Ahead and Intraday markets

This repository contains the code for a case study on battery optimization.

#### Content

- [model](model) contains the optimization model, implemented in Pyomo and largely builty on the [bess-optimizer](https://github.com/FlexPwr/bess-optimizer/) repository.
- [raw_input](raw_input) contains the original input for the case study.
- [input](input) contains the input as processed in [1_make_dataset.iypnb](1_make_dataset.iypnb).
- [2_forecast_revenues.ipynb](2_forecast_revenues.ipynb): here, annualized revenues are forecasted using a tree-based regression model (XGBoost).
- [3_optimization_model.ipynb](3_optimization_model.ipynb): the optimization model is used to compute daily hurdle rates from historical and predicted day-ahead / intraday prices.