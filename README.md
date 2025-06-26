# 📧 Email/SMS Spam Classifier

This is a **machine learning-based spam detection system** built with **Python** and **Streamlit**. It classifies input text messages (emails or SMS) as either **Spam** or **Not Spam** using natural language processing (NLP) and a **Multinomial Naive Bayes** model trained on a labeled dataset.

---

## 🚀 Features

- 🧠 Predicts whether a message is **Spam** or **Not Spam**
- ✂️ Applies **NLP preprocessing** (tokenization, stopword removal, stemming)
- 📊 Uses **TF-IDF vectorization** and **Naive Bayes** classifier
- ⚡️ Loads pre-trained model and vectorizer for fast predictions
- 🎨 Clean and interactive UI built with **Streamlit**

---

## 🛠️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/vjy-07/Email-SMS-Spam-Classifier.git
cd Email-SMS-Spam-Classifier
```
### 2. (Optional) Create a Virtual Environment

```bash
python -m venv venv

# On macOS/Linux
source venv/bin/activate

# On Windows
venv\Scripts\activate
```
### 3. Install Dependencies

```bash
pip install -r requirements.txt
```
### 5. Run the App

```bash
streamlit run app.py
```

## 📁 Project Structure

```text
Email-SMS-Spam-Classifier/
│
├── app.py                    # Main Streamlit app
├── requirements.txt          # List of Python dependencies
├── model.pkl                 # Trained Naive Bayes model
├── vectorizer.pkl            # TF-IDF vectorizer
```
## 🧠 How It Works

1. **User Input**: The user enters an email or SMS message into the text box.
2. **Text Preprocessing**: The message is cleaned and processed using:
   - Lowercasing and tokenization
   - Removal of stopwords and punctuation
   - Stemming using `PorterStemmer`
3. **Vectorization**: The cleaned text is converted into numerical features using a **TF-IDF vectorizer**.
4. **Prediction**: The processed input is passed to a **Multinomial Naive Bayes** model to predict whether it is spam.
5. **Output**: The result is displayed as **Spam** or **Not Spam** in the UI.

## 🧪 Example Inputs

Here are sample messages and their expected outputs:


  ```text
  Input:
  Win a free iPhone by clicking this link now!

  Output:
  🟥 Spam
  ```
  ```text
Input:
Let’s meet tomorrow to discuss the project.

Output:
🟩 Not Spam
  ```
  

