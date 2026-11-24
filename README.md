# SMS Spam Detection

A Streamlit application that uses a Logistic Regression model to classify SMS messages as **spam** or **ham** (legitimate).

## Live Demo

Try the deployed application: [SMS Spam Detection](https://logisticregressionmodelforspamdetection-nyy4fccmdlh35q6jbdyydm.streamlit.app)

## Features

- Enter an SMS message through a web interface
- Preprocess text by removing special characters and numbers, removing English stopwords, and applying lemmatization
- Convert text into numerical features using TF-IDF
- Predict whether the message is spam or ham using Logistic Regression

## Project Structure

- `app.py` - Streamlit application and SMS classification logic
- `logistic_regression_sms_spam_model.pkl` - Trained Logistic Regression model
- `tfidf_vectorizer.pkl` - Fitted TF-IDF vectorizer
- `label_encoder.pkl` - Fitted label encoder
- `spam.csv` - SMS dataset used by the project
- `requirements.txt` - Python dependencies

## Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/kavyajeergi/Logistic_Regression_Model_For_Spam_Detection.git
cd Logistic_Regression_Model_For_Spam_Detection
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Start the application

```bash
streamlit run app.py
```

The app will open in your browser, usually at `http://localhost:8501`.

## Technologies Used

- Python
- Streamlit
- Scikit-learn
- NLTK
- Joblib
- Pandas
- NumPy

## Model Pipeline

1. Clean the input message
2. Tokenize the text
3. Remove English stopwords
4. Apply lemmatization
5. Transform text with TF-IDF
6. Classify the message with Logistic Regression
