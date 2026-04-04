# Midterm Project: Titanic Survival Analysis

## 📖 The "So What?": The Problem
The sinking of the Titanic is one of the most infamous maritime disasters in history. The goal of this project wasn't just to predict survival, but to tell the story of the **social and systemic factors** that determined who lived and who died. 

*   **The Goal:** To build a classification model that predicts passenger survival based on features like age, gender, and socio-economic status (class).
*   **The Audience:** Historians and Data Scientists interested in social stratification.
*   **The Data:** The RAW data from raw.githubusercontent.com, containing 891 passenger records.

## 🛠 The Journey: My Approach
I gave it a "Detective" approach to clean up historical records:
1. **Data Cleaning:** I handled missing values in the 'Age' column by using the median age and dropped the 'Cabin' column due to excessive missing data.
2. **Feature Engineering:** I converted categorical data (Sex and Embarked) into numerical values using One-Hot Encoding so the model could process them.
3. **The Algorithm:** I used a **[Random Forest Classifier]**. I chose this because it prevents "overfiting" (where a model memorized the data too closely) and provides a more realiable story of passenger survival.

## 📊 The Revelation: Results & Insights
My analysis revealed a clear narrative of "Women and Children First," but with a heavy class bias:
*   **Key Insight 1:** Gender was the strongest predictor. Females had a significantly higher survival rate than males across all classes.
*   **Key Insight 2:** Socio-economic status was a "life-raft." Passengers in 1st Class were nearly 3x more likely to survive than those in 3rd Class.
*   **Model Performance:** My model achieved an **Accuracy of [81.01%]**, meaning it correctly predicted whether a passensger survived or perished based on historical data.

## 🎓 Reflection & Challenges
*   **What I Learned:** I learned how to properly handle raw data (eg. label encoding, one-hot encoding) and the use of classifiers (eg. Logistic Regression, Random Forest) to predict the survival rate of passenger for the Titanic dataset.
*   **The Roadblock:** Dealing with the missing 'Age' data was tricky. I initially thought about deleting those rows, but I realized that would lose too much valuable "story" from the dataset, so I chose to fill them (impute) instead.
