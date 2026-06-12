__ML Classification Project__

Project Title: Customer Churn Prediction Using Machine Learning

Project Overview:

This project aims to build and evaluate machine learning classification models for predicting customer churn. Customer churn refers to customers who stop using a company's services. Predicting churn helps businesses identify at-risk customers and improve retention strategies.

A synthetic dataset was generated using Python to simulate customer behavior, making the project fully reproducible without requiring external datasets.

Objectives

* Perform data preprocessing and feature engineering.
* Split data into training and testing sets.
* Train and evaluate multiple classification algorithms.
* Compare model performance using standard evaluation metrics.
* Visualize results using confusion matrices, ROC curves, and feature importance plots.

Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

Dataset Description

The dataset contains simulated customer information with the following features:

| Feature         | Description                               |
| --------------- | ----------------------------------------- |
| Age             | Customer age                              |
| Tenure          | Number of months with the company         |
| MonthlyCharges  | Monthly subscription charges              |
| ContractType    | Type of contract                          |
| InternetService | Type of internet service                  |
| SupportCalls    | Number of support calls made              |
| Churn           | Target variable (0 = No Churn, 1 = Churn) |

The target variable was generated using business rules where customers with high monthly charges, frequent support calls, and low tenure are more likely to churn.

Project Workflow
 1. Data Generation

* Generate synthetic customer records.
* Create churn labels based on predefined business logic.
2. Data Preprocessing

* Encode categorical variables using Label Encoding.
* Scale numerical features using StandardScaler.

3. Train-Test Split

* Split dataset into:

  * 80% Training Data
  * 20% Testing Data
4. Model Training

Two machine learning algorithms were trained:
 Logistic Regression

* Linear classification model
* Fast and interpretable
 Random Forest Classifier

* Ensemble learning model
* Handles non-linear relationships effectively

5. Cross Validation

* 5-Fold Cross Validation performed for both models.
* Helps evaluate model stability and generalization.
 6. Model Evaluation

The following metrics were used:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score

7. Visualization

Generated visualizations include:

* Churn Distribution Plot
* Confusion Matrix
* ROC Curve
* Feature Importance Plot

Evaluation Metrics
 Accuracy

Measures overall correctness of predictions.
Precision

Measures how many predicted churn customers actually churned.

Recall

Measures how many actual churn customers were correctly identified.
 F1 Score
Harmonic mean of Precision and Recall.
ROC-AUC

Measures model's ability to distinguish between churn and non-churn customers.
Expected Results

| Model               | Accuracy  | Precision | Recall    | F1 Score  | ROC-AUC   |
| ------------------- | --------- | --------- | --------- | --------- | --------- |
| Logistic Regression | 85% - 92% | 84% - 90% | 83% - 90% | 84% - 90% | 90% - 96% |
| Random Forest       | 90% - 97% | 90% - 97% | 90% - 97% | 90% - 97% | 95% - 99% |

Random Forest is expected to outperform Logistic Regression due to its ability to capture complex patterns in customer behavior.

 Project Structure

text
Customer-Churn-Prediction/
│
├── Customer_Churn_Prediction.ipynb
├── README.md
├── requirements.txt
└── images/
    ├── churn_distribution.png
    ├── confusion_matrix.png
    ├── roc_curve.png
    └── feature_importance.png
 Installation

Clone the repository:

bash
git clone https://github.com/your-username/customer-churn-prediction.git


Navigate to the project folder:

bash
cd customer-churn-prediction


Install dependencies:

bash
pip install -r requirements.txt


Running the Project

Open Jupyter Notebook:

bash
jupyter notebook


Run all cells in:
text
Customer_Churn_Prediction.ipynb


 Key Findings

* Customers with shorter tenure are more likely to churn.
* Higher monthly charges increase churn probability.
* Frequent support calls indicate customer dissatisfaction.
* Random Forest achieved the best overall performance.

 Future Improvements

* Use real-world telecom customer data.
* Perform hyperparameter tuning using GridSearchCV.
* Apply advanced ensemble methods such as XGBoost.
* Deploy the model using Flask or Streamlit.

 Conclusion

This project demonstrates the complete machine learning workflow for customer churn prediction, including data preprocessing, model training, cross-validation, evaluation, and visualization. The results show that ensemble methods such as Random Forest provide strong predictive performance for churn classification tasks.

 