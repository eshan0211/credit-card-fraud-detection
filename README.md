# credit-card-fraud-detection
(Full report - PDC_report.pdf)

### INTRODUCTION
A credit card is a thin handy plastic card that contains identification information such as a signature or picture, and authorizes the person named on it to charge purchases or services to his account - charges for which he will be billed periodically. Today, the information on the card is read by automated teller machines (ATMs), store readers, bank and is also used in online internet banking system. They have a unique card number which is of utmost importance. Its security relies on the physical security of the plastic card as well as the privacy of the credit card number.

### IMPLEMENTATION DETAILS:

This project can be divided into four parts for implementation:

•	Exploratory Data Analysis and Visualization using threads
• Plotting using threads
•	Training Single Neural Network using Data Parallelism among threads
•	Training Multiple Neural Networks using Functional Parallelism among threads

For all the above tasks, implementation has been achieved using Python Programming Language and threads architecture available in python under the _threads library.

The dataset that we have used in this project is a credit card fraudulent dataset available at the following link:
[https://www.kaggle.com/mlg-ulb/creditcardfraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)

The dataset consists of 31 columns, which represents the various features of over 2 lakh credit card users and a target variable indicating whether they are fraud or not.

A glimpse of the dataset has been shown below:
![image](https://user-images.githubusercontent.com/61506157/146679163-2c81f6f5-7883-4ffc-8338-e3d26d8e5919.png)


All the variables in the dataset are associated with the real time data of the credit card users. However due to user privacy policy the names of these variables are not disclosed.

### CONCLUSION

As usage of credit cards become more and more common in every field of the daily life, credit card fraud has become much more rampant. To improve security of the financial transaction systems in an automatic and effective way, building an accurate and efficient credit card fraud detection system is one of the key tasks for the financial institutions. In this study, 13 classification methods were used to build fraud detecting models. The work demonstrates the advantages of applying the data mining techniques including ANN and LR to the credit card fraud detection problem for the purpose of reducing the bank’s risk. The results show that the proposed LR classifiers outperform ANN classifiers in solving the problem under investigation. However, as the distribution of the training data sets become more biased, the performance of all models decrease in catching the fraudulent transactions. The accuracy observed by Logistic Regressor Classifier was 99.85 and accuracy observed by Artificial Neural Network was 94.5. The reason for this maximum accuracy was the dataset. It contained minimal fraud values compared to the large non-fraud values. As by visualisation, we observed there were 284315 non-fraud values compared to just 492 fraud values.


We have also tested our models to some of the test values and it results in desired output. The fact that we have used parallelism in our training models helped us in training the models faster. Also, we had an insight on how the threads work, how the hyperparameters work and what is the ideal amount of parallelism that should be applied in order to achieve maximum efficiency. Since our dataset contained 31 columns, parallelism that we used in visualising the dataset helped us to reduce time of compilation and helped us to visualise more number of plots concurrently thus saving the time providing with desired outputs. All results have been obtained with a unique data set, comprising all transactions managed during two years by a major Spanish bank and including more than 180 million operations. 

