# Fraud Detection

## Project Overview
This project explores modern **AI-based techniques for fraud detection** using a real-world credit card transactions dataset. It was fully developed using **Alteryx Designer**, focusing on model evaluation and predictive performance.

<p align="center">
  <img src="https://echopx.in/wp-content/uploads/2023/01/Credit-card-activation-fraud.png" 
       alt="Fraud Detection" 
       width="400"/>
</p>

The main goals of the project were:
- To conduct a concise **literature review** on recent AI-based fraud detection methods
- To train and compare several **machine learning models** for fraud detection
- To evaluate models based on key metrics such as **Accuracy**, **AUC**, **F1-score**, **RMSE**, **MAE**, and **MAPE**


## Literature Review
Key paper analyzed:**"Credit Card Fraud Detection Using AdaBoost and Majority Voting"**  
*K. Randhawa et al., IEEE Access, 2018*  
[🔗 View the paper](https://ieeexplore.ieee.org/abstract/document/8292883/)

This paper inspired the use of **Boosting algorithms** (like AdaBoost and XGBoost), which combine weak learners to significantly improve classification performance.


## Alteryx Workflow Structure
The entire workflow was built in **Alteryx Designer** and includes:
- **Importing** the dataset (`creditcard.csv`)
- **Data preprocessing** (cleaning and normalization)
- **Splitting** the dataset into training and test sets
- Training and evaluating multiple models:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Boosted Models (AdaBoost, XGBoost)
  - Visual performance **comparison and metric generation**


## Model Performance Summary
The **Boosted Model** (e.g. XGBoost) showed the strongest performance:
| Metric                  | Boosted Model Result       |
|-------------------------|----------------------------|
| **F1-score**            | 0.7957                     |
| **AUC (ROC Curve)**     | 0.9859                     |
| **Accuracy**            | 0.7551                     |
| **False Negatives**     | 7 only                     |
| **Correlation**         | 0.7988                     |
| **RMSE**                | 0.0256                     |
| **MAE**                 | 0.0011                     |
| **MAPE**                | 61.05%                     |

These results highlight the **effectiveness of Boosted Models** in detecting rare and complex fraudulent transactions.


## Tools & Technologies
- **Alteryx Designer**
- **Machine Learning Algorithms** (Logistic Regression, Trees, Boosting)
- **Classification Metrics**
- Real-world dataset of anonymized credit card transactions
