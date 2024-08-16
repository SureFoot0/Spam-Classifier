# Spam-Classifier

Text_Emails.csv was downloaded from: https://www.kaggle.com/datasets/purusinghvi/email-spam-classification-dataset
Wordcount_Emails.csv was downloaded from: https://www.kaggle.com/datasets/balaka18/email-spam-classification-dataset-csv?select=emails.csv

Method (so far):

	1) Set the main DataFrame (df) to the Wordcount_Emails.csv file because there are 3000 lemmatised words we can use.

	2) Clean df by removing everything except the column headers (lemmatised words)

	3) PrepNewData function to take new data and get the frequency of each token in an input text

	4) Use PrepNewData to fit Text_Emails.csv into an appropriate format.

	5) Fit training and testing data to a SVC

To do:

	1) Implement TF-IDF for improved training and testing data (between step 4 and 5)

	2) Save completed model (after step 5)

Improvements:

	1) Find a dataframe specifically for lots of lemmatised words instead of using Wordcount_Emails.csv

	2) Clean up notebook,

Definitions:

	Appropriate format: Columns: 3000 lemmatised words from Wordcount_Emails.csv

	TF-IDF equation: For text t in document d, tf-idf(t, d) = tf(t, d) * idf(t) where idf(t) = log [ n / df(t) ] + 1 More found here: https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfTransformer.html
	
	SVC: A specific class of the Support Vector Machine (SVM) specifically designed for classification
