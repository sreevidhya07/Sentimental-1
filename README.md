Sentiment Analysis Using Machine Learning and NLP

📌 Project Overview

This project implements a Sentiment Analysis System using Machine Learning and Natural Language Processing (NLP) to classify text into three sentiment categories:

- Positive – Expresses happiness, satisfaction, or a favorable opinion.
- Negative – Expresses dissatisfaction, disappointment, or an unfavorable opinion.
- Neutral – Contains factual information without an obvious positive or negative opinion.

The system uses TF-IDF Vectorization to convert text into numerical features and Logistic Regression to predict sentiment. It also evaluates the model's performance and displays a confusion matrix.

🎯 Objectives

- Understand the basics of Natural Language Processing.
- Perform text preprocessing and cleaning.
- Convert textual data into numerical features using TF-IDF.
- Train a Machine Learning classification model.
- Evaluate model performance using accuracy and a classification report.
- Visualize predictions using a confusion matrix.
- Predict the sentiment of user-provided text.

🛠️ Technologies Used

- Programming Language: Python
- Data Processing: Pandas
- Text Preprocessing: Regular Expressions ("re")
- Machine Learning: Scikit-learn
- Feature Extraction: TF-IDF Vectorizer
- Classification Algorithm: Logistic Regression
- Data Visualization: Matplotlib

📂 Project Structure

sentiment-analysis-nlp/
│
├── sentiment_analysis.py
├── README.md
└── requirements.txt

📊 Dataset

The project uses a sample dataset containing 36 text examples.

Sentiment| Number of Examples
Positive| 12
Negative| 12
Neutral| 12
Total| 36

The dataset is created directly in the Python program using Pandas, so no external dataset download is required.

Example Data

Text| Sentiment
I love this product| Positive
The service is very bad| Negative
The package contains two items| Neutral

⚙️ How It Works

1. Dataset Creation

A sample dataset is created with text sentences and their corresponding sentiment labels.

2. Text Preprocessing

The text is cleaned using a custom function that:

- Converts all text to lowercase.
- Removes numbers and special characters.
- Removes extra spaces.

3. Train-Test Split

The dataset is divided into:

- 75% training data
- 25% testing data

Stratified splitting maintains the proportion of sentiment classes in both sets.

4. Feature Extraction

"TfidfVectorizer" converts text into numerical features based on word importance. The model uses both individual words and two-word combinations through "ngram_range=(1, 2)".

5. Model Training

Logistic Regression learns patterns from the training data and uses them to classify text into Positive, Negative, or Neutral categories.

6. Model Evaluation

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

7. Sentiment Prediction

The program predicts the sentiment of new sentences and displays the predicted class and estimated class probabilities.

📦 Installation

Prerequisites

Install Python 3.9 or later and ensure that Python and pip are available on your system.

Step 1: Clone the Repository

git clone <your-repository-url>
cd sentiment-analysis-nlp

Replace "<your-repository-url>" with your actual GitHub repository URL.

Step 2: Install Dependencies

pip install -r requirements.txt

Alternatively, install the packages directly:

pip install pandas scikit-learn matplotlib

▶️ How to Run

Run the Python program from your terminal:

python sentiment_analysis.py

The program will:

1. Display a preview of the dataset.
2. Show the distribution of sentiment classes.
3. Train the Machine Learning model.
4. Print evaluation metrics.
5. Display the confusion matrix.
6. Predict sentiment for sample sentences.
7. Ask you to enter your own sentence for analysis.

💻 Example Usage

Input

I really love this amazing product

Possible Output

Input text: I really love this amazing product
Predicted sentiment: Positive

Class probabilities:
Negative: ...
Neutral: ...
Positive: ...

The exact prediction and probabilities depend on the training data and the trained model.

You can also enter your own sentence:

Enter a review or sentence: The product is very disappointing

The program will display the predicted sentiment and the estimated probabilities for all three classes.

📈 Evaluation Metrics

Accuracy: Measures the proportion of correctly classified test examples.

Precision: Measures how many predictions for a particular class are correct.

Recall: Measures how many actual examples of a particular class are correctly identified.

F1-score: Combines precision and recall into a single metric.

Confusion Matrix: Shows the actual versus predicted sentiment classes, helping identify classification errors.

«Note: The dataset is small and contains simple, predefined sentences. Evaluation results may vary depending on the train-test split. High accuracy on this sample dataset does not guarantee good performance on real-world reviews.»

📋 Requirements

Create a file named "requirements.txt" with the following contents:

pandas
scikit-learn
matplotlib

The "re" module is part of Python's standard library and does not need to be installed separately.

🚀 Future Improvements

- Use a larger, real-world sentiment dataset.
- Apply advanced text preprocessing and lemmatization.
- Compare Logistic Regression with Naive Bayes and Support Vector Machines.
- Add a graphical user interface using Streamlit.
- Develop a web application for real-time sentiment analysis.
- Support multiple languages.
- Improve handling of negation, sarcasm, and context.

🎓 Learning Outcomes

This project demonstrates the practical application of:

- Natural Language Processing.
- Text preprocessing and feature extraction.
- Supervised Machine Learning.
- Multi-class text classification.
- Model evaluation and visualization.
- Real-time prediction for user-provided text.

👨‍💻 Author

Developed as a Machine Learning and NLP project to explore text classification and sentiment analysis.

📄 License

This project is available for educational and learning purposes. Add an appropriate open-source license if you plan to distribute it publicly.
