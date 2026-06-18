# 📩 AI-Powered SMS Spam Detection System

An intelligent Machine Learning application that classifies SMS messages as **Spam** or **Legitimate (Ham)** using Natural Language Processing (NLP) and TF-IDF feature extraction.

Built using **Python, Scikit-Learn, and Streamlit**, this project helps users identify potentially fraudulent or unwanted SMS messages in real time.

---

## 🚀 Project Overview

Spam messages often contain fraudulent links, phishing attempts, fake offers, and scams. This project uses Machine Learning techniques to automatically detect spam SMS messages and improve user security.

The system processes SMS text, converts it into numerical features using TF-IDF, and predicts whether the message is Spam or Ham using a trained classification model.

---

## 🎯 Objectives

- Detect spam SMS messages automatically
- Improve user security against phishing and fraud
- Apply NLP techniques for text classification
- Compare machine learning algorithms
- Build a user-friendly prediction interface

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Programming Language |
| Pandas | Data Processing |
| NumPy | Numerical Computation |
| Scikit-Learn | Machine Learning |
| NLTK | Text Preprocessing |
| TF-IDF | Feature Extraction |
| Streamlit | Web Application |
| Joblib | Model Saving & Loading |
| Matplotlib | Data Visualization |
| Seaborn | Data Analysis |

---

## 📂 Project Structure

```text
SMS-Spam-Detection/
│
├── dataset/
│   └── spam.csv
│
├── models/
│   ├── spam_model.pkl
│   └── tfidf.pkl
│
├── train_model.py
├── app.py
├── requirements.txt
├── README.md
│
└── assets/
```

---

## 📊 Dataset Information

Dataset: SMS Spam Collection Dataset

- Total Messages: 5,572
- Ham Messages: 4,825
- Spam Messages: 747

Target Classes:

| Label | Meaning |
|---------|----------|
| Ham | Legitimate Message |
| Spam | Unwanted/Fraudulent Message |

---

## ⚙️ Machine Learning Workflow

```text
SMS Message
     ↓
Text Cleaning
     ↓
Tokenization
     ↓
Stopword Removal
     ↓
TF-IDF Vectorization
     ↓
Model Prediction
     ↓
Spam / Ham Classification
```

---

## 🧹 Text Preprocessing

The following preprocessing techniques are applied:

- Lowercase Conversion
- Removal of Special Characters
- Tokenization
- Stopword Removal
- Text Normalization

---

## 🤖 Model Used

### Logistic Regression

Reasons for choosing Logistic Regression:

- High Accuracy
- Fast Training
- Efficient for Text Classification
- Performs well with TF-IDF Features

---

## 📈 Performance

Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1 Score

Expected Accuracy:

```text
98%+
```

---

## 💻 Installation

### Clone Repository

```bash
git clone https://github.com/nithika1405/AI-SMS-Spam-Detection.git
```

### Move Into Project Directory

```bash
cd SMS-Spam-Detection
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Train the Model

```bash
python train_model.py
```

Output:

```text
Accuracy: 0.98+
Model Saved Successfully
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

The application will open automatically in your browser.

---

## 🧪 Example Predictions

### Example 1

Input:

```text
Congratulations!
You have won a free iPhone.
Click here to claim now.
```

Prediction:

```text
SPAM
```

---

### Example 2

Input:

```text
Hi Nithika,
Class starts at 9 AM tomorrow.
```

Prediction:

```text
HAM
```

---

## 🌍 Real-World Applications

- SMS Spam Filtering
- Telecom Industry
- Banking Security Systems
- Fraud Detection Platforms
- Cybersecurity Solutions
- Messaging Applications

---

## 🔮 Future Enhancements

- Deep Learning Models (LSTM)
- BERT-Based Classification
- Multilingual Spam Detection
- Real-Time SMS Monitoring
- Mobile Application Integration
- Cloud Deployment

---


### Home Page

![Home Page](assets/Homepage.png)

### Prediction Result

![Prediction Result](assets/Result.png)
 
---

## 👩‍💻 Author

**Nithika**

B.Tech Computer Science and Engineering (AI & ML)


---

## 📜 License

This project is developed for educational purposes.

---

## ⭐ If you found this project useful, please give it a star on GitHub.
