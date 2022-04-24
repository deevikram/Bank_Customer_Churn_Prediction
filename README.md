# Bank_Customer_Churn_Prediction

Building a deep learning model (ANN) for customer churn predictions

#### Skills used for this project: Exploratory Data Analysis (EDA), Artificial Neural Networks (ANN), Tensorflow, Keras 

## Introduction
Banks provide services and products to customers. Good quality customer services and relevant products marketed to the correct groups can help banks retain customers and maintain a steady customer base. Customer data analysis can help identify deficiencies in the banks' services and products, helping management focus on improvement of the services, thus reducing churn.

Background:'Churn'in the banking and industrial section refers to customers leaving and joining another service provider.

## Objective
- Build a deep learning model for customer churn predictions
- Analysis of the data and summary of the strategies for customer retention

## EDA Excerpts:

![image](https://user-images.githubusercontent.com/83994337/164950300-336d0d46-4278-4b55-9a61-b1a00c2b80b2.png)

- The feature 'CreditScore' is a mostly symmetric distribution, with a peak between 600 and 750. However, there is another peak at 800 where about 300 customers have a credit score of more than 800.The maximum credit score one can have is 850, and the 300 customers having score more than 800 is possible, hence can represent real data.
- There are some outliers present in the box plot for 'CreditScore' versus 'Exited' for the category of custoemrs who left the bank. These can represent real data as well since it is possible to get credit scores less than 400. In general, there was no significant difference in the median credit scores between the categories of customers who remained with the bank and customers who left the bank.
- The same was true for the median credit score for male versus female category of customers. The box plot for 'Gender' versus 'CreditScore' shows outliers present, but this can again represent real data as it is possible to have credit scores less than 400.
- There was no significant difference in the median credit scores between customers who were active members of the bank versus the customers who were not active members in the bank.
- There were no significant differences in the median credit scores for category of customers who were active members or not, or among customers who belonged to France, Germany or Spain. There were no significant differences in the median credit scores of customers who bought 1,2,3 or 4 products from the bank. The box plots for these do show outliers, but could represent real data.

![image](https://user-images.githubusercontent.com/83994337/164950330-93c9eb66-ec83-433c-a64d-4498cdcfa1ea.png)

If we look at age, and at the tenure (number of years the customer has been with the bank), we can clearly see that customers who remained with the bank were younger regardless of how many years they had been with the bank. Customers who left the bank had a higher age regardless of tenure.

### Insights 
- 75 percent of the customers in the data set had credit scores 718 or higher - this indicates that the majority of the customer base had relatively good credit scores. The bank should continue to encourage customers with good credit scores as a strategy for reducing churn.
- Majority of the customer base was middle aged or higher since 75 percent of the customers were 44 years and older.
- 32 percent of the customers left the bank in Germany, so the bank should specifically evaluate their customer services and products to help identify deficiencies and improve their retention rate in Germany.
- The median account balance was slightly higher for customers in Germany. This information can be utilized when forming marketing campaigns or for development of targeted marketing.
- Customers who left the bank had a higher median age and were more likely to be female - this indicates that the bank should focus on improving services for older bank members as well as female bank members.
- With respect to model building and evaluation, the model that performed best (recall score of 74%) was the model that accounted for the class imbalance in the data). - While the default learning rate was adequate, hyperparameter tuning can be used to arrive at a better set of values and to reduce the false negatives further.
- Overall, for the artificial neural network (ANN Model 3) the prediction that the customer will not leave the bank and where the customer actually left the bank was about 5.2%. Further hyperparameter tuning will facilitate reduction of the false negative numbers.

