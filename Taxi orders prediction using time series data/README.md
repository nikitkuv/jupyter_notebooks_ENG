# Taxi orders prediction

Dataset contains historical data on taxi orders in airports. We need to predict number of taxi orders for the following hour to attract more drivers in the time of the highest demand.

**Status:** Completed

**Goal:** make model to predict number of taxi orders for the following hour. 

**Stack:** statsmodels, sklearn, lightgbm, itertools, pandas, numpy, matplotlib, seaborn;

**Conclusions:**

- All the models show results better than customer claimed
- The best result is shown by LightGBM Regressor model based on metric values

## Data description

`num_orders` column contains number of orders.
