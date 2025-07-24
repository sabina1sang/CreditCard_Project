# Credit Card Fraud Detection 🛡️

This project focuses on detecting fraudulent transactions in credit card data using machine learning techniques. It handles extreme class imbalance using SMOTE and evaluates multiple models including Logistic Regression, Random Forest, and XGBoost.

---

## 📂 Dataset

- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Contains transactions made by European cardholders in September 2013.
- Highly imbalanced dataset:
  - Legitimate: `284,315`
  - Fraudulent: `492`

---

## 🧠 Models Used

| Model               | Sampling Used | Description                            |
|--------------------|----------------|----------------------------------------|
| Logistic Regression | SMOTE          | Baseline linear classifier             |
| Random Forest       | SMOTE          | Ensemble of decision trees             |
| XGBoost             | No SMOTE       | Boosted trees with scale_pos_weight    |

---

## 📊 Evaluation Metrics

- **Confusion Matrix**
- **Classification Report** (Precision, Recall, F1-score)
- **ROC AUC Score**
- **Precision-Recall Curve**

---

## ⚙️ Workflow

1. **Data Loading**
2. **EDA & Visualization**
3. **Feature Scaling**
4. **Train-Test Split (Stratified)**
5. **Handling Imbalance with SMOTE**
6. **Model Training**
7. **Evaluation**
8. **Precision-Recall Curve Plot**

---

## 📈 Sample Output

=== Random Forest ===
Confusion Matrix:
[[56852 11]
[ 24 75]]

Classification Report:
precision recall f1-score support
0 1.00 1.00 1.00 56863
1 0.87 0.76 0.81 99

ROC AUC Score: 0.9813

---

## 🛠️ Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
requirements.txt

nginx
Copy
Edit
numpy
pandas
matplotlib
seaborn
scikit-learn
xgboost
imbalanced-learn
📎 File Structure
Copy
Edit
CreditCard_Project/
│
├── creditcard.csv
├── creditcard_fraud_detection.py
├── random_forest_model.pkl
├── README.md
└── requirements.txt
🚀 Future Work
Hyperparameter tuning

Use of deep learning (e.g., autoencoders)

Streamlit dashboard for live predictions

Deploy as API with Flask or FastAPI

🤝 License
This project is licensed under the MIT License.

📬 Contact
Created by @sabina1sang – feel free to reach out!
