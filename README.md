# Credit-card-fraud-detection
Imbalanced data set - ROS, SMOTE, ADASYN
 <p> It is important for thr credit card companies to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase </p>
<p> 
The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues,original features and more background information about the data is not provided. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.
</p>
<p>The data set is taken from kaggle</p>

Most of the variables in the dataset were a skewed to different extentas and hence they were handled using power transformer before model building. The given data was split into Train and Test while ensuring that the percentage of fraus remains the same in both the splits. Different algorithms were employed for model building on the imbalanced dataset and 3 fold cross validation was performed on them. Different sampling techniques were then employed to balance the dataset and build a suitable model . The best model gave 80 % precision and 83 % recall. 
