# Telecom plan classification
Data is from retail chain of hypermarkets containing information about clients, products range, hypermarkets and client transactions made in those hypermarkets.

**Status:** Completed

**Goal**: define methodology to predict cutomer churn in non-contractual setting and create a probabilistic model using defined methodology.

**Stack:** sklearn, pandas, numpy, matplotlib, seaborn;

**Conclusions:**
- Two different approaches were applied to solve the original task of customer churn prediction in non-contractual setting: BG/NBD model and classic machine learning algorithms with and without using of some results of BG/NBD.
- During RFT feature analysis there were some interesting insights like the fact that the last 8 months of the data there were no customer inflow at all even though high loyalty of the old customers was observed from the data. We recommend to improve marketing program in order to attract new customers and increase their auditory.
- Classic machine learning algorithms with RFM features show near ideal performance, which probably because of data leakage since the target variable was calculated based on the probabilities which in turn were generated from those RFM features.
- Classic machine learning algorithms without RFM features are a bit worser but in general the results are relatively good especially when it comes to the models that use features created from transaction dates.
- BG/NBD model has some advantages over classic machine learning algorithms in such a task:
    - Requires less data: just data on customer transactions with their ids, dates of transactions and total sum of purchases on the transactions.
    - Since it requires less data it also need to make less cleaning and postprocessing so data remains less altered.
    - It is fater to train and to make it ready for training.
    - Allows us to calculate probabilities of a client to be alive directly from the original data, we don't need to create target variable, which is very complex process in non-contractual settings of customer churn prediction tasks.
    - Gives us tools for deeper analysis of customer behavior patterns.
- Despite of those facts, classic machine learning algorimths showed their streingth as well so we recommend to use BG/NBD model in combination with pre-trainde classic algorithms models.

## Data description

Data is stored in the following file-tables:

- `transactions.parquet` — transaction data;
    - chq_id - ID of transaction
    - plant - ID of store
    - chq_date - Date of transaction
    - chq_position - Position of material in transaction
    - client_id - ID of client
    - material - ID of material (item)
    - sales_count - Count of item in the check position
    - sales_sum - Amount in rubles by the check position
    - is_promo - Fact of selling the position of the check for promo
    
- `clients.csv` — directory of clients;
    - client_id - ID of client
    - gender - Gender of client
    - city - City where the client makes the most purchases
    - birthyear - Year of birth
    
- `materials.csv` — directory of products;
    - material - ID of material (item)
    - hier_level_1 - 1st level of items hierarchy
    - hier_level_2 - 2nd level of items hierarchy
    - hier_level_3 - 3rd level of items hierarchy
    - hier_level_4 - 4th level of items hierarchy
    - vendor - Vendor of item
    - is_private_label - Own brand mark
    - is_alco - Sign of alcoholic beverages
    
- `plants.csv` — directory of hypermarkets;
    - plant - ID of store
    - plant_type - Type of store (HM - hypermarket, SM - supermarket)
    - city - City where the store located
