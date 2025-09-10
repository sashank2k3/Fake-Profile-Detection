Fake Profile Detection 
# 🚨 Fake Instagram Profile Detection using Machine Learning

This project is a real-time Instagram profile analyzer that predicts whether a given profile is **fake** or **real** using machine learning. It uses profile metrics like follower count, following count, post count, and verification status to make predictions.

---

## 📌 How It Works

- You enter an Instagram **username**.
- The application uses the **Apify API** to fetch public profile data.
- It extracts key features such as:
  - Number of followers
  - Number of followings
  - Number of posts
  - Is the account private?
  - Is the account verified?
- These features are passed into a pre-trained **machine learning model** (`classifier.pkl`) to predict whether the profile is real or fake.

---

## 🛠 Technologies Used

- **Python**
- **Streamlit** – for building the web app
- **Joblib** – for loading the ML model
- **Apify API** – to scrape Instagram data
- **Scikit-learn** – for training the ML model
- **Pandas, NumPy** – for data manipulation

---

## 🧠 ML Model

The model is trained using a labeled dataset containing Instagram profile attributes. The classification is binary:
- `0` → Likely Fake
- `1` → Likely Real

The training includes feature normalization and multiple algorithm trials like Logistic Regression, Decision Trees, and Random Forests. The final deployed model is chosen based on accuracy and generalization.

---

## 🖥️ Project UI

- The app is built with **Streamlit** for a clean and interactive interface
- Users simply input a **username** and click **Predict**.
- Output shows the profile’s stats and the prediction result with appropriate messaging (Success/Error).

---
