# Predicting Customer Churn in Telecommunication using Data Mining Techniques

## Dataset Source : 
https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113

### Dataset Description:
*Each row represents a customer, each column contains customer’s attributes described on the column Metadata.

*The data set includes information about:

*Customers who left within the last month – the column is called Churn

*Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies

*Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges

*Demographic info about customers – gender, age range, and if they have partners and dependents

## Inspiration
To explore this type of models and learn more about the subject.

## Project Description
All the standard steps of Knowledge Discovery that is Selection, Preprocessing, Transformation, Training and Evaluation have been used in this project.
First the standard Pyhton Machine Learning libraries are imported eg. numpy, pandas, etc.
The dataset is stored as a pandas DataFrame reffered by variable dataset.

### Data Cleaning
CustomerID column is droped as it does not contribute to the result of Churn.

DataFrame currently has 1 float, 2 int and 17 object type. In order to implement the Machine Learning Models we need to have all the features as numeric datatype.

### Data Visualisation
All the features are plotted against Churn to find interesting patterns int the dataset.
for eg. Customers Having Internet Service of type fibre optics are more likely to Churn than Customers with No Internet Service.

### Data Preprocessing

