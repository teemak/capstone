### New Haven County Real Estate Market
---
#### Executive summary
Understanding the dynamics of the real estate market is crucial, especially considering its susceptibility to various economic factors. This study hypothesizes that interest rates play a significant role in determining housing prices.
#### Rationale
Real estate stands as a pivotal investment for many, often necessitating financial support through loans. Despite being perceived as an investment opportunity, its pricing is subject to multifaceted influences. Hence, a comprehensive grasp of market trends is imperative for making informed financial decisions.
#### Research Question
Analyzing market trends is essential for discerning patterns. This study aims to identify the primary drivers of price fluctuations and predict future market movements. Additionally, it explores potential investment avenues within the real estate market.
#### Data Sources
| Description | Source |
|------------ | ------ |
| Mortgage Interest Rates | https://fred.stlouisfed.org/series/MORTGAGE30US |
| Consumer Price Index | https://fred.stlouisfed.org/series/CPIAUCSL |
| Rental Vacancy Rates | https://fred.stlouisfed.org/series/RRVRUSQ156N |
| US Condo Median Sale Price | https://www.zillow.com/research/data |
| Zillow Home Value Index | https://www.zillow.com/research/data |
| Unemployment Rate | https://beta.bls.gov/dataViewer/view/timeseries/EIUIR4 |
#### Methodology
The target variable is the binary outcome of whether the sale price of a property increases. Machine learning techniques are utilized to enhance prediction accuracy by incorporating relevant features. Scikit-learn's permutation importance method identified "adj_price" as the most significant contributing factor.
#### Results
The baseline model demonstrated an accuracy of 65%, which improved to 74% after incorporating feature engineering. Notably, "adj_price" emerged as the most influential parameter, underscoring its significance in predicting market movements. The Naive Bayes model had an accuracy of 80%. Support Vector Machines had performed the best so far with a 81% accuracy. The neural network's highest accuracy was 99%. I don't think that is the true score there is probably overfitting.
#### Next steps
While "adj_price" holds substantial predictive power, its nature as a lagging indicator necessitates the inclusion of additional features. Future iterations of the model will focus on integrating more comprehensive datasets to enhance predictive capabilities.
#### Outline of project
- [New Haven Real Estate Market Direction](https://github.com/teemak/capstone/blob/main/1.%20Exploratory%20Data%20Analysis.ipynb)
