## Credit Card Fraud Detection

**Author: Harpreet Sohal**

### Executive summary

**Project overview and goals:** The goal of this project is to develop and evaluate machine learning models for detecting fraudulent credit card transactions. By leveraging a simulated dataset and various classification techniques, we aim to identify the most effective model for fraud detection. We will train, tune, and compare various models, including Logistic Regression, Decision Tree, and Random Forest, to determine the best model for identifying fraudulent transactions. Additionally, we will analyze feature importance to gain insights into which transaction attributes are most indicative of fraud.

**Findings:** The best model for detecting credit card fraud is the Decision Tree model, with an accuracy score of 93.45%, a precision of 93.64%, and an F1 score of 28.83%. This model outperforms the Logistic Regression and Random Forest models in terms of recall, indicating a better balance between detecting fraudulent transactions and minimizing false positives. Despite the Random Forest model achieving slightly lower performance, it offers valuable insights through feature importance analysis.

**Results and conclusion:** The evaluation of the models shows that the Decision Tree model is the most effective in detecting fraudulent transactions, balancing precision and recall effectively. The key features identified as most important for fraud detection include the transaction amount, the day of the week, and the hour of the transaction. Future work can focus on enhancing model performance by incorporating more advanced techniques and real-world data validation.

### Rationale

Credit card fraud results in significant financial losses for individuals and institutions. Developing robust fraud detection models can help mitigate these losses, improve risk management, and enhance customer trust. Identifying fraudulent transactions accurately and efficiently is crucial for preventing financial fraud and protecting assets.

### Research Question

How can we effectively detect fraudulent credit card transactions to minimize financial losses and enhance risk management practices? Further research is necessary to reduce these losses and provide banks with diverse data points that can be explored further. This includes determining the amount of funds that need to be set aside for fraudulent transactions and assessing how quickly a fraud can be identified in real-time scenarios based on the frequency of transactions.

### Data Sources

**Dataset:** The dataset used for this project is simulated using the Transaction Data Simulator provided by the Fraud Detection Handbook. The data includes dummy customers and their transactions, with fraud data added for three scenarios:
1. Any transaction with an amount greater than 220 is considered fraudulent.
2. All transactions at randomly selected terminals over 28 days are marked as fraudulent.
3. One-third of transactions by randomly selected customers over 14 days are marked as fraudulent after their amounts are multiplied by five.

### Methodology

- **Data Loading and Understanding:** Load the data and understand the features.
- **Visualizations:** Create visualizations to understand the distribution of features and the presence of fraud in different scenarios.
  - Transaction Amount Distribution https://github.com/harpreetsohal1/Credit-Card-Fraud/blob/main/output/Transaction_Amount_Distribution.png
  - Fraud Scenarios   https://github.com/harpreetsohal1/Credit-Card-Fraud/blob/main/output/Fraud_Scenarios.png
  - Fraud vs Non-Fraud Transactions (https://github.com/harpreetsohal1/Credit-Card-Fraud/blob/main/output/Fraud_vs_NonFraud.png)
- **Feature Engineering:** Create new features that might be useful for detecting fraud.
- **Train/Test Split:** Split the dataset into training and testing sets.
- **Baseline Model:** Train a logistic regression model and evaluate it.
- **Simple Model:** Train a decision tree model and evaluate it.
- **Model Scoring:** Calculate accuracy, precision, recall, and F1 score for the models.
- **Model Comparison:** Compare the performance of the baseline model and the simple model.
- **Improve the Model:** Use GridSearchCV to fine-tune a Random Forest model and evaluate it.

### Model evaluation and results 

**Baseline Model Evaluation (Logistic Regression):**
- Accuracy: 93.32%
- Precision: 100%
- Recall: 14.26%
- F1 Score: 24.96%

  - https://github.com/harpreetsohal1/Credit-Card-Fraud/blob/main/output/logistic_regression_confusion_matrix.png

**Simple Model Evaluation (Decision Tree):**
- Accuracy: 93.45%
- Precision: 93.64%
- Recall: 17.04%
- F1 Score: 28.83%
  - https://github.com/harpreetsohal1/Credit-Card-Fraud/blob/main/output/decision_tree_confusion_matrix.png

**Improved Model Evaluation (Random Forest):**
The Decision Tree model is the best model for detecting fraudulent transactions, and balancing precision and recall effectively.
- Accuracy: 93.41%
- Precision: 91.71%
- Recall: 16.89%
- F1 Score: 28.53%
  - https://github.com/harpreetsohal1/Credit-Card-Fraud/blob/main/output/random_forest_confusion_matrix.png


### Outline of project

- [Link to download data](https://github.com/harpreetsohal1/Credit-Card-Fraud/tree/main/simulated-data-csv)
- [Link to notebook](https://github.com/harpreetsohal1/Credit-Card-Fraud/blob/main/Credit-Card-Fraud_1.ipynb)
- [Link to visuals](https://github.com/harpreetsohal1/Credit-Card-Fraud/tree/main/output)

### Contact and Further Information

For any questions or further information, please contact Harpreet Sohal (harpreetsohal1@gmail.com).
