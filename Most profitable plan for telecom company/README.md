# Assessment of the most profitable tariff plan for cellular company
There is the dataset containing data about two tariff plans of cellular company including cellular data, data on SMS and web traffic data.

**Status:** Complete

**Goal**: Assess and define the most profitable tariff plan in terms of revenue and which one should have bigger advertising dollars.

**Stack:** pandas, numpy, matplotlib, seaborn, scipy, math;

**Conclusions:**
- In order **to increase revenue** first **it needs to provide higher advertising budget** to higher revenue generating **Ultra plan** in order to attract more clients, becaues of according to the samples the number of Ultra users is 2 times lower than number of Smart users, second it is probably worth **to think about Ultra plan conditions re-development** in the way of decreasing of plan limitations for number of free minutes and messages to have higher probability of getting additional revenue above the plan;

## Data description

1. Table users (information about users):
    - user_id — user id
    - first_name — user first name
    - last_name — user last name
    - age — age in years
    - reg_date — date of registration
    - churn_date — date of churn (if contains missing value then user used the plan on the moment of data collection)
    - city — user city
    - tariff — user plan
2. Table calls (data about calls):
    - id — call id
    - call_date — call date
    - duration — call duration in minutes
    - user_id — user id
3. Table messages (data about messages):
    - id — message id
    - message_date — message date
    - user_id — user id
4. Table internet (data about web sessions):
    - id — session id
    - mb_used — web traffic used in mb
    - session_date — session date
    - user_id — user id
5. Table tariffs (information about plans):
    - tariff_name — plan name
    - rub_monthly_fee — monthly subscription fee
    - minutes_included — free minutes included in the plan
    - messages_included — free messgaes included in the plan
    - mb_per_month_included — free web traffic amount included in the plan
    - rub_per_minute — price of a minute above free plan in rubles (for example, if plan has 100 free minutes and user spent 101 minutes then user will pay addition fee above the plan)
    - rub_per_message — price of a message above free plan in rubles
    - rub_per_gb — price of a gb above free plan in rubles (1 gb = 1024 mb)
