# InsightAI – AI-Powered Interview Management Platform

**InsightAI** is an advanced AI-driven platform that redefines interview management through automation, real-time analysis, and intelligent evaluation. The system combines **LLM-based mock interviews**, **gaze and emotion analysis**, and a robust backend for candidate tracking and scheduling—delivering an end-to-end solution for modern recruitment workflows.

## 🧠 Key Highlights

* **LLM-Powered Questioning:** Uses Groq AI and Google Generative AI to generate contextual, difficulty-tiered interview questions.
* **Real-Time Analysis:** Tracks eye movement and emotion using GazeML (MediaPipe + OpenCV) and DeepFace for behavioral insights.
* **Automated Scheduling:** Seamlessly integrates with Zoom and email services to coordinate interviews.
* **End-to-End Evaluation:** Automatically records, transcribes, and evaluates interviews to provide data-backed hiring insights.

---

## 📦 Project Structure

### 1. \[`aimockinterview/`] – Frontend (Next.js)

* AI-driven mock interview UI
* Real-time video/audio processing
* Clerk-based authentication
* Tailwind-based responsive design

### 2. \[`gazeml/`] – Gaze & Emotion Analysis (Python)

* Eye-tracking via MediaPipe & OpenCV
* Emotion detection using DeepFace
* Heatmap generation and live engagement metrics

### 3. \[`quasarai/`] – Backend API (Django)

* Candidate & session management
* Scheduling and resume parsing
* Feedback and report storage
* Groq API integration for LLM-based analysis

---

## 🛠️ Technology Stack

**Frontend:**

* Next.js 14, React 18
* Tailwind CSS, Clerk
* Drizzle ORM, Google Generative AI

**Backend:**

* Django 5.1, Python 3.8+
* SQLite, Gunicorn
* Groq LLM, PDF parsing

**GazeML Component:**

* Python, MediaPipe, OpenCV, DeepFace
* WebSocket streaming for real-time input

**APIs:**

* Zoom API, OAuth2
* Email notifications

---

## 🚀 Getting Started

### Prerequisites

* Node.js v18+
* Python 3.8+
* Git

### Installation Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Siddharth-Basale/Quasar3.oFinalRepo.git
   cd Quasar3.oFinalRepo
   ```

2. **Setup Frontend (AI Mock Interview)**

   ```bash
   cd aimockinterview
   npm install
   npm run dev
   ```

3. **Setup Backend (QuasarAI)**

   ```bash
   cd quasarai
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   python manage.py migrate
   python manage.py runserver
   ```

4. **Setup GazeML**

   ```bash
   cd gazeml
   pip install -r requirements.txt
   python app.py
   ```

---

## 🔐 Environment Variables

### AI Mock Interview (`.env`)

```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_key
CLERK_SECRET_KEY=your_clerk_secret
DATABASE_URL=your_database_url
GOOGLE_AI_API_KEY=your_google_ai_key
```

### QuasarAI (`.env`)

```
SECRET_KEY=your_django_secret_key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
```

---

## 📋 Features

* AI-generated interview questions using Groq and Google AI
* Real-time gaze and emotion tracking via GazeML
* PDF-based resume parsing
* Role-based access control and secure user management
* Video interview recording and transcription
* Interview scheduling and automated notifications

---

## 🤝 Contributing

1. Fork the repo
2. Create your feature branch: `git checkout -b feature/YourFeature`
3. Commit changes: `git commit -m 'Add YourFeature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Open a pull request

---

## 📄 License

Licensed under the [MIT License](LICENSE).

---

## 👤 Author

* Siddharth Basale – Developer & Project Lead

---

## 🙏 Acknowledgments

* [Google AI](https://ai.google/) – for LLM services
* [Groq](https://groq.com/) – for high-performance AI APIs
* [Clerk](https://clerk.dev/) – for authentication
* Open-source contributors and the AI/ML dev community
