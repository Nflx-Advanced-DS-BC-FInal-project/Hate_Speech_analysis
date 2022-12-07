# Hate_Speech_analysis
#Team Members
Mahederemariam Dagne
Napoleon Davis II

Dataset using Twitter data, is used to research hate-speech detection.  The classifiers utilized in the original dataset  hate speech, offensive, and neither.  Note:  Due to the nature of the study, we wanted prompt the audience that this dataset contains text that can be considered to be vulgar, racist, sexist, homophobic, and/or generally offensive.  

Deleted index columns.
Added cleaned / tokenized tweets column
Tokenization didn’t remove the usernames and retweet tags.
Used regular expressions to remove the usernames and RT tags


Trained and Evaluated Data Model
Naïve Bayes Algorithm
Evaluated individual words
Evaluated phrases with n-grams

Optimization
5_fold_cv_accuracy	Test_accuracy	Data Model				Time_sec
8	0.976	0.975		Tf-idf		PassiveAggressiveClassifier	0.025794
15	0.975	0.976		Hashing		PassiveAggressiveClassifier	0.148768
1	0.973	0.967		BoW			PassiveAggressiveClassifier	0.029578
7	0.973	0.975		BoW			LinearSVC				0.033365
16	0.973	0.973		Hashing		SGDClassifier			0.212212

Conclusion
Best Classification model:  Passive aggressive classifier with tfidf vectorizer
Without stop words performed better than with stop words


Problems and Limitations

Deciding on the best classification model
Methodology in which we approached solution
Time constraints prevented us from further optimization

### FUTURE CONSIDERATIONS
Incorporate twitter API to obtain updated dataset

Pull annual dataset from twitter to analyze hate speech over time
Evaluate using trained model.

Incorporate Multi-label classification model


