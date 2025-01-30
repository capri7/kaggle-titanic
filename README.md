## Project Overview
以下の部分がこのコンペの概要です。以下はkaggleの文章をそのままコピペしています。なので編集が必要です。

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).
ここまでがkaggleのコピーです。

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

- [LightGBM details](notebook/EDA.ipynb)
  それぞれのプロットについて詳しく説明を入れています。
  
1.Survived rate
Died    61.62 %
Survived    38.39%

2. Insights from Survival and Death Rates by Embarkation Port
Cherbourg:
Passengers embarking from Cherbourg have the highest survival rate compared to other ports.
The survival rate is nearly equal to the death rate, indicating a relatively balanced outcome.
Queenstown:
Passengers from Queenstown have a higher death rate compared to their survival rate.
This suggests that passengers from this port may have had fewer chances of survival.
Southampton:
Passengers from Southampton experienced the highest death rate among the three ports.
The survival rate is significantly lower, making this port a notable point of interest for further investigation.


3.Age Distribution of Survivors and Deaths

4.Investigate the relationship between survival rate and Gender

5.Age Distribution by Gender and Survival Status

6. Investigate the relationship between survival rate and family size
7.Investigate the relationship between survival rate and pclass by gender
8.Investigate the relationship between age and pclass



#### Key Observations:
Passenger Distribution: Pclass 3 passengers accounted for more than half (55.1%) of the total, suggesting a reliance on lower-class passengers for revenue. On its maiden voyage, only 1,317 passengers boarded, just 53% of the ship’s capacity, while the crew count remained at 907.

Fare Analysis: The average fare for Pclass 1 was more than six times higher than Pclass 3, highlighting a stark economic divide between passenger classes.

Lifeboat Shortage: While outdated maritime safety regulations are the primary reason for insufficient lifeboats, financial constraints might have played a role. For example, prioritizing cargo over additional lifeboats could have been seen as a cost-saving measure.

These observations suggest that the Titanic operated under significant financial and operational pressures, balancing luxury, revenue, and safety—an imbalance that tragically contributed to the disaster.






# Titanic - Machine Learning from Disaster

## 🚢 Project Overview
This project predicts Titanic passenger survival using machine learning models. The dataset, sourced from Kaggle, includes passenger details such as age, gender, class, and fare. The challenge is to identify factors influencing survival and build a predictive model.

---

## 📊 Model Performance
The most effective models and their validation accuracies are summarized below:

| Model             | Accuracy  | 
|-------------------|-----------|
| **Random Forest** | **79.42%** |
| Ensemble          | 78.23%    |
| Gradient Boosting | 78.73%    |
| LightGBM          | 77.99%    |
| SVC               | 77.51%    |
| Stacking          | 77.51%    |
| CatBoost          | 77.27%    |
| XGBoost           | 76.79%    |

---

## 🔍 Key Insights from EDA
- **Survival Rate**: 38.39% of passengers survived, while 61.62% perished.
- **Embarkation Port**:
  - **Cherbourg**: Highest survival rate among ports.
  - **Queenstown**: Higher death rate compared to survival rate.
  - **Southampton**: Highest death rate among all ports.
- **Age**: Younger passengers had a higher chance of survival.
- **Gender**: Women (81.1% survival) were significantly more likely to survive than men (25.8% survival).
- **Family Size**: Both very small and very large family sizes had lower survival rates.
- **Passenger Class**: First-class passengers had higher survival rates, especially women.

---

## 📂 EDA Notebook
Explore the detailed exploratory data analysis and visualizations:
[EDA Notebook](notebook/EDA.ipynb)

---

## 🌟 Additional Observations
- **Passenger Class Distribution**: 55.1% of passengers were from 3rd class, indicating reliance on lower-class passengers for revenue.
- **Fare Disparity**: First-class fares were six times higher than third-class, showcasing the economic divide.
- **Operational Constraints**: Lifeboat shortages, financial pressures, and safety regulations contributed significantly to the disaster.

---

This README is now concise and impactful, with a focus on essential details and results. Let me know if you'd like any further tweaks! 🚀

