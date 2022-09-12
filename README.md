# Credit_Card_Fraud_Detection

Consumers in 2020 reported losing over $3.3 billion to fraud, an increase of $1.5 billion over the amount reported in 2019. Worldwide, businesses are expected to lose $75 billion to e-commerce fraud from 2019 to 2023. In 2019, the U.S. accounted for 33.57 percent of all gross card fraud losses worldwide.

Credit card fraud represented the second most commonly reported type of identity theft in 2020. In 2020, credit cards were most frequently identified as the payment method in fraud reports. According to Federal Trade Commission, there were over 390k reports of credit card fraud in 2020 and 149M dollars were lost only in the United States. In 2020 the rate of new account credit card fraud attempts rose 48% as compared to 2019.

Thus, in order to stop these frauds we need a powerful fraud detection system that not only detects the fraud but also detects it before it takes place and in an accurate manner.

**The dataset consisted of 1.8 million transactions of 1000 credit cards with 800 merchants**. The variables that fall under all transactions statistics type depict the general card usage profile of the card. The variables under regional statistics type show the region wise spending habits of the card. The variables under merchant statistics type show the usage of the card in different merchant categories. The variables of time based statistics types identify the usage profile of the cards with respect to usage amounts versus time ranges or frequencies of usage versus time ranges.

The basis of credit card fraud detection lies in the analysis of cardholder’s spending behaviour. To study the historical trend, I calculated the daily, weekly and monthly rolling averages of the amount spent by a customer and the number of transactions done.

After the data cleaning and feature engineering step, it was time to apply classification algorithms. **I compared the performance of Logistic regression, Random Forest and Gradient Boosted Trees. Hyperparameter tuning was done for all models with 3-fold cross validation**.

It is important to choose the right model evaluation parameter. Since the dataset was highly imbalanced, I decided to use the area under Precision-Recall curve.
I found the optimal probability threshold by maximizing the F1 score.

Entire project was done using PySpark and SparkSQL.
