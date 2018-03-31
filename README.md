### **Description:** The main purpose of this project is to predict the Passenger survived or not from Titanic disaster.


* Step-1: Download dataset from [https://www.kaggle.com/c/titanic/data](https://www.kaggle.com/c/titanic/data), store it in dataframe. 
* Step-2: Check for the columns which contain null values and apply feature engineering techniques as stated below:
     * Calculate mean of age separately for male and female and substitue it in places were null value occurs.
     * Calculate mean of fares and substitue it in places were null value occurs.
     * Replace null values of Embarked as S as that occurs the most.
* Step-3: We will drop Passenger ID, Name, Cabin and Ticket from Train and Test Dataset.
* Step-4: Next we need to convert the columns Sex and Embarked into numbers. We will do it with One Hot Encoding except reduce one categorical level to reduce number of columns.
* Step-5: Lets do some more feature Engineering:
     * Remove Outliers.
     * Create age groups fare groups and assign them numbers and create new columns of the same and drop fare and age.
* Step-6: Now that we our done with feature engineering and data is ready to be fed to the model lets try some ML algorithm and see which is the best
* Step-7: Create a dataframe with PassengerID and Survived value predicted for the test dataset using the ML algorithm which gives the best accuracy score to submit predicted value into required submission format


# Conclusion

* The  Algorithm gives the best accuracy is Decision Tree with 90.32% for the given dataset.

|       Algorithm       | Accuracy |
|:----------------------|:--------:|
|     Decision Tree     |  90.32%  |
|     Random Forest     |  89.75%  |      
|          KNN          |  85.59%  |
|Support Vector Machine |  83.22%  |
|  Logistic Regression  |  80.41%  |      
|      Naive Bayes      |  78.04%  |
