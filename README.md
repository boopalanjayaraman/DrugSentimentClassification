# Drug Sentiment Classification
Drug Sentiment Classification - uses dataset from Innoplexus hackathon from Analytics Vidhya.

This was not submitted to the contest because it was done after the contest ended. And hence, contains only the accuracy / f1 score for cross validation data.

Code uses pre-trained BERT model. Was developed using Google colab. 

Preprocessing done: Tokenization using BERT vocabulary, Choosing only the sentences where the drug name is specified (one sentence and one after), Removing common stop words, but keeping certain negative polarity stop words, Removing other types of stop words (months, days, numeric), removing special characters and URLs, Undersampling / oversampling for classes (imbalanced data set), padding for smaller sentences, one-hot encoding for labels.

Training vs Cross validation split: 20%, Maximum number of tokens for each sample: 256, Batch size: 16. 

BERT learning rate (recommended value): 0.00001. Number of epochs: 10-15. (Sample may differ).
