In this project we will use various predictive models to see how accurate they are in detecting whether a transaction is a 
normal payment or a fraud and find the best one. Financial institutions and card issuers have adopted a comprehensive 
approach to security that tackles fraud on four fronts. The first step is to devalue sensitive information to make it less 
useful if it falls into the wrong hands. An example is tokenization, which "converts credit card numbers into randomlygenerated values (tokens)." A token is a unique number relating to a specific transaction and has no use beyond that 
transaction. Consequently, a cybercriminal will find the token data he has obtained to be worthless. Second, there is 
increasing reliance on the analysis of data, with the object of detecting unusual patterns, for example where the location 
of the transaction differs from that of the cardholder's mobile phone. Third, pushing businesses and others in the 
payment system to observe industry protocols, such as the Payment Card Industry (PCI) standards, for the protection of 
data. For example, under PCI standards, neither point-of-sale (POS) terminals nor a business's own records, can store 
consumer's credit card numbers. Finally, alerting consumers to the dangers of card fraud and encouraging them to 
adopt best practices, such as monitoring their accounts regularly. Credit card fraud detection systems use a combination 
of statistical and machine learning techniques to analyze transactional data and identify patterns, trends, and anomalies 
that indicate potential fraud. Some common techniques include supervised and unsupervised machine learning 
algorithms, anomaly detection, and neural networks. These techniques help detect fraudulent activities in real-time and 
allow credit card issuers to take appropriate actions to prevent further losses. Effective credit card fraud detection 
systems can help reduce financial losses for financial institutions, merchants, and consumers. However, it is important to 
balance the need for fraud detection with the need for minimal disruption to legitimate transactions. False positives can 
be costly and can negatively impact customer experience. Therefore, credit card issuers must continuously refine their 
fraud detection systems to improve accuracy and minimize disruption to legitimate transactions.

DATASET LINK:https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.
