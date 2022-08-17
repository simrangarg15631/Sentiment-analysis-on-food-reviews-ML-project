# Sentiment-analysis-on-food-reviews-ML-project
The project uses Machine learning model to analyse the food reviews and predict whether the review is positive or negative. The message is displayed on a Tkinter window.

Sentiment analysis deals with the process of computationally identifying and categorizing opinions expressed in a piece of text, especially in order to determine whether the writer’s attitude toward a particular topic is positive or negative.Knowing the opinion of customers is very important for any business. It is expensive to check each and every review manually and label its sentiment. So, a better way is to rely on machine learning models for that.

Hence, in this project, we analyze the reviews given by the customers of the restaurant with the help of Machine Learning Classification algorithm. This project mainly focuses on the implementation of various classification algorithms and their performance analysis. The simulation results showed that Logistic Regression resulted in the highest accuracy of 82 % for the given dataset. 

i. Python libraries we have used in our project are:
  1. pandas
  2. Numpy
  3. Re
  4. Tkinter
  5. Sklearn

ii. About Data set

The data set consists of 1000 reviews of fine foods. It contains 500 positive and 500 negative reviews. It is saved in a tsv (tab separated value) file. It is read using read_csv() function of Pandas.

We have the following columns:

1. Review: Review about the product

2. Liked: 0 or 1, 0 for negative review and 1 for positive review

iii. Objective

Given a review, determine whether the review is positive (1) or negative (0).

iv. Preprocessing text data

Text data requires some preprocessing before we go on further with analysis and making the prediction model. Hence in the preprocessing phase, we do the following in the order below:-

• Begin by removing the Html tags.

• Replace abbreviations.

• Remove contact number.

• Remove any punctuations, special characters and numbers.

• Replace more than one space with single space. 

• Finally, convert data to lowercase.

v. Train test split

Once we are done with preprocessing, we will split our data into train and test. 80% of the data is used for training the model and 20% of the data is used for testing the model.

vi. Vectorizing text data

After that, I have applied Count Vectorizer technique for featuring our text and saved them as separate vectors.

vii. Machine learning Approach: Logistic regression

As our dataset is labelled, we have to use a Supervised learning approach. Our model predicts discrete output values, that’s why we are using Classification algorithm. We have used Logistic Regression classification algorithm as it gives highest accuracy for the given dataset. We have also tried to train the models using SVM and Decision Trees but their accuracy was low as compared to Logistic Regression.

• Accuracy of Logistic Regression – 82%

• Accuracy of SVM – 79%

• Accuracy of Decision Trees – 16%

viii. Save the Model

Our model is saved in a pkl file using pickle package which is then passed to our GUI.

ix. GUI Window using Tkinter

Our project consists of a GUI window which takes review as input from the user and then drops a message box telling us whether the customer is satisfied or not
