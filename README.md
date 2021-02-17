# Telecom-Churn-UpGrad


###### Problem Statement

*In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of <b>15-25% annual churn rate</b>. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.*

###### Task to Perform
To reduce customer churn, telecom companies need to predict which customers are at high risk of churn.

###### Understandings

There are two main models of payment in the telecom industry 
- postpaid (customers pay a monthly/annual bill after using the services)
- prepaid (customers pay/recharge with a certain amount in advance and then use the services)

***Postpaid***: when customers want to switch to another operator, they usually inform the existing operator to terminate the services, and you directly know that this is an instance of churn.

***Prepaid***: customers who want to switch to another network can simply stop using the services without any notice, and it is hard to know whether someone has actually churned or is simply not using the services temporarily.

#### Step1: Data Exploration and Preparation

# Importing the required library

import numpy as np
import pandas as pd

***Loading Data using pandas***

# Reading the Telecom dataset
telecom = pd.read_csv('./telecom_churn_data.csv')

# Displaying the top few reords
telecom.head()

###### Basic Information

- *Analysing the Dataset about the datatype, columns etc*

telecom.shape

telecom.info(verbose=False)

***Observation:***

- The dataset contains 99,999 rows and 226 columns
- Out of 226 columns 179 float, 35 int and 12 object datatype

### Exploratory Data Analysis

#### Step1: Data Cleaning
