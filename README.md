Productionization-of-ML-Systems
🏨 Hybrid Travel Recommendation System (Capstone Project)

This project is part of a Travel & Tourism Capstone, where I built a Hybrid Recommendation System that suggests hotels to users using a combination of Collaborative Filtering and Content-Based Filtering.
The system is deployed as an interactive web application using Streamlit.

🚀 Project Highlights
Component	Description
Recommendation System	Hybrid (CF + CBF)
Machine Learning	KNNBasic (Surprise Library)
NLP	TF-IDF Vectorization
Deployment	Streamlit + Ngrok
Evaluation Metric	RMSE
Use Case	Personalized hotel recommendations
📁 Dataset Overview

The dataset consists of real-world hotel booking details:

travelCode → Unique booking ID
userCode → Unique user ID
name → Hotel name
place → Location
days → Stay duration
price → Cost per day
total → Total booking amount
date → Booking date
🧹 Data Preprocessing
Removed missing and duplicate values
Converted date column to datetime format
Standardized text fields (lowercase, cleaned)
Extracted insights like:
Unique users
Unique hotels
🤖 1. Collaborative Filtering (CF)
Implemented using KNNBasic from Surprise Library
Used total booking cost as implicit rating
Trained model on user-hotel interactions

📊 Performance:

RMSE ≈ 0.97
🧠 2. Content-Based Filtering (CBF)
Applied TF-IDF Vectorization on:
Hotel names
Locations
Calculated cosine similarity between hotels
Recommended similar hotels based on user history
🔀 3. Hybrid Recommendation System

Combined both approaches:

Final Score = 70% Collaborative Filtering + 30% Content-Based Filtering

✔ Improved personalization
✔ Better recommendation accuracy

🌐 4. Streamlit Web Application
Built an interactive UI using Streamlit
Users enter User ID
System returns Top Hotel Recommendations
Features:
Real-time predictions
Simple and clean UI
Easy to use
⚙️ How to Run Locally
Step 1: Install dependencies
pip install pandas numpy scikit-learn streamlit pyngrok scikit-surprise
Step 2: Run the app
streamlit run app.py
👤 Gender Classification API (NLP Project)

This module predicts gender from a person’s name using Deep Learning (BERT) and exposes it via a Flask REST API.

🧠 Project Highlights
Component	Tool/Tech
Model	BERT (bert-base-uncased)
NLP	Tokenization
API	Flask
Deployment	Ngrok + Docker
Automation	Jenkins
📁 Dataset
name → Person name
gender → Male / Female
Preprocessing:
Removed null values
Standardized text
Label encoding:
0 = Female
1 = Male
🧪 Model Training
Used BERT Tokenizer & Classifier
Fine-tuned on name dataset
Accuracy: ~60%+
🚀 API Flow
Input: Name
Model processes text
Output: Predicted Gender
✈️ Flight Price Prediction System

A machine learning model to predict flight ticket prices based on travel details.

🚀 Highlights
Trained on real flight data
Built using XGBoost Regressor
Deployed using Gradio (Hugging Face Spaces)
🧠 Features Used
Airline
Source
Destination
Duration
Total Stops
⚙️ Tech Stack
Python
Pandas, NumPy
Scikit-learn
XGBoost
Flask (API)
Gradio (UI)
🎯 Outcome
Accurate flight price prediction
Interactive UI for users
Scalable deployment-ready system
