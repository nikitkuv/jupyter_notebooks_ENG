# Analysis of video games success patterns
Dataset consist of historical data about games sales, critic and user scores, genres and platforms.

**Status:** Complete

**Goal**: To find relationships and patterns in successfully sellable games. It will allow to count on potentially popular product and plan advertising campaign.

**Stack:** pandas, numpy, matplotlib, seaborn, scipy, math;

**Conclusions:**
- To focus on games of *PS4 and XOne* platforms of *action, shooter, sports and role-playing* genres and of *E and M* ESRB ratings - for all the regions except Japan, and to focus on games of *3DS* platform of *role-playing and action* genres and of T and E ESRB ratings - for Japan;
- Additionally it worths to consider the option with games of *PS3 and X360* platforms for the same genres and ratings for all the refions except Japan, and the option with games of Playstation platforms like *PS3, PSV and PS4* for the same genres and ratings for Japan;

## Data description

- Name — game name
- Platform — platform
- Year_of_Release — game year of release
- Genre — genre
- NA_sales — sales in North America region in millions of copies
- EU_sales — sales in Europe region in millions of copies
- JP_sales — sales in Japan region in millions of copies
- Other_sales — sales in other world in millions of copies
- Critic_Score — critic score (0-100)
- User_Score — user score (0-10)
- Rating — ESRB (Entertainment Software Rating Board) rating of a game
