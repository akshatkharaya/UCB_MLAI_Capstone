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
Performed exploratory data analysis (EDA) and built models using classification algorithms, e.g., Logistic Regression, Decision Tree, Random Forest, XGBoost. As per instructor feedback after Part 1 submission, tested 3 other algorithms - Isolation Forest, One-Class SVM and Auto-Encoders. The goal of these Machine Learning and Deep Learning algorithms is to classify each transaction into fraud vs not fraud. Each model is then evaluated across various factors such as accuracy, precision (i.e., correctness of the prediction when the model predicts a transaction is fraud), recall (i.e., out of the actual fraud transactions, how many is the model able to capture), etc. Further, we look at AUPRC (Area Under Precision Recall Curve). 

#### Results
Among the classification algorithms tested, overall recommendation is XGBoost due to strong performance and faster training and inference. 
XGBoost has the best performance in terms of AUPRC with a value of 0.8823 while Random Forest has AUPRC of 0.8677. While XGBoost has 15 false negatives and Random Forest has 14, the number of false positives for XGBoost are significantly lower at 18 than Random Forest at 33.  
Random Forest has a significantly higher training time of ~500 seconds (on my laptop) than XGBoost (~10 seconds).  
Logistic Regression and Decision Tree have significantly worse performance than XGBoost and Random Forest. 
Algorithms tried as per instructor feedback (Isolation Forest, One-Class SVM and Auto-Encoders) were evaluated using F1 score but showed poor performance. 

#### Next steps
There are several next steps to undertake before the model can be deployed in production. 
(1) Test more algorithms: More algorithms should be tested to select the best one based on accuracy measure(s) and training/inference times. 
(2) Optimize hyperparameters: For the top 2-3 most appropriate algorithms, find the optimal hyperparameters using a more powerful computing cluster, which I could not do due to compute limitations. 
(3) Senstivity analysis: Conduct sensitivity analysis based on business knowledge. For example, how quickly and well does the model capture new fraud patterns? Is it too sensitive to particular features that sometimes may be missing during real-time execution? 
(4) Champion vs challenger: If there is an existing model in production (i.e., champion), then the proposed model should be deployed as challenger model in parallel to evaluate its real-world performance. It will also help identify and resolve any issues that occur in production. 

#### Outline of project
This project includes the README file summarizing the context, methodology and results, and 1 Jupyter notebook that includes the technical analysis. 
- Link to Jupyter notebook: https://github.com/akshatkharaya/UCB_MLAI_Capstone/blob/main/Capstone_Final_AkshatKharaya.ipynb 

##### Contact and Further Information
Contact: Akshat Kharaya (https://www.linkedin.com/in/akshatkharaya/)