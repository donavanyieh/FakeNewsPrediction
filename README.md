# Classification on real and fake news dataset
#### View the full notebook with outputs here on Kaggle:<br>https://www.kaggle.com/yiehyuheng/true-fake-news-prediction-ensembles-auc

<b>Tech Stack</b><br>
Python (Pandas, NumPy, Matplotlib), NLTK, SpaCy, XGBoost, sklearn models (Logistic Regression, Naive Bayes, SVC, Random Forest ensemble), sklearn metrics (f1 score, ROC curve, ROCAUC score)
<br><br>
<b>Dataset</b><br>
https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset
<br><br>
<b>Note</b><br>
 On evaluation of F1-scores and ROCAUC scores, most models (except for Naive Bayes) gave results close to 98%, which is untypical for normal machine learning models and ensembles. Even deep learning models such as LSTM do not typically give such good results.<br><br> On further investigation, it turns out that the truthful articles were obtained by crawling articles from Reuters, and fake news articles were obtained from unreliable websites flagged by PolitiFact. Since they come from totally different sources, the news articles were extremely skewed, giving rise to unreasonably good results.<br><br>
This emphasises the point of garbage in garbage out when it comes to data analytics/ machine learning tasks. That being said, this general pipeline and evaluation methods should still be transferrable to NLP tasks of similar nature.
