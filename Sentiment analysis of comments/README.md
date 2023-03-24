# Sentiment analysis of comments
Dataset contains comments on various products from e-shop with sentiment label

**Status:** Completed

**Goal**: Build a model to classify comments as positive or negative.

**Stack:** nltk, re, sklearn, imblearn, lightgbm, itertools, pandas, numpy, matplotlib, seaborn, tqdm;

**Conclusions:**
- LogisticRegression using class weights showed the best f1 metric values
- Beside that model, another LogisticRegression model using SMOTE showed result higher than 0.75 as claimed

## Data description
*Text* column contains comment text, *toxic* — target variable representing binary variable where 1 means negative and 0 means positive.
