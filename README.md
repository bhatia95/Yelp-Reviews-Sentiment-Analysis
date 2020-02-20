# Yelp-Reviews-Sentiment-Analysis
Sentiment classification for Yelp product reviews using Recurrent Neural Networks.
In this project we are developing such an automatic sentiment classifcation system that relies on machine learning techniques to learn from a large set of product reviews provided by Yelp. The levels of polarity of opinion we consider include strong negative, weak negative, neutral, weak positive, and strong positive.

1. Datasets:
- train data.csv: trn id and review text. Contains 650,000 product reviews which acts as the
training data.  
- train label.csv: trn id and sentiment labels. The label set (1,2,3,4,5) refer to -ve polarity lev-
els (strong negative, weak negative, neutral, weak positive, strong and positive) respectively.  
- test data.csv: test id and review text. Contains 50,000 product reviews which acts as the
testing data.    

2. The basic text pre-processing steps include
- Case normalization: Text can contain upper- or lowercase letters. It is a good idea to just
allow either uppercase or lowercase.  
- Tokenization is the process of splitting a stream of text into individual words.  
- Stopwords are words that are extremely common and carry little lexical content. The list
of English stop words can be downloaded from the Internet. For example, a comprehensive
stop-word list can be found from Kevin Bouge's website2.  
- Removing the most/least frequent word: Besides the stopwords, we usually remove words
appearing in more than 95% of the documents and less than 5% of the documents as well.  

3. Parameters for accuracy:
Accuracy = number of correct predictions/number of all predictions  

# Dependencies:
python (>=3.5) - Developed on 3.5. Untested on 2.7, 3.4 or 3.6, but ought to work on v. >=3.5  
pandas (>=0.19) Needed for some data sorting operations  
keras (2.0.2/2.0.3) - Deep learning FTW  
tensorflow (1.0.1) - My preferred Keras backend.  
nltk (>3.4) - word corpus  
