A spam detector built using Python.

Libraries used :

NumPy
Pandas
MatPlotLib
nltk
seaborn
string
wordcloud
collections
sklearn
The first step was to analyse the data.

![image](https://user-images.githubusercontent.com/84259885/214381205-927808cf-ef72-4b2c-b1e7-10494f9661da.png)
The above figure shows the percentage of data that is spam.

Next step was to calculate the no. of words and characters in each message. Next step was to analyze the no of characters/words to the category of the data.
![image](https://user-images.githubusercontent.com/84259885/214381347-fc638dad-32a4-44f4-a6b1-ff990aafcc6d.png)
![image](https://user-images.githubusercontent.com/84259885/214381369-a1272899-5028-41a1-ba25-38d97156672a.png)

The next step was to use Porter Stemmer on the messages.

The next step was to find out the most occuring words in spam and ham messages.
![image](https://user-images.githubusercontent.com/84259885/214381414-c628f9ac-dc57-4889-ab15-69f6aca5d457.png)
![image](https://user-images.githubusercontent.com/84259885/214381437-0669984d-b52f-4b7b-8cf9-d1a807608243.png)

The next step was to transform the data using tf.idf vectorizer

The last step was to apply the Multinomial Naive Bayes ML algorithm. ( It had the best performance among many other ML agorithms tested)

CONFUSION MATRIX [[896 0] [ 30 108]]

CLASSSIFICATION REPORT precision recall f1-score support

       0       0.97      1.00      0.98       896
       1       1.00      0.78      0.88       138

accuracy                           0.97      1034

macro avg 0.98 0.89 0.93 1034 weighted avg 0.97 0.97 0.97 1034

The above is the result.
