# Emotion-Detection-6Classes-RF-TFIDF-chatbot

A Natural Language Processing (NLP) project that classifies text into six distinct human emotions: Anger, Fear, Joy, Love, Sadness, and Surprise.

This project implements an end-to-end machine learning pipeline, from data preprocessing to model deployment using a web-based interactive chatbot.

## Features

- Accurate Emotion Prediction: Achieves approximately 88.5% accuracy on test data using a Random Forest classifier.
- Robust Preprocessing Pipeline: Cleans and normalizes text data using stopword removal, lemmatization, and TF-IDF vectorization.
- Multiple ML Models Tested: Evaluation of Logistic Regression, Naive Bayes, and Random Forest models.
- Interactive Web App: A user-friendly Streamlit interface that allows real-time emotion predictions.
- Ready for Deployment: Model and vectorizer are saved as .joblib files, ready for deployment on platforms like Hugging Face Spaces or AWS.

## Dataset

The dataset used in this project is the Emotions Dataset for NLP from Kaggle. It contains over 16,000 labeled sentences, each classified into one of six emotion categories:

- anger
- fear
- joy
- love
- sadness
- surprise

## Getting Started

### Prerequisites

Make sure you have Python 3.11 or higher installed on your system.

## How It Works

1. Text Input: The user enters a sentence in the web interface.
2. Preprocessing: The text is cleaned by removing special characters, stopwords, and applying lemmatization.
3. Feature Extraction: The processed text is converted into numerical features using the saved TF-IDF vectorizer.
4. Prediction: The trained Random Forest model predicts the most likely emotion.
5. Output: The predicted emotion is displayed on the screen in real-time.

## Model Performance

The Random Forest model outperformed other classifiers, achieving the following results on the test set:

- Accuracy: 88.55%
- Weighted F1-Score: 0.89

| Class       | Precision | Recall | F1-Score |
|-------------|-----------|--------|----------|
| Anger       | 0.89      | 0.91   | 0.90     |
| Fear        | 0.84      | 0.88   | 0.86     |
| Joy         | 0.91      | 0.91   | 0.91     |
| Love        | 0.77      | 0.74   | 0.75     |
| Sadness     | 0.94      | 0.92   | 0.93     |
| Surprise    | 0.65      | 0.62   | 0.64     |

Note: The model shows slight confusion between "Sadness" and "Fear", which is a common challenge in emotion recognition.

## Dependencies

All required packages are listed in requirements.txt. Key dependencies include:

- streamlit
- nltk
- scikit-learn
- joblib
- pandas
- numpy

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the issues page if you would like to help.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Author

Fatma Abdullah
