## Case study: battery revenues on Day-Ahead and Intraday markets

This repository contains the code for a case study on battery optimization.

#### Content
- [input](input) contains the processed input.
- [model](model) contains the optimization model, implemented in Pyomo and largely builty on the [bess-optimizer](https://github.com/FlexPwr/bess-optimizer/) repository.
- [1_make_dataset.iypnb](1_make_dataset.iypnb) processes the original input in `raw_input/` (private folder) into a training and a forecasting dataset.
- [2_forecast_revenues.ipynb](2_forecast_revenues.ipynb): here, annualized revenues are forecasted using a tree-based regression model (XGBoost).
- [3_optimization_model.ipynb](3_optimization_model.ipynb): the optimization model is used to compute daily hurdle rates from historical and predicted day-ahead / intraday prices.