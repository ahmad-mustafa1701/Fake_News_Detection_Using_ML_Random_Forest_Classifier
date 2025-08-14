Fake News Detection Using Machine Learning (Random Forest Classifier)
📌 Overview

This project is aimed at detecting fake news articles using Machine Learning with a Random Forest Classifier. It uses spaCy for text preprocessing, TF-IDF Vectorization for feature extraction, and 5-fold cross-validation for robust model evaluation. The goal is to create a reliable tool for identifying misinformation in news content.

📂 Dataset
The original dataset contains 44,921 news articles:

True News – 21,418 entries

Fake News – 23,503 entries

Original Columns:

title – headline of the news

text – body content of the article

subject – category or topic of the news

date – date of publication

label/index – classification (1 = Fake, 0 = Real)

Note: For demonstration and faster training, only 250 fake news and 250 true news records were used, resulting in a dataset of 500 articles.

🛠 Preprocessing

Text preprocessing is done using the spaCy library:

Lowercasing text

Tokenization – breaking text into words

Stopword Removal – removing common but uninformative words

Punctuation Removal

Lemmatization – converting words to their base form

📊 Feature Extraction

We use TF-IDF (Term Frequency – Inverse Document Frequency) to convert the processed text into numerical feature vectors.

Maximum features: 5000

Removes common and rarely used words to improve model performance

🤖 Model

Algorithm: Random Forest Classifier

Evaluation: k=5 Fold Cross-Validation

Reason: Random Forest handles high-dimensional data well and reduces overfitting through ensemble learning.

📈 Results

Model performance is evaluated using metrics:

Accuracy

Precision

Recall

F1-score

Average accuracy achieved during 5-fold cross-validation is around 99.80%.
