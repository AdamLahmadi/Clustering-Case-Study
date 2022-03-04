## Clustering in the Marketing Department

# Quick overview and Impact

One of the key pain points for marketers is to identify customer needs. By understanding the customer, marketers can launch a targeted marketing campaign that is tailored for specific needs. If data about customers is available, data science can be applied to perform market segmentation.

In this case study we will analyse extensive customer data and use K-Means clustering to divide customers into 4 distinctive groups to allow marketers to know their customers better.

The following customer clusters were created:

  - First Customers cluster (Transactors): Customers who pay least amount of interest charges and careful with their money, Cluster with lowest balance ($104) and cash advance (\$303), Percentage of full payment = 23%.

  - Second customers cluster (revolvers): Customers who use credit card as a loan (most lucrative sector): highest balance ($5000) and cash advance (~$5000), low purchase frequency, high cash advance frequency (0.5), high cash advance transactions (16) and low percentage of full payment (3%).

  - Third customer cluster (VIP/Prime): Customers with high credit limit $16K and highest percentage of full payment, target for increase credit limit and increase spending    habits.

  - Fourth customer cluster (low tenure): Customers with low tenure (7 years), low balance

# Our Dataset

For this case study we are using the Kaggle dataset: https://www.kaggle.com/arjunbhasin2013/ccdata

The dataset summarizes the usage behavior of about 9000 active credit card holders during the last 6 months. The file is at a customer level with 18 behavioral variables that look as follows:

CUSTID : Identification of Credit Card holder (Categorical)

BALANCE: Balance amount left in their account to make purchases (

BALANCEFREQUENCY: How frequently the Balance is updated, score between 0 and 1 (1 = frequently updated, 0 = not frequently updated)

PURCHASES: Amount of purchases made from account

ONEOFFPURCHASES: Maximum purchase amount done in one-go

INSTALLMENTSPURCHASES: Amount of purchase done in installment

CASH ADVANCE: Cash in advance given by the user

PURCHASESFREQUENCY: How frequently the Purchases are being made, score between 0 and 1 (1 = frequently purchased, 0 = not frequently purchased)

ONEOFFPURCHASESFREQUENCY: How frequently Purchases are happening in one-go (1 = frequently purchased, 0 = not frequently purchased)

PURCHASESINSTALLMENTSFREQUENCY: How frequently purchases in installments are being done (1 = frequently done, 0 = not frequently done)

CASHADVANCEFREQUENCY: How frequently the cash in advance being paid

CASHADVANCETRX: Number of Transactions made with "Cash in Advanced"

PURCHASESTRX: Number of purchase transactions made

CREDITLIMIT: Limit of Credit Card for user

PAYMENTS: Amount of Payment done by user

MINIMUM_PAYMENTS: Minimum amount of payments made by user

PRCFULLPAYMENT: Percentage of full payment paid by user

TENURE: Tenure of credit card service for user
