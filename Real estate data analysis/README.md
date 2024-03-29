# Real estate data analysis
We have Saint-Petersburg, Russia and surrounding area real estate dataset.

**Status:** Completed

**Goal**: explore parameters, which define market price of real estate property.
Each property has two types of data: first one - recieved from user who posted an offer for sale, second - cartographic data about property.

**Stack:** pandas, numpy, matplotlib, seaborn, datetime;

**Conclusions:**
Key pricing factors:
    - Total area and number of rooms, which is dependent on total area;
    - Distance to city center for big cities: the price is significantly higher within first 9 km from Saint-Petersburg center, outside this mark there is no relationship between the price and the distance form city center;
    - Floor category: first floor flats are cheaper, and everywhere except Saint-Petersburg last floor flats are also cheaper than others excluding first floor flats;
    - There is no relationships between weekday and month of date of offer publication, but we can extract some trends analysing data based on years of publication: since 2016 there is a trend in increasing of the price;
    - As expected the most expensive flats are in Saint-Petersburg with a high margin from other localities, the second place is Pushkin. The cheapest flats are in Vyborg;

## Data description

- airports_nearest — distance to the nearest airport (m)
- balcony — number of balconies
- ceiling_height — ceiling height (m)
- cityCenters_nearest — distance to city center (m)
- days_exposition — number of days an offer for sale was posted (from date of posting till withdrawal)
- first_day_exposition — posting date
- floor — floor
- floors_total — number of floors in the building
- is_apartment — apartments (boolean)
- kitchen_area — kitchen area (m²)
- last_price — property price at time of offer withdrawal (rubles)
- living_area — living area (m²)
- locality_name — locality name
- open_plan — open plan (boolean)
- parks_around3000 — number of parks in 3 km
- parks_nearest — distance to the nearest park (m)
- ponds_around3000 — number of ponds in 3 km
- ponds_nearest — distance to the nearest pond (m)
- rooms — number of rooms
- studio — studio (boolean)
- total_area — total area (m²)
- total_images — total number of property images
