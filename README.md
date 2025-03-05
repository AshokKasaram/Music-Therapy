# 🎵 AI-Powered Music Therapy Recommendation System 🎵  
🔬 **Leveraging AI & Machine Learning to Personalize Music for Mental Wellness**  

## 🌟 Project Overview  
This project explores the **relationship between music preferences and mental health** to build an **AI-powered music therapy system** that recommends **emotionally supportive songs.**  

By analyzing **listening habits, mental health conditions (Anxiety, Depression, Insomnia, OCD), and genre preferences**, the system generates **data-driven, personalized playlists** designed to **improve mood and well-being.**  

✅ **Predicts optimal music genres based on mental health data.**  
✅ **Fetches real-time song recommendations via Spotify API.**  
✅ **Uses Machine Learning, Content-Based & Collaborative Filtering for AI-driven recommendations.**  
✅ **Designed for future deployment using Flask/FastAPI with cloud hosting (AWS/GCP).**  

---

## 🔥 Features & Implementation  

### 📌 1. Data Collection & Cleaning  
- **Dataset:** The **MUSIC THERAPY DATASET** contains **listening habits, genre preferences, streaming platform choices, and self-reported mental health conditions.**  
- **Preprocessing Steps:**  
  - Missing values handled using **median (for numerical data) and mode (for categorical data).**  
  - Categorical variables encoded (**Yes/No responses mapped to 1/0**).  
  - Frequency-based responses standardized (**Never → 0, Rarely → 1, Frequently → 3, etc.**).  

---

### 📊 2. Exploratory Data Analysis (EDA) & Key Insights  
- **Correlations analyzed** between **music preferences and mental health conditions.**  
- **Key Findings:**  
  - **Rock & Pop** are the most preferred genres.  
  - **Latin & Gospel music are linked to lower anxiety levels.**  
  - **Rock, Hip-Hop, and EDM are associated with higher anxiety and depression.**  
  - **Classical music listeners reported lower depression scores (calming effect).**  
  - **Excessive music listening (12+ hours) correlates with higher anxiety and depression.**  
  - **Spotify dominates as the most-used platform (ideal for therapy interventions).**  

📌 **These insights were incorporated into feature engineering for improved model accuracy.**  

---

### 🔍 3. Feature Engineering & Machine Learning  
New features were created to enhance model performance:  
- 🎵 **Listening Intensity:** Average listening hours per day * genre preference scores.  
- 🎶 **Relaxing vs. Energetic Music Preference:** Aggregate score of calm genres (Classical, Jazz, Lofi) vs. high-energy genres (Rock, Hip-Hop, EDM).  
- 📊 **Total Genre Engagement:** Sum of all frequency-based genre scores.  

These features were used to train multiple machine learning models.  

---

### 🧠 4. Multi-Model Machine Learning Approach  
A **multi-model approach** was implemented to predict **music genres based on mental health factors.**  

🏆 **Models Implemented & Evaluated:**  
1️⃣ **Random Forest** 🌲  
2️⃣ **K-Nearest Neighbors (KNN)** 🔵  
3️⃣ **Neural Networks (Deep Learning - TensorFlow/Keras)** 🧠  
4️⃣ **XGBoost (Best Performing Model 🎯)** ✅  

📌 **Final Model Choice:** **XGBoost** (Best F1-score: **0.9800**).  
📌 **Dynamic Thresholding:** Fine-tuned genre selection using **precision-recall tradeoffs** to prevent overfitting.  

---

### 🔗 5. Hybrid Music Recommendation System  
A **hybrid recommendation system** was designed using:  
✅ **Content-Based Filtering** (Spotify Audio Features: Danceability, Valence, Energy, Tempo).  
✅ **Collaborative Filtering (Planned for Future Updates).**  
✅ **Hybrid Filtering (Mixing ML predictions & audio similarity scores).**  

📌 **Final output:** **Personalized song recommendations based on both user preferences and scientific audio analysis.**  

---

### 🎵 6. Real-Time Song Fetching via Spotify API  
The **Spotify API** was integrated to fetch **live song recommendations.**  
✅ **Spotify API Authentication (OAuth2.0).**  
✅ **Dynamic Genre-Based Song Search.**  
✅ **Audio Feature Extraction (Danceability, Valence, Energy, Tempo, etc.).**  
✅ **Top songs fetched with direct listening links!**  

📌 **Users can either:**  
🎧 **Manually select genres** → Fetch songs from Spotify.  
🎧 **Use AI-based genre prediction** → Model selects the best genres → Fetch songs accordingly.  

---

### 🛠 7. Project Architecture & Deployment Plans  
🏗 **Current Architecture:**  
- 🔹 **Python for Data Science & ML (Scikit-Learn, XGBoost, TensorFlow).**  
- 🔹 **Spotify API for real-time music recommendations.**  
- 🔹 **Flask/FastAPI (Planned for Deployment).**  
- 🔹 **AWS/GCP (Planned for Scaling & Hosting).**  

🚀 **Planned Upgrades:**  
- ✅ **Deploy via Flask for live user interaction.**  
- ✅ **Enhance Collaborative Filtering for User-Based Recommendations.**  
- ✅ **Build an Interactive Web UI.**  

---

## 🎯 Next Steps & Roadmap  
📌 **Short-Term Goals:**  
- [ ] Improve Recommendation Filtering Using Hybrid Methods.  
- [ ] Optimize Spotify API Queries for Better Song Fetching.  
- [ ] Deploy a Web-Based User Interface (Flask/FastAPI).  

📌 **Long-Term Goals:**  
- [ ] Add User Feedback Loop for **Personalized Reinforcement Learning.**  
- [ ] Integrate **Collaborative Filtering** for real-world user preferences.  
- [ ] Scale the system with **AWS Lambda & Serverless APIs.**  

---

## 🌟 Why This Project Matters  
🎶 **Music therapy has proven mental health benefits, but there is no AI-driven personalization at scale.**  
🚀 **This project combines Data Science, Machine Learning, and APIs to create a truly impactful recommendation system for mental wellness.**  
📈 **The final goal is to develop an intelligent, AI-powered music therapy platform accessible to millions worldwide.**  
