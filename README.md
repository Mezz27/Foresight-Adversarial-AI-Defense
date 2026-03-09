# 🔥 Foresight: Machine Learning Model for Detecting DNS Tunneling Attacks

## 📌 Project Overview

**Foresight** is a machine learning–based cybersecurity project designed to detect **DNS tunneling attacks**, a technique used by attackers to hide malicious data inside DNS queries to bypass traditional security systems.

By analyzing network traffic patterns, the model learns to distinguish **legitimate DNS requests from malicious ones**, helping automate threat detection in network environments.

The project explores multiple machine learning models and evaluates their ability to detect suspicious DNS activity.

---

# 🎯 Objectives

* Detect DNS tunneling attacks using machine learning
* Compare multiple classification algorithms
* Handle **class imbalance** in cybersecurity datasets
* Evaluate models using multiple performance metrics
* Improve automated detection of malicious DNS traffic

---

# 🧠 Machine Learning Models Used

The following models were trained and compared:

* Logistic Regression
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)
* XGBoost

Each model was evaluated on three dataset versions:

* Original Dataset
* SMOTE Oversampled Dataset
* Undersampled Dataset

---

# ⚙️ Technologies & Libraries

The project is implemented in **Python** using:

* pandas
* numpy
* scikit-learn
* xgboost
* imbalanced-learn
* matplotlib

Development and experimentation were performed using **Jupyter Notebook**.

---

# 📊 Model Performance Results

| Model               | Dataset       | Accuracy | Precision | Recall | F1 Score | AUC-ROC |
| ------------------- | ------------- | -------- | --------- | ------ | -------- | ------- |
| XGBoost             | Undersampling | 0.582    | 1.000     | 0.513  | 0.678    | 0.758   |
| XGBoost             | SMOTE         | 0.857    | 0.857     | 1.000  | 0.923    | 0.755   |
| XGBoost             | Original      | 0.854    | 0.857     | 0.996  | 0.921    | 0.556   |
| SVM                 | Original      | 0.582    | 1.000     | 0.513  | 0.678    | 0.752   |
| SVM                 | SMOTE         | 0.143    | 0.000     | 0.000  | 0.000    | 0.430   |
| SVM                 | Undersampling | 0.143    | 0.000     | 0.000  | 0.000    | 0.424   |
| Random Forest       | SMOTE         | 0.857    | 0.857     | 1.000  | 0.923    | 0.767   |
| Random Forest       | Undersampling | 0.857    | 0.857     | 1.000  | 0.923    | 0.764   |
| Random Forest       | Original      | 0.567    | 0.800     | 0.660  | 0.723    | 0.522   |
| Logistic Regression | Original      | 0.582    | 1.000     | 0.513  | 0.678    | 0.743   |
| Logistic Regression | SMOTE         | 0.200    | 1.000     | 0.067  | 0.126    | 0.580   |
| Logistic Regression | Undersampling | 0.252    | 0.926     | 0.139  | 0.241    | 0.576   |
| Decision Tree       | SMOTE         | 0.851    | 0.862     | 0.984  | 0.919    | 0.761   |
| Decision Tree       | Undersampling | 0.857    | 0.857     | 1.000  | 0.923    | 0.502   |
| Decision Tree       | Original      | 0.526    | 0.792     | 0.605  | 0.686    | 0.318   |

---

# 📈 Key Findings

* **Random Forest and XGBoost showed the strongest overall performance** for detecting DNS tunneling activity.
* Handling dataset imbalance with **SMOTE significantly improved detection accuracy**.
* **SVM struggled with oversampled and undersampled datasets**, indicating sensitivity to feature distribution.
* Tree-based models proved more robust for network anomaly detection.

---

# 🔐 Cybersecurity Relevance

DNS tunneling is commonly used for:

* Data exfiltration
* Command-and-control communication
* Malware communication
* Firewall evasion

Machine learning models like those used in **Foresight** can help detect these hidden attacks by identifying abnormal traffic patterns.

---

# 🧪 Project Workflow

The project pipeline follows this process:

Dataset Collection
→ Data Preprocessing
→ Feature Scaling
→ Handling Class Imbalance (SMOTE / Undersampling)
→ Model Training
→ Model Evaluation
→ Performance Comparison

---

# 🚀 Future Improvements

* Real-time DNS traffic monitoring
* Integration with SIEM systems
* Deep learning–based anomaly detection
* Real-time attack alert dashboard
* Deployment as a network security API

---

# 👩‍💻 Author

**Meenu Hani**
Senior Data Analyst

---

# License

This project is protected under an All Rights Reserved license.  
Permission from the author is required before any use or distribution.

---

# ⭐ Support

If you found this project useful, consider **starring the repository**.

