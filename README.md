Date: June-July 2025

**The complete project analysis and details is available in 'main.ipynb'.**


**The dataset used for this project is available in the 'data/' folder.**

<h1>Credit Risk Prediction Project</h1>

The risk in credit and lending provided by banks to individuals lies in the potential for default, where the borrower is unable to fully repay their loans. Banks must therefore assess whether individuals have the capacity to reimburse their loans to ensure that these financial investments yield positive outcomes. This is important for ensuring sound financial decision-making.

The goal of this project is to develop a model that assesses whether an individual is likely to fail to repay their debts on time. This credit scoring algorithm will be implemented as a supervised machine learning classification task, using the "Give Me Some Credit" dataset provided by Kaggle (1).

This dataset provides relevant features such as prior failure to repay loans on time, monthly income, lines of credit, number of dependents and number of current loans. The model will predict the whether an individual will experience a delinquency of 90 days or worse. Among the features, the most indicative of credit default is expected to be previous occurrences of financial stress, demonstrated by repeated failures to repay loans on time.

<h2>Project Takeaways</h2>

* The model that performed the best was HistGradientBoostingClassifer with hyperparameter optimization and feature selection. 
* The final model demonstrated strong recall (0.80), but lower precision and f1. However recall is prioritized because it focuses on ensuring all positive cases (potential fraud) are identified.
* The limitations of this model are potentially more cases of false positives (due to low precision) and the moderate-level of interpretably provided by the HistGradientBoostingClassifier model.
* The features that most influence a person's probability to commit credit fraud in the next 2 years includes Debt-to-Income ratio (DTI), previous fraud and current debts. 

<h2>References</h2>

(1) Credit Fusion and Will Cukierski. Give Me Some Credit. https://kaggle.com/competitions/GiveMeSomeCredit, 2011. Kaggle.
