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
First the data type of Total Charges feature column is changed from objecct to float type.
Then the null and NaN values are detecting in the dataset. There were 10 NULL values in Total Charges Column so we use Simple Imputer Class of Sckit Learn Package
to impute the NULL values with mean of the remaining data from the column Total Charges. This efectively takes cake of the NULL values.
#### Encoding Categorical Data
Binary features are encoded using Label Encoding that is Yes = 1 and No = 0 etc.
Nominal Features that features having more that 2 categorical values are encoded using One Hot Encoding Method. 
Finally we get 41 columns in feature matrix.
#### Train Test Split
The dataset is splitted into 4 numpy arrays x_train, y_train, x_test, y_test where Training arrays have 80% of the total data present in the dataset and rest 20% is used for testing.

### Training the Model
The Model is then trained on differnt Machine Learning Models to predict the class of the Churn depending upon the input. 
We save the predicted data in a numpy array y_pred.

### Testing the Model
The y_pred is compared with the y_test array and an accuracy is estimated based on this comparision.

### K-Fold Cross Validation
Cross validation od the training accuracies is performed and their mean is calculated as well as Standard Deviation between accuracies is calculated.

### Hyperparameters
All the parameters of the attributes are tested to get the best model parameters.

### Visualising Results
Yet to be Completed!
