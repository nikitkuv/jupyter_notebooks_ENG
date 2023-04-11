# Telecom customer churn prediction
Data on customers, their plans and contracts.

**Status:** Completed 

**Goal**: train a model to predict customer churn in telecom company.

**Stack:** imblearn, sklearn, lightgbm, pandas, numpy, matplotlib, seaborn;

**Conclusions:**
- According to data analysis there are two possible reasons for customers to churn:
    1. High charges. Most of the customers churn right after starting using company's service because of high charges as a result of not fully understanding the terms of the contract or just because of it is too expensive and there are more cheap relativly the same plans in the competitors
    2. Uncareful attention and poorly organized communication to the new customers. Majority of the customers churn because of poor service quality
- According to modeling results, the key features are continuous features related to charges bot total and monthly
- From categorical features we can highlight presense of fiber connection, contract term, diversity of available services like online security, technical support, internet service, availability of digital reciepts
- The best models are LGBM default and smote ones having **ROC AUC = 0.91** and **Accuracy = 0.86**

## Data description

Data consist of the following files obtained from different sources:

- `contract.csv` — contract information;
- `personal.csv` — customer information;
- `internet.csv` — information about plans of customers;
- `phone.csv` — information about telephony and phone plans.
