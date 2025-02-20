# 🎵 Facial Emotion-Based Music Recommendation System

## 📌 Overview
This project is an **AI-powered music recommendation system** that detects facial emotions using **Computer Vision (OpenCV)** and **Machine Learning**, then recommends and plays songs from **Spotify** based on the detected mood.

## 🚀 Features
- **Real-time Facial Emotion Detection** using OpenCV.
- **Machine Learning Model (Random Forest)** for emotion classification.
- **Spotify API Integration** for music recommendation.
- **Automatic Web Launch & Music Play** on Spotify.
- **Webcam-based Emotion Detection**.

## 🎯 How It Works
1. **Detect Face & Emotion:** The system captures a live feed from the webcam and detects the user's facial expression.
2. **Classify Emotion:** The trained ML model classifies the detected face into one of the emotions.
3. **Fetch a Song:** Based on the emotion, the system queries the **Spotify API** to get a relevant song.
4. **Play Music:** The recommended song **automatically opens in a web browser and starts playing**.

## 📌 Technologies Used
- **Python** (OpenCV, NumPy, Scikit-learn)
- **Machine Learning (Random Forest Classifier)**
- **Spotify API** for music recommendation
- **Web Browser Automation** to open Spotify

## 📂 Project Structure
```
├── dataset/                 # Emotion dataset (train & test images)
├── facial_emotion_music.py  # Main Python script
├── requirements.txt         # Required dependencies
├── README.md                # Project documentation
└── captured_image.jpg       # Sample captured face image
```

## 🔧 Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/facial-emotion-music.git
cd facial-emotion-music
```
### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```
### 3️⃣ Set Up Spotify API
1. Go to [Spotify Developer Dashboard](https://developer.spotify.com/dashboard)
2. Create an app and get the **Client ID** & **Client Secret**
3. Update the following lines in `facial_emotion_music.py` with your credentials:
```python
client_id = 'your-client-id'
client_secret = 'your-client-secret'
```
### 4️⃣ Run the Project
```bash
python facial_emotion_music.py
```

## 🎭 Emotion Mapping with Spotify Genres
| Emotion  | Genre       |
|----------|------------|
| Angry    | Rock       |
| Disgust  | Classical  |
| Fear     | Ambient    |
| Happy    | Pop        |
| Neutral  | Chill      |
| Sad      | Acoustic   |
| Surprise | Party      |

## 🎥 Demo
When a face is detected:
- A bounding box appears around the face.
- The detected emotion is displayed on the screen.
- A song matching the mood is fetched from **Spotify**.
- The song **automatically plays in the web browser**.

## 📌 Notes
- The model is trained on grayscale **48x48** facial images.
- Ensure the **webcam is properly connected** before running the script.
- You can modify `emotion_to_genre` mapping to customize the music preferences.

## 🤝 Contribution
Feel free to fork this project and contribute by improving the model, adding features, or integrating with other music services!

## 📜 License
This project is licensed under the MIT License.

---
🚀 **Enjoy AI-powered music based on your mood!** 🎶


