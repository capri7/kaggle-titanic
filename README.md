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
  - **Elderly Passengers (60+ years old)**: Survival rates varied greatly by gender.
  - **Women (60+ years old):** All survived.
  - **Men (60+ years old):** Very low survival rates, likely under 20%.


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



