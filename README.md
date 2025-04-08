# Credit Card Fraud Detection Using Supervised Learning

This project focuses on detecting fraudulent credit card transactions using machine learning models on an imbalanced dataset. It includes data preprocessing, model training, performance evaluation, and business-focused insights.

---

## Project Description

Credit card fraud poses serious financial risks to both companies and consumers. The dataset used in this project contains European cardholder transactions, with only 0.17% labeled as fraud, making it a highly imbalanced classification task.

This project aims to develop models capable of identifying fraud patterns and minimizing false negatives, which are the most costly errors in this scenario.

The workflow includes:
- Data cleaning and handling class imbalance
- Exploratory data analysis
- Model training and comparison (Logistic Regression, Random Forest, XGBoost)
- Evaluation using precision, recall, F1-score, and ROC-AUC
- Business interpretation and recommendations

---

## Dataset

- **Source**: [Kaggle – Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Transactions**: 284,807
  - Legitimate: 284,315
  - Fraudulent: 492 (~0.17%)
- **Features**: 30 anonymized numerical features (PCA-transformed)

> The dataset is not included in this repo. To use this project, download `creditcard.csv` from Kaggle and place it in the root directory or a `/data` folder.

---

## Tools Used

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

---

## Model Comparison

| Model               | Precision (Fraud) | Recall (Fraud) | F1-Score (Fraud) | ROC-AUC |
|---------------------|-------------------|----------------|------------------|---------|
| Logistic Regression | 0.99              | 0.86           | 0.92             | 0.98    |
| Random Forest       | 1.00              | 0.86           | 0.93             | 0.97    |
| XGBoost             | 0.99              | 0.87           | 0.93             | 0.98    |

All models performed well, with **XGBoost and Random Forest** achieving the best balance between precision and recall.

---

## Key Takeaways

- Logistic Regression provides solid performance and interpretability.
- Random Forest and XGBoost offer higher precision and F1-scores.
- Proper handling of class imbalance is crucial for fraud detection models.
- High recall is vital to reduce undetected fraud cases.

---

## How to Run

1. Clone the repository
2. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
3. Place `creditcard.csv` in the project directory
4. Run the notebook `credit_card_fraud_detection.ipynb`

---

## License

This project is for educational and research purposes only.
