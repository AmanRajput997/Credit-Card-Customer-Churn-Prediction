# Credit-Card-Customer-Churn-Prediction
## 📝 Description
This project aims to predict whether a credit card customer will churn (i.e., close their account). By identifying customers who are likely to churn, the bank can take proactive steps to retain them. This is a binary classification problem, and a neural network model is built using TensorFlow and Keras to make the predictions.

## 💾 Dataset
The dataset used for this project is the "Churn Modelling" dataset from Kaggle. It contains information about bank customers who have held a credit card.

You can find the dataset here: [Credit Card Customer Churn Prediction Dataset](https://www.google.com/search?q=https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customer-churn-prediction)

### Columns
The dataset has 10,000 rows and the following 14 columns:

• __RowNumber:__ Row number

• **CustomerId:** Unique identifier for each customer

• __Surname:__ Customer's surname

•__CreditScore:__ Customer's credit score

• __Geography:__ Customer's country (France, Spain, Germany)

• __Gender:__ Customer's gender

• __Age:__ Customer's age

• __Tenure:__ Number of years the customer has been with the bank

• __Balance:__ Customer's account balance

• __NumOfProducts:__ Number of bank products the customer uses

• HasCrCard: Whether the customer has a credit card (1 = yes, 0 = no)

• IsActiveMember: Whether the customer is an active member (1 = yes, 0 = no)

• EstimatedSalary: Customer's estimated salary

• Exited: Whether the customer has churned (1 = yes, 0 = no) - This is the target variable.

## ⚙️ Methodology
The project follows these steps:

1. Data Loading and Exploration: The data is loaded using pandas, and initial exploration is done to understand the data's structure and features.

2. Data Preprocessing:

• Unnecessary columns (RowNumber, CustomerId, Surname) are dropped.

• Categorical features (Geography, Gender) are converted into numerical format using one-hot encoding.

3. Train-Test Split: The data is split into training (80%) and testing (20%) sets.

4. Feature Scaling: The numerical features are scaled using StandardScaler to ensure that all features contribute equally to the model's training.

5. Model Building: A sequential neural network is built using TensorFlow/Keras with the following architecture:

• An input layer with 11 neurons and a ReLU activation function.

• A hidden layer with 11 neurons and a ReLU activation function.

• An output layer with 1 neuron and a sigmoid activation function for binary classification.

6. Model Compilation and Training: The model is compiled with the Adam optimizer and binary cross-entropy loss function. It is then trained for 100 epochs.

## 📈 Results
The model's performance is evaluated based on its accuracy. The final accuracy on the test set is approximately 85%.

Training and Validation Loss
Training and Validation Accuracy
## 🚀 How to Run
To run this project, you will need to have a Python environment with the following libraries installed:

• pandas

• numpy

• scikit-learn

• tensorflow

• matplotlib

__You can then open the Jupyter Notebook file (credit-card-customer-churn-prediction.ipynb) and run the cells sequentially.__
