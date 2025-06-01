# SPAM-MAIL-PREDICTION-USING-ML

📧 Spam Mail Prediction System using Machine Learning
Author: Ashish Kumar
Project Type: Academic / ML Application
Technologies Used: Python, Scikit-learn, Pandas, NLTK, Tkinter

🔍 Overview
The Spam Mail Prediction System is a machine learning-based application that identifies whether a given email message is spam or not spam (ham). The project leverages Natural Language Processing (NLP) for text cleaning and classification using various algorithms, primarily the Multinomial Naive Bayes classifier.

This project also includes a GUI-based application using Tkinter, allowing users to interactively input email text and get real-time classification results.

🚀 Features
📄 Email Classification: Predicts email messages as Spam or Ham.

⚙️ Preprocessing: Text normalization, stopword removal, stemming (via NLTK).

📊 Model Evaluation: Accuracy, confusion matrix, precision, recall.

🧠 ML Algorithms: Multinomial Naive Bayes (with comparison to SVM and Decision Tree).

💻 User Interface: Simple GUI for interactive use using Tkinter.

📈 Visualization: Word cloud and accuracy comparison chart.

🛠️ Installation & Setup
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/spam-mail-prediction.git
cd spam-mail-prediction
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
(Ensure packages like pandas, sklearn, nltk, matplotlib, tkinter are installed.)

Run the Jupyter Notebook for model exploration and training:

bash
Copy
Edit
jupyter notebook "SPAM MAIL PREDICTION SYSTEM BY ML.ipynb"
Launch the GUI (if provided as a separate script):

bash
Copy
Edit
python gui_app.py
🧪 Dataset
The dataset used is based on the popular SMS Spam Collection Dataset, consisting of 5,572 labeled SMS messages. It includes:

label column (spam/ham)

message column (text content)

📉 Model Performance
Best Model: Multinomial Naive Bayes

Accuracy: ~98%

Includes a confusion matrix and evaluation metrics.

📁 Project Structure
vbnet
Copy
Edit
📦 spam-mail-prediction
├── SPAM MAIL PREDICTION SYSTEM BY ML.ipynb
├── requirements.txt
├── gui_app.py (optional)
├── README.md
└── assets/ (e.g. images, dataset files)
📌 Future Improvements
Support for live email inbox scanning.

Deployment as a web application (Flask/Django).

Integration with Gmail API for real-world use.

🧑‍💻 Author
Ashish Kumar
BSc/MSc in Computer Science
Galgotias University
[LinkedIn] | [GitHub]

📜 License
This project is licensed under the MIT License. Feel free to use and modify for educational or personal purposes.

