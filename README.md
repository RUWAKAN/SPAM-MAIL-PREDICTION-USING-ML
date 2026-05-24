# 📧 Spam Mail Prediction System using Machine Learning

A machine learning project that classifies email messages as **Spam** or **Ham (Not Spam)** using Natural Language Processing (NLP) and the Multinomial Naive Bayes algorithm. Built with Python in a Jupyter Notebook environment.

---

## 🖼️ Preview

| Ham (Not Spam) | Spam |
|---|---|
| | <img src="OK%20IMAGE.jpg" width="300"/> | <img src="SPAM%20IMAGE.jpg" width="300"/> | |

---

## ✨ Features

- Classifies any email message as **Spam** or **Ham** instantly
- Full NLP text preprocessing pipeline — cleaning, stopword removal, stemming
- Trained on 5,572 real labeled email messages
- ~98% model accuracy using Multinomial Naive Bayes
- Pre-trained model saved as `.pkl` for reuse without retraining
- TF-IDF vectorizer saved separately for consistent text transformation
- Confusion matrix and evaluation metrics included

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Language | Python 3 |
| Notebook | Jupyter Notebook |
| ML Library | Scikit-learn |
| NLP | NLTK |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Model Saving | Pickle (`.pkl`) |

---

## 🧪 Dataset

The project uses the **SMS Spam Collection Dataset** (`mail_data.csv`):

- 5,572 labeled messages
- Two columns: `Category` (spam / ham) and `Message` (email text)
- Sourced from the UCI Machine Learning Repository

---

## 📊 Model Performance

| Metric | Score |
|---|---|
| Accuracy | ~98% |
| Classifier | Multinomial Naive Bayes |

Full confusion matrix and precision/recall scores are available inside the notebook.

---

## 📂 Project Structure

```
📦 SPAM-MAIL-PREDICTION-USING-ML
├── SPAM MAIL PREDICTION SYSTEM BY ML.ipynb   # Main notebook
├── mail_data.csv                              # Dataset
├── spam.pkl                                   # Trained ML model
├── vectorizer.pkl                             # TF-IDF vectorizer
├── OK IMAGE.jpg                               # Ham result screenshot
├── SPAM IMAGE.jpg                             # Spam result screenshot
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3 and the following libraries installed:

```bash
pip install numpy pandas scikit-learn nltk matplotlib seaborn jupyter
```

Also download the NLTK stopwords corpus (run once):

```python
import nltk
nltk.download('stopwords')
```

### Run the Notebook

1. **Clone the repository**
   ```bash
   git clone https://github.com/RUWAKAN/SPAM-MAIL-PREDICTION-USING-ML.git
   cd SPAM-MAIL-PREDICTION-USING-ML
   ```

2. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

3. **Open** `SPAM MAIL PREDICTION SYSTEM BY ML.ipynb` and run all cells.

---

## 🔁 Using the Pre-trained Model

You can load the saved model directly without retraining:

```python
import pickle

# Load model and vectorizer
with open('spam.pkl', 'rb') as f:
    model = pickle.load(f)

with open('vectorizer.pkl', 'rb') as f:
    vectorizer = pickle.load(f)

# Predict on new email
email = ["Congratulations! You've won a free iPhone. Click here to claim."]
features = vectorizer.transform(email)
prediction = model.predict(features)

print("SPAM" if prediction[0] == 1 else "HAM")
```

---

## ⚙️ How It Works

```
Raw Email Text
      ↓
Text Preprocessing (lowercase, punctuation removal, stopwords, stemming)
      ↓
TF-IDF Vectorization
      ↓
Multinomial Naive Bayes Classifier
      ↓
Output: SPAM or HAM
```

---

## 🗺️ Roadmap

- [ ] Web app interface using Flask or Streamlit
- [ ] Gmail API integration for real inbox scanning
- [ ] Support for multilingual spam detection
- [ ] Deep learning model comparison (LSTM / BERT)

---

## 👨‍💻 Author

**Ashish Kumar (RUWAKAN)**
BCA (2022–2025) — Galgotias University

---

## 📜 License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify it for educational or personal purposes.
