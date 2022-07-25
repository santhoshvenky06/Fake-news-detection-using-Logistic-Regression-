# Fake-news-detection-using-Logistic-Regression-
This project is a **fake news detection Machine Learning model** built using the **Logistic Regression algorithm**. I started with downloading the dataset from Kaggle. You can use the following link: 
**https://www.kaggle.com/c/fake-news/data?select=train.csv**


I read the data file and checked the distribution of Fake and Genuine news in the dataset. Fake news is represented by 0's and genuine news is represented by 1's under the label column. 

I then check for NULL values in the data set and fill the null values with a space ' '. Because the text column would be tedious and time consuming to be used as a feature, I decided to use the content and author data labels as features. To make this easier, I combined both of it into a single datalabel **content**. 

I then divide the data set into my dependant and independant features (X & Y respectively).

I then implement the **PorterStemmer()** function. Stemming is the process of reducing words down to its parent/root word. The stemming process is applied to all the words in the content label and stored. 

The vectorizer function is used to convert the character strings into vectors. 

I then apply the infamous **train, test, split and the LogisticRegression()** algorithm and trained the model using my training data. Checking the accuracy score, I was able to acheive an accuracy score of 98% approximately. However, I believe using the **Long term- short term memory networks (LSTM) , a variation of thr RNN,** I will be able to achieve a higher accuracy score. 

On testing my model using the testing data, I was able to achieve desirable predictions. 
