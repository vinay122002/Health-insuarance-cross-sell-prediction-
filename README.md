# HEALTH INSURANCE CROSS SELL PREDICTION
Predicting whether a customer would be interested in buying Vehicle Insurance so that the company can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.


---

## Table of Content
  * [Abstract](#abstract)
  * [Problem Statement](#problem-statement)
  * [Data Description](#data-description)
  * [Conclusion](#conclusion)
  * [Reference](#reference)

---



# Abstract
An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. There are multiple factors that play a major role in capturing customers for any insurance policy. Here we have information about demographics such as age, gender, region code, and vehicle damage, vehicle age, annual premium, policy sourcing channel.
Based on the previous trend, this data analysis and prediction with machine learning models can help us understand what are the reasons for news popularity on social media and obtain the best classification model.

# Problem Statement
Our client is an Insurance company that has provided Health Insurance to its customers. Now they need the help in building a model to predict whether the policyholders (customers) from the past year will also be interested in Vehicle Insurance provided by the company.

An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee.

*Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimize its business model and revenue.*


# Data Description
We have a dataset which contains information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc. related to a person who is interested in vehicle insurance.
We have 381109 data points available.


| Feature Name | Type | Description |
|----|----|----|
|id| (continous) |Unique identifier for the Customer.|
|Age |(continous)| Age of the Customer.|
|Gender |(dichotomous)|Gender of the Custome|
|Driving_License |(dichotomous)|0 for customer not having DL, 1 for customer having DL.|
|Region_Code |(nominal)|Unique code for the region of the customer.|
|Previously_Insured| (dichotomous)| 0 for customer not having vehicle insurance, 1 for customer having vehicle insurance.|
|Vehicle_Age| (nominal)| Age of the vehicle.|
|Vehicle_Damage | (dichotomous)| Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.|
|Annual_Premium| (continous)| The amount customer needs to pay as premium in the year.|
|Policy_Sales_Channel| (nominal)| Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.|
|Vintage |(continous)|Number of Days, Customer has been associated with the company.|
|**Response** (Dependent Feature)|(dichotomous)| 1 for Customer is interested, 0 for Customer is not interested.|


----

# Conclusion
Starting from loading our dataset, we firstly performed data cleaning and refactoring by outlier detection and normalization of data. Then we covered  EDA, feature selection and algorithm selection, and hyperparameter tuning.
The Accuracy score obtained for all models was in the range of 68% to 85% before tuning
After tuning the models we were able to get an accuracy of approx 87%. But we selected our best model as the model with an accuracy score of 85% considering precision and recall as we have an unequal number of observations in each class in our dataset, so accuracy alone can be misleading.





---
Here is a glimpse of few graphs we plotted, there are many more in the notebook please have a look.
![image](https://user-images.githubusercontent.com/35359451/136075191-a409b7a4-adf9-4950-ba79-489cb91cba69.png)|![image](https://user-images.githubusercontent.com/35359451/136075288-2879d356-8b14-4d45-9ab1-9a95e892434b.png)|![image](https://user-images.githubusercontent.com/35359451/136075349-a59d1d2a-b19a-4155-a372-077d680905ed.png)|
:-------------------------:|:-------------------------:|:-------------------------:
![image](https://user-images.githubusercontent.com/35359451/136075430-09139077-575b-444c-9bbf-fe352aac1d60.png)|![image](https://user-images.githubusercontent.com/35359451/136075516-ac13173a-9a79-4477-9f4f-f24fd3a49cba.png)|![image](https://user-images.githubusercontent.com/35359451/136076533-4c3d8e4b-ce04-4d9c-942c-38ad1b31d006.png)|
![image](https://user-images.githubusercontent.com/35359451/136076076-b7616323-5020-4646-b4a9-6e12d149fda8.png)|![image](https://user-images.githubusercontent.com/35359451/136076150-7e78971f-e134-401e-8b97-97aae61cfa46.png)|![image](https://user-images.githubusercontent.com/35359451/136076259-ffef7f15-8b6b-4230-a1c5-8e697ce06c50.png)|



---
# References
 - https://towardsdatascience.com
 - https://www.analyticsvidhya.com
 - https://machinelearningmastery.com


---
