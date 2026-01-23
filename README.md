# 📰 Fake News Detection (NLP + SVM + Streamlit)

This project is a **Fake News Detection System** built using **Natural Language Processing (NLP)** and **Machine Learning (Linear SVM)**.  
It classifies news articles as **FAKE** or **REAL** using the **TF-IDF Vectorizer** and a **LinearSVC** model.

---

## 📌 Features

✅ Load Fake and Real datasets (`Fake.csv` and `True.csv`)  
✅ Clean and preprocess text (lowercase, remove URLs, punctuation, stopwords, stemming)  
✅ Convert text into numerical format using **TF-IDF**  
✅ Train model using **Linear Support Vector Classifier (LinearSVC)**  
✅ Save trained model + vectorizer using **Joblib**  
✅ Streamlit Web App to test news input live  

---

## 📂 Project Structure

Fake-News-Detection/
│
├── Fake.csv
├── True.csv
├── fake_news_svm_model.pkl
├── tfidf_vectorizer.pkl
├── main.py
├── README.md


---

## 📊 Dataset

This project uses two datasets:

- **Fake.csv** → contains fake news articles  
- **True.csv** → contains real news articles  

Each dataset includes columns like:
- `title`
- `text`
- `subject`
- `date`

---

## ⚙️ Requirements

Install required libraries using:

```bash
pip install numpy pandas matplotlib seaborn nltk scikit-learn joblib streamlit

#🧠 Model Used

TF-IDF Vectorizer

max_features = 5000

ngram_range = (1,2) (unigram + bigram)

Classifier

LinearSVC() (Support Vector Machine)


#🧹 Text Preprocessing Steps

✔ Convert to lowercase
✔ Remove URLs
✔ Remove punctuation, numbers, special characters
✔ Remove stopwords
✔ Apply stemming using PorterStemmer


#🚀 How to Run the Project
#✅ Step 1: Train the Model

#Run your Python file to train and save the model:

python main.py


#This will create:

fake_news_svm_model.pkl

tfidf_vectorizer.pkl

#✅ Step 2: Run Streamlit App
streamlit run main.py


#Then open the browser link shown in the terminal.

🧪 Example Prediction

Input:

Government announces new policy for students


Output:

#✅ REAL NEWS / ❌ FAKE NEWS (depending on prediction)

📌 Streamlit App Output

The app allows the user to:

Paste any news text

Click Predict

Get result as:

❌ FAKE NEWS (Red)

✅ REAL NEWS (Green)

💾 Saved Model Files

#This project saves the trained model and vectorizer:

fake_news_svm_model.pkl

tfidf_vectorizer.pkl

These are used directly in Streamlit without retraining.

#🛠 Future Improvements

✨ Add more advanced models like:

Logistic Regression

Random Forest

LSTM / BERT

✨ Add accuracy and confusion matrix display in Streamlit
✨ Deploy online using Streamlit Cloud or HuggingFace Spaces

👨‍💻 Author

Developed by [Suraj Kumar]
Fake News Detection using NLP + SVM + Streamlit
