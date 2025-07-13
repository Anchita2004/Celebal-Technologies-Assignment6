# 🍷 Wine Quality Classification with Machine Learning

This project applies multiple machine learning models to predict the quality of red wine using physicochemical properties. The goal is to classify wine as **Good (quality ≥ 7)** or **Bad (quality < 7)** and compare model performances using common evaluation metrics and hyperparameter tuning.

---

## 📁 Dataset

- Source: [Wine Quality Dataset - Kaggle](https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009)
- File used: `winequality-red.csv`
- Attributes: 11 physicochemical features + 1 quality score

---

## 📊 Project Workflow

1. **Data Preprocessing**
   - Load dataset
   - Convert quality to binary classification (Good/Bad)
   - Feature scaling

2. **Model Training**
   - Logistic Regression
   - Decision Tree
   - Random Forest
   - Support Vector Machine (SVM)
   - K-Nearest Neighbors (KNN)

3. **Model Evaluation**
   - Metrics used: **Accuracy**, **Precision**, **Recall**, **F1 Score**
   - Visualized using bar charts

4. **Hyperparameter Tuning**
   - Used `GridSearchCV` and `RandomizedSearchCV` to find optimal parameters
   - Tuned models: Random Forest, SVM

5. **Final Comparison**
   - Compared base and tuned models
   - Selected the best based on F1 Score

---

## 📈 Results Summary

| Model                  | Accuracy | Precision | Recall | F1 Score |
|------------------------|----------|-----------|--------|----------|
| Logistic Regression    | 0.8937   |0.6956     |0.3720  | 0.4848   |
| Random Forest          | 0.9406   |0.9285     |0.6046  | 0.7323   |
| Support Vector Machine | 0.9000   |0.7619     |0.3720  | 0.5000   |
| KNN                    | 0.8937   |0.6667     |0.4186  | 0.5142   |
| Decision Tree          | 0.8968   |0.6000     |0.6976  | 0.6451   |

