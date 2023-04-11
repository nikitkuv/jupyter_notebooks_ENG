# Car price prediction
Dataset contains historical data on car sales: technical parameters and prices.

**Status:** Completed

**Goal**: create a model to predict car price based on its characteristics.

**Stack:** sklearn, pandas, numpy, matplotlib, seaborn;

**Conclusions:**

- Despite of the worst result in training-prediction time the final chosen model is **LightGBM** because of much better quality of predictions compared to all the other used models
- To reduce training-prediction time we can continue to tune hyperparameters and model's quality will not be affected much

## Data description

  - DateCrawled — date the form (row) was collected
  - VehicleType — vehicale type
  - RegistrationYear — year of car registration
  - Gearbox — type of gearbox
  - Power — power in horse power
  - Model — car model
  - Kilometer — run in km
  - RegistrationMonth — month of car registration
  - FuelType — type of fuel
  - Brand — car brand
  - NotRepaired — whether the car was repaired or not
  - DateCreated — date the form (row) was created
  - NumberOfPictures number of car pictures in the form
  - PostalCode — postal code of car owner 
  - LastSeen — date of owner last activity
  - Price — price in euros
