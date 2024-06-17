### Credit Card Fraud Detection

**Author: Harpreet Sohal**

#### Executive summary
This project explores the possibility of creating models for fraud detection, specifically in the context of credit card transactions. Financial losses caused by credit card fraud amount to tens of billions of dollars globally. This project aims to leverage machine learning techniques to identify and prevent fraudulent transactions effectively.

#### Rationale
Credit card fraud is a significant issue that results in substantial financial losses for individuals and financial institutions. By improving fraud detection mechanisms, we can reduce these losses, enhance risk management practices, and improve customer trust and satisfaction.

#### Research Question
How can we effectively detect fraudulent credit card transactions to minimize financial losses and enhance risk management practices?

#### Data Sources
The dataset used for this project is simulated using the Transaction Data Simulator provided by the Fraud Detection Handbook. The data includes dummy customers and their transactions, with fraud data added for three scenarios:
1. Any transaction with an amount greater than 220 is considered fraudulent.
2. All transactions at randomly selected terminals over 28 days are marked as fraudulent.
3. One-third of transactions by randomly selected customers over 14 days are marked as fraudulent after their amounts are multiplied by five.

#### Methodology
- **Data Loading and Understanding**: Load the data and understand the features.
- **Visualizations**: Create visualizations to understand the distribution of features and the presence of fraud in different scenarios.
- **Feature Engineering**: Create new features that might be useful for detecting fraud.
- **Train/Test Split**: Split the dataset into training and testing sets.
- **Baseline Model**: Train a logistic regression model and evaluate it.
- **Simple Model**: Train a decision tree model and evaluate it.
- **Model Scoring**: Calculate accuracy, precision, recall, and F1 score for the models.
- **Model Comparison**: Compare the performance of the baseline model and the simple model.
- **Improve the Model**: Use RandomizedSearchCV to fine-tune a Random Forest model and evaluate it.

#### Results
The results show that while both the baseline (Logistic Regression) and simple (Decision Tree) models achieve high accuracy due to class imbalance (majority class being non-fraudulent transactions), the recall for fraudulent transactions is relatively low. This indicates that many fraudulent transactions are being missed. By using RandomizedSearchCV to fine-tune a Random Forest model, the recall and overall performance of the fraud detection system were improved.

#### Next steps
- **Further Feature Engineering**: Explore additional features that may improve model performance.
- **Advanced Modeling Techniques**: Implement more advanced models like Gradient Boosting Machines or Neural Networks.
- **Real-world Data**: Validate the models on real-world credit card transaction data.
- **Deployment**: Develop a system for real-time fraud detection and integrate it with financial institutions' transaction processing systems.

#### Outline of project

- Credit-Card-Fraud notebook (https://github.com/harpreetsohal1/Credit-Card-Fraud/blob/main/Credit-Card-Fraud.ipynb))

##### Contact and Further Information
For any questions or further information, please contact Harpreet Sohal.
