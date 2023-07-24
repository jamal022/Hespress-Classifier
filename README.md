# Hespress-Classifier
- Data Preparation: I concatenated the "stories" data into a single dataframe for easier handling.

- Data Cleaning: I dropped useless columns that won't contribute to my use case (e.g., "id").

- Handling Missing Values: I checked and addressed any missing values in the data.

- Label Selection: The label column, "topic," was chosen as my target variable for classification.

- Data Balancing Check: I examined the distribution of the label column to ensure the data's balance and lack of bias.

- Text Pre-processing: I created a copy of the dataframe, focusing on the "story" column for pre-processing.

- NLP Techniques Application: I applied NLP techniques such as removing stopwords, punctuation, non-alphabetic characters, tokenization, and stemming to create a processed corpus.

- CountVectorizer Usage: I utilized the CountVectorizer library from scikit-learn in Python to convert the text corpus into a matrix of token counts.

- Feature and Label Definition: The processed corpus was used as the X data (features), and the label column was defined as y.

- Data Split: The data was split into an 80:20 ratio for training and testing purposes, where 80% of the data was used for training and 20% for testing.

- Classifier Selection: I chose the Multinomial Naive Bayes algorithm as my classifier.

- Model Training: I trained the classifier on the X_train and y_train data.

- Model Evaluation: I tested the trained model on the X_test data, and I analyzed the predictions to assess its performance.

By following these steps, I developed a Hespress Classifier that can effectively predict the topics of news stories.
