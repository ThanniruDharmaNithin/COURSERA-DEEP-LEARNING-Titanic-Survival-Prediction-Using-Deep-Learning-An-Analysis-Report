# 🚢 Titanic Survival Prediction Using Deep Learning

**Course:** Coursera – Deep Learning  
**Submitted by:** THANNIRU DHARMA NITHIN  

---

## 🎯 Objective
The objective of this analysis is to predict the survival of passengers on the Titanic using Deep Learning algorithms. The study explores which features most significantly influenced survival rates, helping historians, researchers, and analysts understand factors contributing to survival. These insights can also inform better safety protocols and passenger management strategies in similar scenarios.

---

## 📊 Dataset Overview
The Titanic dataset contains passenger information, including demographics, ticket class, family connections, and boarding details. Key features include:

- **PassengerId:** Unique ID of the passenger  
- **Survived:** Survival status (0 = No, 1 = Yes)  
- **Pclass:** Ticket class (1st, 2nd, 3rd)  
- **Name:** Passenger name  
- **Sex:** Gender  
- **Age:** Passenger age  
- **SibSp:** Number of siblings/spouses aboard  
- **Parch:** Number of parents/children aboard  
- **Ticket:** Ticket number  
- **Fare:** Passenger fare  
- **Cabin:** Cabin number  
- **Embarked:** Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)  

The goal is to build a predictive model for the `Survived` attribute based on these features.

---

## 🧐 Data Exploration & Preprocessing
Initial exploration revealed missing values and categorical features that required encoding. Key preprocessing steps included:

1. **Handling Missing Values:** Dropping rows with missing `Age` or `Embarked`.  
2. **Encoding Categorical Variables:**  
   - `Sex` converted to numeric (female = 1, male = 0)  
   - `Embarked` one-hot encoded  
3. **Dropping Irrelevant Columns:** Removed `Name`, `Ticket`, `Cabin`, and original `Embarked`.  
4. **Feature Scaling:** Standardization of numerical features for model training.  

These steps ensured clean, structured data for effective deep learning modeling.

---

## 🧠 Model Architecture
A neural network was designed with multiple variations to predict survival:

- **Model 1 (Recommended):** Two hidden layers, 64 neurons each, ReLU activation, 50% dropout  
- **Model 2:** Three hidden layers, 128 neurons each, ReLU activation, 50% dropout  
- **Model 3:** Two hidden layers, 64 neurons each, ReLU activation, 30% dropout  

Model 1 was selected for its balance between simplicity, training time, and interpretability.

---

## 📌 Key Findings
1. **Training Issues:** All models experienced NaN values in the loss function, indicating preprocessing or configuration challenges.  
2. **Low Accuracy:** Model 1 achieved a test accuracy of 44.89%, which is below the random baseline of 50%.  
3. **Feature Insights:** Passenger class, age, and gender were significant factors in survival.  
4. **Challenges Identified:** Missing data, insufficient feature engineering, and model hyperparameters need improvement.  

---

## 💡 Next Steps & Recommendations
To improve model performance and reliability:

- Investigate NaN values in loss function and correct preprocessing issues.  
- Perform advanced feature engineering to extract more informative variables.  
- Tune model hyperparameters (neurons, layers, learning rate, dropout).  
- Explore data augmentation or cross-validation to enhance robustness.  
- Consider alternative deep learning architectures (e.g., LSTM, ensemble models) for better predictive performance.  

---

## 🏆 Conclusion
While the deep learning models achieved limited accuracy, this project demonstrates the process of applying neural networks to structured tabular data for predictive analysis. The insights gained on features affecting survival provide valuable understanding of historical passenger data and lay a strong foundation for future improvements in predictive modeling.  

This project highlights the challenges of real-world data, the importance of preprocessing, and the potential of deep learning to inform decision-making in structured datasets.

---
