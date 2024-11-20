### Capstone Project Title: Credit Card Fraud Detection

**Author**: Akshat Kharaya

#### Executive summary

#### Rationale
Credit card fraud is a big problem for banks. According to Nilson Report, credit and debit card fraud losses reached a record $34.36 billion in 2022 (source: https://wallethub.com/edu/cc/credit-card-fraud-statistics/25725). Robust credit card fraud detection is critical to safeguard customers and company's finances. 

#### Research Question
How to detect fraud in credit card transactions?

#### Data Sources
Credit card data on Kaggle: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud. As noted on the Kaggle webpage, “This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions.”

#### Methodology
Performed exploratory data analysis (EDA) and built models using 4 classification algorithms: Logistic Regression, Decision Tree, Random Forest and XGBoost. 

#### Results
Among the 4 classification algorithms, overall recommendation is XGBoost due to strong performance and faster training and inference. 
XGBoost has the best performance in terms of AUPRC with a value of 0.8823 while Random Forest has AUPRC of 0.8677. While XGBoost has 15 false negatives and Random Forest has 14, the number of false positives for XGBoost are significantly lower at 18 than Random Forest at 33.  
Random Forest has a significantly higher training time of ~500 seconds (on my laptop) than XGBoost (~10 seconds).  
Logistic Regression and Decision Tree have significantly worse performance than XGBoost and Random Forest. 

#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information