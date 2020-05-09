# Credit-Card-Fraud-Detection
Steps:
1.Import the dataset we will be using for this project named ‘CreditCard.csv’ which is in the csv format.
2.Run all the commands in the CreditCardFraudDetectio.ipynb file

Description of Project:
In the implementation phase first we import various libraries from Python which is our chosen language for this project. 
Jupyter notebook is the platform on which the coding part was done.The libraries are numpy, pandas, seaborn, matplotlib and sklearn in which each provide a specific role for the calculation of the results.We import the dataset we will be using for this project named ‘CreditCard,csv’ which is in the csv format (here CSV stands for Comma separated values) because csv formats take less time to be processed on. 
After importing the data we next describe the data using describe() method for the value of the class attribute.
(In this case which is the attribute defining if the transaction we are testing out is a fraud one or not) to be equal to one, i.e the transaction is fraud.
Next, Scaling of the data in the given dataset is done using StandardScalar() and reshape(-1,1) method.
NumPy provides the reshape() function on the NumPy array object that can be used to reshape the data.
Now, the attributes are split as input data and target output. 
Target output is a class value which determines whether transaction is fraud or not.
Further, data is split into three parts training data, testing data and some data is kept for it to be used during future prediction. 
Training data is used to train the model and then model is tested against test data to predict the accuracy of the model.
The first algorithm we apply is the Decision tree Classifier algorithm in which the model is trained for the training dataset using the information gain method. 
Then we use fit() method to train the model using these values and predict the data using this classifier.
Decision Tree Classifier that the results obtained had a huge gap and the accuracy would be low for every transaction. 
So we apply feature selection to it using the Gini Importance algorithm in which we determine that some transactions wouldn’t be of great importance to us for providing results.
Again, we apply the DecisionTreeClassifier() for determining the results for the fraud transactions and obtain the prediction using the same split of data.
 Next, we apply RandomForestClassifier() on the same dataset and on the data obtained after feature selection after applying the DecisionTreeClassifier().

