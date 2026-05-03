# 📩 SMS Spam Detection using Machine Learning

This project is a machine learning-based system that classifies SMS messages as **Spam** or **Not Spam (Ham)** using Natural Language Processing (NLP) techniques.

---

## 🚀 Features

- Classifies messages into spam or ham  
- Uses text preprocessing and vectorization  
- Compares two approaches:
  - CountVectorizer
  - TF-IDF Vectorizer  
- Achieves ~98% accuracy using Naive Bayes  

---

## 🛠 Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  

---

## 🧠 Machine Learning Approach

### 1. Data Preprocessing
- Removed unnecessary columns  
- Renamed columns (`label`, `text`)  
- Converted labels:
  - `spam → 1`
  - `ham → 0`

---

### 2. Feature Extraction

Two methods were used:

#### 🔹 CountVectorizer
- Converts text into word frequency  
- Performed better for this dataset  

#### 🔹 TF-IDF Vectorizer
- Considers importance of words  
- Slightly lower accuracy in this case  

---

### 3. Model Used

- **Multinomial Naive Bayes**

Reason:
- Works well with text classification  
- Efficient and fast  

---

## 📊 Results

| Method              | Accuracy |
|--------------------|----------|
| CountVectorizer    | ~98%     |
| TF-IDF             | ~96%     |

👉 CountVectorizer performed better because spam detection relies heavily on keyword frequency.

---

## 🧪 Sample Predictions

| Message                          | Prediction |
|----------------------------------|------------|
| "Win ₹5000 now!!!"              | Spam       |
| "Let's meet tomorrow"           | Ham        |
| "Free entry in contest"         | Spam       |

---

## 📁 Project Structure
main.ipynb       # Complete ML pipeline
spam.csv         # Dataset
README.md        # Project documentation
---

## 🔮 Future Improvements

- Use advanced models (Logistic Regression, SVM)  
- Add GUI (Streamlit / Web App)  
- Deploy as API  

---

## 👨‍💻 Author

Karan Singh