# Drug Review Sentiment Analysis with NLP and Deep Learning
## Tools: Python (Pandas, NumPy), Scikit-learn, TensorFlow/Keras, NLTK

In this project, I built a sentiment analysis model using real-world drug review data to classify patient feedback and analyze patterns in medication experiences. The goal was to compare traditional machine learning and deep learning approaches for understanding sentiment in healthcare-related text data.

## Key Steps:

Dataset Preparation: Loaded and cleaned real-world drug review data containing patient reviews, ratings, drug names, and medical conditions. Removed missing values, standardized text fields, and prepared the review data for sentiment classification. Converted patient ratings into sentiment labels to support supervised learning.

### Text Preprocessing:

Cleaned review text by removing unnecessary characters, HTML tags, numbers, and special symbols.

Applied tokenization, lowercasing, stopword removal, and lemmatization to standardize the text and reduce noise.

Prepared text data differently for machine learning and deep learning models, including feature extraction for traditional models and sequence padding for neural network models.

### Exploratory Data Analysis:

Analyzed the distribution of sentiment labels across the drug review dataset.

Examined common patterns in patient feedback to understand how review language differs across positive and negative experiences.

Reviewed rating and sentiment distributions to identify class imbalance and better understand the structure of the dataset.

### Machine Learning Baseline:

Built a Naive Bayes baseline model to classify drug reviews based on processed text features.

Evaluated the baseline model using accuracy, precision, recall, and F1-score.

The Naive Bayes model achieved approximately 77.9% accuracy, providing a strong comparison point for the deep learning models.

### Deep Learning Model Development:

Implemented multiple deep learning models for sentiment classification, including CNN, LSTM, and a CNN-LSTM hybrid model.

Used tokenized and padded text sequences as input for neural network models.

Compared model performance to determine which architecture handled drug review sentiment classification most effectively.

### Model Evaluation:

Evaluated each model using accuracy, precision, recall, and F1-score.

Compared traditional machine learning results with deep learning performance to understand the strengths and weaknesses of each approach.

The CNN model performed strongest among the deep learning models, reaching approximately 90% accuracy.

### Key Takeaways:

NLP and deep learning can be used to analyze large-scale patient reviews and classify medication-related sentiment more efficiently than manual review.

The Naive Bayes baseline performed reasonably well with approximately 77.9% accuracy, showing that traditional machine learning can still be effective for text classification tasks.

The CNN model achieved the strongest performance among the deep learning approaches, reaching approximately 90% accuracy.

CNN performed better than the LSTM and CNN-LSTM hybrid models because many drug reviews contain strong local word patterns and short sentiment phrases that CNNs can capture effectively.

The CNN-LSTM hybrid did not outperform the CNN, likely because the added model complexity did not provide enough benefit for this dataset and may have increased the risk of overfitting.

Patient drug reviews contain meaningful patterns about medication experiences, side effects, and satisfaction, showing that NLP can support healthcare-related text analysis.
