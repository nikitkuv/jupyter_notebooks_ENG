# Assessment of the most profitable tariff plan for cellular company
There is the dataset containing data about two tariff plans of cellular company including cellular data, data on SMS and web traffic data.

**Status:** Complete

**Goal**: Assess and define the most profitable tariff plan in terms of revenue and which one should have bigger advertising dollars.

**Stack:** pandas, numpy, matplotlib, seaborn, datetime;

**Conclusions:**
Key pricing factors:
    - Total area and number of rooms, which is dependent on total area;
    - Distance to city center for big cities: the price is significantly higher within first 9 km from Saint-Petersburg center, outside this mark there is no relationship between the price and the distance form city center;
    - Floor category: first floor flats are cheaper, and everywhere except Saint-Petersburg last floor flats are also cheaper than others excluding first floor flats;
    - There is no relationships between weekday and month of date of offer publication, but we can extract some trends analysing data based on years of publication: since 2016 there is a trend in increasing of the price;
    - As expected the most expensive flats are in Saint-Petersburg with a high margin from other localities, the second place is Pushkin. The cheapest flats are in Vyborg;

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
