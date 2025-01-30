## Project Overview
以下の部分がこのコンペの概要です。以下はkaggleの文章をそのままコピペしています。なので編集が必要です。

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).

# Model Performance

This project focuses on predicting Titanic passenger survival using machine learning models. 
The most effective model was **Random Forest**, achieving an accuracy of 86.59% on the validation set.

## Key Results
| Model            | Accuracy | 
|------------------|----------|
| Random Forest    | 79.42%   | 
| Ensembele        | 78.23%   | 
| Gradient Boost   | 78.73%   | 
| LightGBM         | 77.99%   | 
| SVC              | 77.51%   | 
| Stacking         | 77.51%   | 
| CatBoost         | 77.27%   | 
| XGBoost          | 76.79%   | 


## Insight FROM EDA
- [LightGBM details](models/lightgbm/evaluation.md)

The Titanic is widely known as a luxury ocean liner; however, when analyzing the passenger class distribution and ticket fares, a different narrative emerges.

#### Key Observations:
Passenger Distribution: Pclass 3 passengers accounted for more than half (55.1%) of the total, suggesting a reliance on lower-class passengers for revenue. On its maiden voyage, only 1,317 passengers boarded, just 53% of the ship’s capacity, while the crew count remained at 907.

Fare Analysis: The average fare for Pclass 1 was more than six times higher than Pclass 3, highlighting a stark economic divide between passenger classes.

Lifeboat Shortage: While outdated maritime safety regulations are the primary reason for insufficient lifeboats, financial constraints might have played a role. For example, prioritizing cargo over additional lifeboats could have been seen as a cost-saving measure.

These observations suggest that the Titanic operated under significant financial and operational pressures, balancing luxury, revenue, and safety—an imbalance that tragically contributed to the disaster.



