# Hespress-Classifier
Data Preparation: We combined the "stories" data into a single dataframe for easier handling.

Data Cleaning: Useless columns that won't contribute to our use case (e.g., "id") were dropped.

Handling Missing Values: We checked and addressed any missing values in the data.

Label Selection: The label column, "topic," was chosen as our target variable for classification.

Data Balancing Check: We examined the distribution of the label column to ensure the data's balance and lack of bias.

Text Pre-processing: A copy of the dataframe was created, focusing on the "story" column for pre-processing.

NLP Techniques Application: NLP techniques such as removing stopwords, punctuation, non-alphabetic characters, tokenization, and stemming were applied to create a processed corpus.

CountVectorizer Usage: The CountVectorizer library from scikit-learn in Python was utilized to convert the text corpus into a matrix of token counts.

Feature and Label Definition: The processed corpus was used as the X data (features), and the label column was defined as y.

Data Split: The data was split into an 80:20 ratio for training and testing purposes, where 80% of the data was used for training and 20% for testing.

Classifier Selection: The Multinomial Naive Bayes algorithm was chosen as our classifier.

Model Training: The classifier was trained on the X_train and y_train data.

Model Evaluation: The trained model was tested on the X_test data, and the predictions were analyzed to assess its performance.

By following these steps, we developed a Hespress Classifier that can effectively predict the topics of news stories.
