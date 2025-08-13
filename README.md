# 🧠 Customer Churn Prediction using Artificial Neural Networks (ANN)

This project predicts **customer churn** (whether a customer will leave or stay) using an **Artificial Neural Network (ANN)** built with TensorFlow/Keras.

The dataset contains 14 features including demographic, account, and financial information, with the target variable **Exited**:
- **1** = customer exited  
- **0** = customer retained  

---

## 📊 Dataset Details
| Feature | Description |
|---------|-------------|
| Row_number | Index for each customer |
| Customer_ID | Unique ID for each customer |
| Surname | Customer surname |
| Credit_Score | Customer's credit score |
| Geograpgy | Customer's location *(typo corrected to Geography)* |
| Gender | Gender of customer |
| Age | Age of customer |
| Tenure | Years of association with the company |
| Balance | Account balance |
| NumOfProducts | Number of products owned |
| HasCrCard | Whether the customer has a credit card |
| IsActiveMember | Whether the customer is active |
| EstimatedSalary | Estimated salary |
| Exited | **Target** (1 = exited, 0 = stayed) |

---

## 🛠️ Project Workflow
1. **Data Loading & Exploration**
2. **Data Cleaning**
   - Handle null values  
   - Remove duplicate records  
   - Drop non-predictive ID/name columns  
3. **Data Preprocessing**
   - One-hot encoding for categorical columns  
   - Standard scaling for numerical columns  
4. **Train-Test Split** (80% training, 20% testing)
5. **Model Building**
   - Keras Sequential model with:
     - Dense(64, ReLU) + Dropout(0.3)
     - Dense(32, ReLU) + Dropout(0.2)
     - Dense(1, Sigmoid)
6. **Model Training**
   - Early stopping based on validation accuracy  
7. **Model Evaluation**
   - Confusion Matrix  
   - Classification Report  
   - Accuracy score  

---

## 💻 Technologies Used
- **Python 3.x**
- **Pandas** & **NumPy** — data manipulation
- **Scikit-learn** — preprocessing, metrics
- **TensorFlow/Keras** — ANN model
- **Matplotlib** — visualizations

