# 🎵 Music Emotion Matcher

**Music Emotion Matcher** is an intelligent real-time music recommendation system that personalizes your music experience by analyzing your **facial expressions** and **voice** to detect your mood. Based on the detected emotion, it recommends a tailored Spotify playlist to match your emotional state — creating an immersive and mood-enhancing experience.

---

## 🌟 Product Vision

Our goal is to change how people discover and enjoy music by building a system that understands their emotions. The system will recognize a person's mood through facial expressions or voice (speech) and suggest songs based on how they feel at that moment.

We aim to make listening to music more **personal, effortless, and enjoyable** — offering the right songs at the right time.

---

## 👥 FOR WHOM?

- **FOR**: Music lovers and individuals who enjoy personalized listening.
- **WHO**: Need music recommendations that match their emotional state for improved mood and engagement.
- **THE MUSIC EMOTION MATCHER** is a smart music recommendation system
- **THAT**: Automatically detects facial emotions or voice tones to recommend songs suited to the user's current feelings.
- **UNLIKE**: Traditional music platforms that rely only on past listening history or manual selections,
- **OUR PRODUCT**: Uses advanced facial and speech emotion detection technology with real-time music suggestions from Spotify — offering an intuitive, natural, and deeply personal experience.

---

## 🧠 Core Components

The system comprises three interconnected modules:

1. **Facial Emotion Recognition (FER)**  
   Uses computer vision (OpenCV + DeepFace) to analyze facial expressions and detect emotions like happiness, sadness, anger, and more.

2. **Speech Emotion Recognition (SER)**  
   Extracts features from user audio (via microphone) using **Librosa** and classifies emotions with a **CNN model** built using TensorFlow/Keras.

3. **Music Recommendation Engine**  
   Maps the detected emotions to relevant music genres and uses the **Spotify Web API** to generate emotion-based playlists.

---

## 🛠 Tech Stack

| Layer       | Technology                       |
|-------------|----------------------------------|
| Frontend    | React.js                         |
| Backend     | Flask (Python)                   |
| ML Models   | TensorFlow/Keras, DeepFace       |
| Audio       | Librosa, sounddevice             |
| Video       | OpenCV                           |
| API         | Spotify Web API                  |
| Database    | SQLite (for emotion logs)        |

---

## 🚀 Features

- Real-time **facial expression** and **speech** emotion detection
- Interactive and responsive **React UI**
- Personalized **Spotify playlists** mapped to current emotional state
- Emotion logs and insights
- Easy-to-use interface — no manual mood input required

---

## 📂 Project Structure

```bash
music-emotion-matcher/
│
├── backend/
│   ├── server.py               # Flask server and API endpoints
│   ├── face_emotion_model.pkl  # Pre-trained facial emotion model
│   ├── speech_emotion_model.pkl# Trained speech emotion CNN
│   ├── utils/                  # Emotion processing utils
│   └── static/uploads/         # Audio/video uploads (temp)
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.js
│   │   └── index.js
│
├── database/
│   └── emotions.db             # SQLite database for logs
│
├── requirements.txt
├── README.md
└── .env                        # Spotify API keys & env variables
