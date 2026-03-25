# UPI-transaction-classification

📌 Project Overview
This project focuses on building a **Random Forest Classifier** to predict the status of UPI transactions (SUCCESS or FAILED) based on transaction details such as amount, sender/receiver UPI IDs, and timestamp.

 📂 Dataset
File: `transactions.csv`
Columns:
1. `Sender UPI ID` → categorical feature
2. `Receiver UPI ID` → categorical feature
3. `Amount (INR)` → numerical feature
4. `Timestamp` → converted to `Hour`
5. `Status` → target variable (`SUCCESS` = 1, `FAILED` = 0)

⚙️ Preprocessing Steps
1. Encode categorical features (`Sender UPI ID`, `Receiver UPI ID`) using **LabelEncoder**.
2. Convert `Status` column into numeric values.
3. Extract `Hour` feature from `Timestamp`.
4. Handle missing values ('dropna').
5. Train-test split (80% train, 20% test).

🧠 Model
 Algorithm: Random Forest Classifier
 Library: scikit-learn
 Training: Model trained on preprocessed features.
 📊 Evaluation
 Metrics Used:
  - Accuracy Score
  - Classification Report (Precision, Recall, F1-score)
  - Confusion Matrix (visualized using Seaborn heatmap)

 Results:
- Train Accuracy: ~1.0  
- Test Accuracy: ~0.545  
- Confusion Matrix and Classification Report included.

 🚀 How to Run
1. Clone the repository:
 git clone https://github.com/your-username/upi-transaction-classification.git

📈 Future Improvements
1.Try other ML models (Logistic Regression, XGBoost).
2.Add feature engineering (day of week, transaction frequency).
3.Hyperparameter tuning for Random Forest.

👨‍💻 Author: Muthu
📌 Language: Python (pandas, scikit-learn, seaborn, matplotlib)
