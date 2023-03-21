# Toxic-comment-classification-project
This project is intended to classify toxic comments which are classified as toxic, severe toxic, identity hate, insult, threat and obsence.
The technique used to achieve this classification is the Term frequency- Inverse Document frequency is a numerical statistic that is intended to reflect
how important a word is to a document in a collection or corpus. It is most commonly used in text mining and sentiment analysis major area of its application include
the search engines.

Term frequency
Term frequency, tf(t,d), is the relative frequency of term t within document d,
{\displaystyle \mathrm {tf} (t,d)={\frac {f_{t,d}}{\sum _{t'\in d}{f_{t',d}}}}},
where ft,d is the raw count of a term in a document, i.e., the number of times that term t occurs in document d.

Inverse document frequency
The inverse document frequency is a measure of how much information the word provides, i.e., if it is common or rare across all documents.

Term frequency–inverse document frequency

Then tf–idf is calculated as
{\displaystyle \mathrm {tfidf} (t,d,D)=\mathrm {tf} (t,d)\cdot \mathrm {idf} (t,D)}

A high weight in tf–idf is reached by a high term frequency (in the given document) and a low document frequency of the term in the whole collection of documents; 
the weights hence tend to filter out common terms. Since the ratio inside the idf's log function is always greater than or equal to 1, the value of idf (and tf–idf) 
is greater than or equal to 0.
As a term appears in more documents, the ratio inside the logarithm approaches 1, bringing the idf and tf–idf closer to 0.

Machine Learning approach:
Before applying any ML Model first we had to convert the text into vectors using the TF-IDF, the above stated approach. By actually doing this we would be able to use
linear algebra to work upon and solve our problems. since ML models are based on mathematics. After soing the preliminary steps
of the NLP such as vectorization, lemmatization etc.
We have used classification models such as Logistic Regression and Regression tree also along with bagging and boosting algorithms such as XGBoost
and Light Gradient Boosting. The scoring technique was the f1 score and the model performance was judged on the AUC-ROC curve and score.
