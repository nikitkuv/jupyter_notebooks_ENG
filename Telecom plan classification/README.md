# Telecom plan classification
Dataset contains data on telecom company customer behavior who used two new tariff plans - Ultra and Smart plans. Company has made a research that many customers still use archive tariff plans.

**Status:** Completed

**Goal**: build a model which is able to analyse historical customer behavior and recommend a new plan to new customers.

**Stack:** sklearn, pandas, numpy, matplotlib, seaborn;

**Conclusions:**
- The final model is **RandomForestClassifier, having accuracy on test set = 0.8**

## Data description

 - сalls — number of calls
 - minutes — total minutes spent on calls
 - messages — number of sms messages
 - mb_used — internet traffic used in Mb
 - is_ultra — tariff plan used («Ultra» — 1, «Smart» — 0)
