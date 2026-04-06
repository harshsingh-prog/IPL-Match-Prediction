🏏 IPL Win Probability Predictor
📌 Overview

The IPL Win Probability Predictor is a Machine Learning-powered web application that predicts the winning probability of a team during a live IPL match.

Built using Streamlit, this app takes real-time match inputs such as score, overs, wickets, and target, and calculates the probability of the batting and bowling teams winning.

🚀 Features
📊 Real-time win probability prediction
🧠 Machine Learning model (trained pipeline)
🎯 Interactive UI using Streamlit
⚡ Instant predictions based on match conditions
🏟️ Supports multiple IPL teams and venues

🧱 Project Architecture
IPL-Win-Predictor/
│
├── app.py                # Streamlit frontend application
├── pipe.pkl             # Trained ML model pipeline
├── IPL Win Probability Predictor.ipynb   # Model training notebook
├── README.md            # Project documentation

⚙️ Tech Stack

💻 Languages & Frameworks
Python 🐍
Streamlit (Web App Framework)
📚 Libraries Used
Pandas
NumPy
Scikit-learn
Pickle
🤖 Machine Learning
Classification Model (Logistic Regression / similar pipeline)
Feature Engineering:
Runs Left
Balls Left
Wickets Remaining
Current Run Rate
Required Run Rate
📊 Model Details

The model is trained on historical IPL match data and predicts win probability based on dynamic match conditions.

🔢 Input Features

Batting Team
Bowling Team
City
Target Score
Current Score
Overs Completed
Wickets Fallen
⚡ Derived Features (Auto-calculated)
Runs Left = Target - Score
Balls Left = 120 - (Overs × 6)
Wickets Remaining = 10 - Wickets Fallen
Current Run Rate = Score / Overs
Required Run Rate = (Runs Left × 6) / Balls Left

🧮 Prediction Logic
The model uses a trained pipeline (pipe.pkl) to compute probabilities:

Win Probability (Batting Team)
Loss Probability (Bowling Team)

🖥️ User Interface

The app provides:

Dropdowns for team selection
City selection
Numeric inputs for match stats
Predict button to calculate probability
