# Titanic - Machine Learning from Disaster

## 🚢 Project Overview
This project focuses on predicting Titanic passenger survival using machine learning models. The dataset, sourced from Kaggle, includes passenger details such as age, gender, class, and fare. The challenge is to identify key factors influencing survival and develop a predictive model.


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
  - **Cherbourg**: Highest survival rate among the ports, likely due to the higher proportion of first- and second-class passengers.
  - **Queenstown**: Higher death rate compared to survival rate, as most passengers boarding here were third-class.
  - **Southampton**: Highest death rate among all ports, as the majority of passengers boarded at this location.
- **Age**: Younger passengers had a significantly higher chance of survival. 
  - **Children (0–10 years old)**: Over 55% survived, demonstrating a priority for saving children.
  - **Young adults (20–30 years old)**: Survival rates dropped significantly, with only around 30–40% surviving.
  - **Elderly passengers (60+ years old)**: Survival rates were the lowest, with less than 20% surviving.
- **Gender**: Women (81.1% survival) were significantly more likely to survive than men (25.8% survival).
- **Family Size**: Survival rates varied significantly based on family size.
  - **Solo passengers (FamilySize = 1)**: Had the highest mortality rate, with **over 60% not surviving**.
  - **Small families (FamilySize = 2–4)**: Achieved the highest survival rates, with **50–60% surviving**.
  - **Large families (FamilySize = 5 or more)**: Experienced significantly lower survival rates, with **less than 30% surviving**.
- **Passenger Class**: Survival rates varied significantly by passenger class. 
  - **First-Class Passengers**: Enjoyed the highest survival rates, especially women, with nearly all first-class women surviving.
  - **Second-Class Passengers**: Also showed high survival rates for women, though slightly lower than first-class.
  - **Third-Class Passengers**: Both men and women faced the highest mortality rates. Women in third class had a survival rate of approximately 50%, which significantly lowered the overall survival rate for women.


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



# Titanic - Machine Learning from Disaster

## 🚢 Project Overview
This project focuses on predicting Titanic passenger survival using machine learning models. The dataset, sourced from Kaggle, includes passenger details such as age, gender, class, and fare. Using advanced machine learning techniques, I identified key factors influencing survival and developed predictive models with competitive accuracy.

---

## 📊 Model Performance
The most effective models and their validation accuracies are summarized below. The Random Forest model achieved the best accuracy, outperforming other algorithms due to its ability to handle feature interactions effectively.

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
### **Overall Survival Trends**
- **Survival Rate**: 38.39% of passengers survived, while 61.62% perished.
- **Gender**: Women (81.1% survival) were significantly more likely to survive than men (25.8% survival).
- **Age**: Younger passengers had higher survival rates:
  - **Children (0–10 years old)**: Over 55% survived.
  - **Young adults (20–30 years old)**: Survival rates dropped to around 30–40%.
  - **Elderly passengers (60+ years old)**: Less than 20% survived.

### **Port and Class**
- **Embarkation Port**:
  - **Cherbourg**: Highest survival rate due to more first- and second-class passengers.
  - **Queenstown**: High death rate, dominated by third-class passengers.
  - **Southampton**: Largest group of passengers with the highest death rate.
- **Passenger Class**:
  - **First-Class Passengers**: Nearly all women survived.
  - **Second-Class Passengers**: High survival rate for women.
  - **Third-Class Passengers**: Lowest survival rate for both men and women.

### **Family Size**
- **Solo passengers (FamilySize = 1)**: Over 60% did not survive.
- **Small families (FamilySize = 2–4)**: Highest survival rates (50–60%).
- **Large families (FamilySize = 5 or more)**: Survival rates dropped below 30%.

---

## 📂 EDA Notebook
Explore the [EDA Notebook](notebook/EDA.ipynb) for detailed analyses, including survival trends by age, gender, class, and family size, along with visualizations and actionable insights.

---

## 🌟 Additional Observations
- **Passenger Class Distribution**: 55.1% of passengers were in 3rd class, highlighting the Titanic's reliance on lower-class passengers for revenue.
- **Fare Disparity**: First-class fares were six times higher than third-class, reflecting significant economic divides among passengers.
- **Operational Challenges**: Lifeboat shortages, financial priorities, and outdated safety regulations significantly influenced the disaster's scale.

---



