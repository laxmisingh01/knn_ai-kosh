# KNN Classification and Regression on AI Kosh Dataset

This project demonstrates how to apply **K-Nearest Neighbors (KNN)** for both:

- ✅ Classification — predicting disability type  
- ✅ Regression — predicting total population count  

using a real-world dataset from India’s **AI Kosh** platform.

The impact of varying the value of **K** on model performance is analyzed through:

- 📈 Accuracy vs K (Classification)
- 📉 RMSE vs K (Regression)

---

## 📂 Dataset

Source: AI Kosh – UDID Disability Statistics Dataset  

The dataset contains:

- **Categorical Features**
  - state_name
  - district_name
  - age_group

- **Numerical Features**
  - male_count
  - female_count

- **Targets**
  - disability_type_name (classification)
  - total_count (regression)

> ⚠️ The dataset is not included in this repository.  
> Please download it from the AI Kosh portal and place it in the project directory as:
>
> `UDIDDATA_0.csv`

---

## 🧠 Methodology

1. Load and inspect dataset
2. Handle missing values (if any)
3. Split features and targets
4. Encode categorical variables using One-Hot Encoding
5. Scale numerical features using StandardScaler
6. Train KNN models for multiple K values
7. Evaluate:
   - Accuracy for classification
   - RMSE for regression
8. Plot performance curves

---

## 📊 Results Summary

- **Classification:** Best accuracy observed around K = 9–11  
- **Regression:** Lowest RMSE observed around K = 1–3  

These results show how neighborhood size strongly influences KNN behavior.

---



```bash
pip install pandas numpy matplotlib scikit-learn
