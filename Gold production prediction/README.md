# Gold recovery prediction
The dataset contains data about parameters of production and cleaning of gold ore from the company that develops solutions for efficient work of industrial plants.

**Status:** Completed

**Goal**: prepare a prototype of machine learning model that predicts gold recovery coefficient from gold ore

**Stack:** sklearn, lightgbm, pandas, numpy, matplotlib, seaborn;

**Conclusions:**
- According to the conducted anaylsis we can conclude that the main task of the proccess, which is gold recovery from the ore, completes successfully
- But we can increase efficiency of silver and lead enrichment processes to make additional profit
- Trhee models showed good results for prediction of gold recovery coeeficient in rougher and final concentrates, the best one is **Lasso regression**

## Data description

Technical process:
   - Rougher feed — rougher feed
   - Rougher additions (or reagent additions) — flotation agents: Xanthate, Sulphate, Depressant
   - Xanthate — xanthate (promoter, or flotation activator);
   - Sulphate — sulphate (here sodium sulphate);
   - Depressant — depressant (sodium silicate).
   - Rougher process — flotation
   - Rougher tails — rougher tails
   - Float banks — float banks
   - Cleaner process — cleaner process
   - Rougher Au — rougher Au concentrate
   - Final Au — final Au concentrate

Stage parameters:
   - air amount — volume of air
   - fluid levels — fluid levels
   - feed size — feed size
   - feed rate — feed rate

Features nomenclature:
 - Feature name must be this way: *stage.parameter_type.parameter_name*
 - Exapmle: rougher.input.feed_ag

Values for *stage* part:
   - rougher — flotation
   - primary_cleaner — primary cleaner
   - secondary_cleaner — secondary cleaner
   - final — final characteristics

Values for *parameter_type* part:
   - input — feed parameters
   - output — product parameters
   - state — current parameters of the stage
   - calculation — calclulation characteristics
