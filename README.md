# TechnoHacks_Movie_Reviews_Classification
The project demonstrates the process of building a sentiment analysis model for movie reviews using NLP techniques. It covers data preprocessing, feature extraction, model selection, hyperparameter tuning, and model evaluation. The goal is to accurately classify movie reviews as positive or negative based on their textual content, which can be useful in various applications, such as opinion mining and recommendation systems.

# Key Components and steps 

Data Loading and Understanding:

The project starts by loading labeled movie review data from two files: 'labeledTrainData.tsv' and 'testData.tsv.' These datasets contain movie reviews, along with sentiment labels (0 for negative and 1 for positive).
Data Preprocessing:

Text data preprocessing is a critical step in NLP tasks. The following preprocessing steps are applied to the movie reviews:
Conversion to lowercase: All text is converted to lowercase to ensure consistency.
Removal of non-alphabetic characters: Non-alphabetic characters, such as punctuation and numbers, are removed from the text.
Removal of stopwords: Common English stopwords (e.g., "the," "and," "in") are removed from the text to reduce noise.
Feature Extraction:

The text data is transformed into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. TF-IDF assigns a numerical value to each word in the text based on its frequency in the document and its importance in the entire corpus.
Model Building and Hyperparameter Tuning:

In this project, two machine learning models are considered: Logistic Regression and Random Forest.
Hyperparameter tuning is performed using techniques like GridSearchCV to find the best combination of hyperparameters for the chosen model (e.g., 'C' for logistic regression or various parameters for random forest).
Model Evaluation:

The performance of the model is assessed using cross-validation, which provides an estimate of how well the model will generalize to unseen data.
Evaluation metrics such as accuracy, confusion matrix, and classification report are used to measure model performance.
Sentiment Classification:

After training and evaluating the model on the labeled data, the model is used to predict sentiment labels (positive or negative) for unlabeled movie reviews from the 'testData.tsv' file.
Results Presentation:

The predicted sentiment labels for the test reviews are stored in a DataFrame, and the results are presented, including the first few rows of the test predictions.
