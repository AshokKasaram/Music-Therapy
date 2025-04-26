# Music Therapy : A Data-Driven Personalized Recommendation System

---

## Project Motivation
Music is a powerful emotional tool, often used for stress relief, mood regulation, and mental support.  
This project explores how **data science** and **machine learning** can personalize music recommendations based on **mental health profiles** and **listening behaviors**, aiming to **enhance emotional wellness through tailored musical experiences**.

---

## Project Workflow

1. **Dataset Loading and Cleaning**
   - Mental health survey dataset with emotional indicators (Anxiety, Depression, Insomnia, OCD) and music behaviors.
   - Standardized genre names, encoded categorical features, handled missing values.
   - Engineered new features like Genre Diversity Score.

2. **Exploratory Data Analysis (EDA)**
   - Analyzed relationships between mental health scores and favorite genres.
   - Investigated BPM (tempo) patterns, exploratory behavior, and genre preferences.
   - Visualized demographic trends across age groups and behaviors.

3. **Listener Segmentation**
   - Applied KMeans clustering to create user segments:
     - Low-Stress Chill Listeners
     - Moderate Familiar Listeners
     - High-Affect Exploratory Listeners
   - Visualized clusters using PCA.

4. **Music Impact Prediction**
   - Built ML models (Logistic Regression, Random Forest, XGBoost) to predict emotional outcomes:
     - Improve / No Effect / Worsen
   - Tuned hyperparameters and balanced dataset to improve fairness and macro F1-score.
   - Achieved 91% accuracy and strong minority class sensitivity with XGBoost.

5. **Recommendation System Development**
   - **Content-Based Filtering**: Matched user emotional-behavioral profile with genre profiles using cosine similarity.
   - **Collaborative Filtering**: Recommended genres based on peer users with similar emotional and listening traits.
   - **Hybrid Filtering**: Combined content and collaborative scores (60/40 weighting) to create balanced, empathetic recommendations.

6. **Real-Time Track Fetching**
   - Integrated **Spotify Web API** to fetch top 10 live tracks for each recommended genre.

7. **Web Application**
   - Built a full **Flask web app** running inside Jupyter Notebook.
   - Designed a dark-themed, Spotify-inspired UI for genre and track recommendations.

---

## Technologies Used

- **Python**: Pandas, NumPy, Scikit-learn, XGBoost
- **Machine Learning**: Classification, Clustering, Cosine Similarity
- **Web Development**: Flask, HTML, CSS (Spotify-styled UI)
- **Spotify API**: Real-time genre-to-track mapping
- **Visualization**: Matplotlib, Seaborn
- **Interactive Deployment**: Flask + Webbrowser (inside Notebook)

---

## Key Achievements

| Task                         | Outcome                                    |
| ---------------------------- | ----------------------------------------- |
| ML Modeling (XGBoost)         | 91% Accuracy, 90% Macro F1-Score          |
| Listener Clustering           | 3 meaningful listener personas identified |
| Hybrid Recommendation System | Balanced personal & peer-based suggestions |
| Web Application               | Fully functional Flask app with Spotify integration |

---

## Future Enhancements

- Expand the dataset with richer attributes and conduct broader surveys.
- Integrate audio-based track-level features (valence, energy) from Spotify.
- Add real-time feedback loop (thumbs up/down) for continuous model improvement.
- Publicly deploy the app on cloud platforms (AWS, GCP, Heroku).
- Explore personalized playlist generation and mood tracking.

---

# "Data gave the insight. Music gave it meaning."
