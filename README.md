# Deep-fake-Audio-detection

## Overview
This Flask-based web application allows users to register and log in to the system, and test audio files to detect whether they are genuine or fake. The classification is performed using a Random Forest machine learning model trained on audio features. The app provides a simple UI for audio testing and user management.

## Features
- User registration and login system with SQLite database backend
- Audio file testing to classify real or fake audio using ML model
- Displays classification result on the web interface
- Simple web pages for user interaction and audio testing

## Technologies
- Python
- Flask
- SQLite for user data storage
- Librosa for audio feature extraction
- Scikit-learn for the Random Forest classifier
- Joblib for model serialization

## Installation
1. Clone the repository
2. Install dependencies:
pip install flask librosa numpy scikit-learn joblib
3. Ensure the pre-trained model file `random_forest_model.joblib` is in the project directory.
4. Run the Flask app:
python app.py
5. Open the browser at `http://127.0.0.1:5000/`

## Usage
- Register as a new user or log in with existing credentials.
- Navigate to the audio testing page.
- Upload or specify the audio file path to test.
- View the result: "Real" or "Fake" audio.

## File Structure
- `app.py` - Main Flask application handling routes and rendering templates
- `audio_test.py` - Contains audio feature extraction and prediction logic
- `random_forest_model.joblib` - Pre-trained Random Forest model file
- `templates/` - HTML templates for rendering the web pages
- `static/audio/` - Directory for audio files to be tested

## Notes
- Ensure audio files are in supported formats compatible with librosa.
- Database `user_data.db` is created automatically on first run.

## Authors
Harshitha D G - AI Software Engineer Intern
Deepak Athresh R - Software Engineer Intern


