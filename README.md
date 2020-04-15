# Data-mining
This project is from Kaggle Competition. https://www.kaggle.com/c/nlp-getting-started. 
It is a friendly project for data scientists looking to get started with Natural Language Processing.
The competition dataset is not too big, the information in this dataset is easy to understand and deal with.
It is a Text Binary Classification task, which aimed at predicting which Tweets are about real disasters and which ones are not, through the analysis of a dataset of 10,000 tweets.
In this project, I do my project according to the following steps.


1.Basic EDA

This includes analyze the distribution of the target values, the differences of average text length between different targets values, 
the missing values in the data. I also using wordclound display how important words are in a collection of text.
Using wordclound help me to take a quick peek at the word distribution of a collection of texts, clean the texts and I can 
see what are some frequent stopwords that maybe needed to be filtered out, I can see the differences between frequent words
between disaster tweets and non disaster tweets.

2.Text data preprocessing.

Remove Noise(punctuation, HTML,……)

Lowercasing

      Make the same words in different cases can be treated as the same.
      
Remove stop words

      Drop some extremely common words which would appear to be of little value in data analyzing.(Remove the words that are very commonly used in a given language, we can focus on the important words instead.) 
      
Tokenization

     Split an input sequence into tokens. A token can be a word, sentence, paragraph , etc. In this project, I just split sentences into words
     
Token normalization(Lemmatization    Stemming)

      Reduce inflectional forms and sometimes derivationally related forms of a word to a common base form. Eg: (am,are,is->>be)(car,cars,car’s,cars’->>car)
      In this project I use Lemmatization to normalize the token.

3.Text Vectorization.

Bag of words (BOW), TF-IDF. In this project, I compared these two techniques with different classifiers.

4.Build different classification model.

Four traditional model I used in this project.

Logistic Regression 

SVM 

XGBoost 

Naive Bayes

5.Evaluating the perfoemances of different models.

(Matrix: F1 score)

The results show that Naive Bayes with TF-IDF text Vectorization performs best. The score ranks top 45% in this active competition .


