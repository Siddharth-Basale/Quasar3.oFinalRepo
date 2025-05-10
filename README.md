# InsighAI - AI-Powered Interview Platform

InsighAI is a comprehensive AI-powered interview platform that combines multiple components to provide an end-to-end interview experience. The platform consists of three main components: an AI Mock Interview system, a GazeML integration for eye-tracking analysis, and a QuasarAI backend for interview management.

## 🚀 Project Structure

The project is organized into three main components:

### 1. AI Mock Interview (`aimockinterview/`)
A Next.js-based web application that provides AI-powered mock interviews with features like:
- Real-time video interviews
- Speech-to-text capabilities
- AI-powered interview feedback
- User authentication and session management
- Modern UI with Tailwind CSS

### 2. GazeML Integration (`gazeml/`)
A Python-based component that handles eye-tracking analysis:
- Eye movement tracking
- Attention analysis
- Integration with the main interview platform

### 3. QuasarAI Backend (`quasarai/`)
A Django-based backend that manages:
- Interview scheduling
- Candidate management
- Interview feedback storage
- Integration with external services

## 🛠️ Technology Stack

### Frontend (AI Mock Interview)
- Next.js 14
- React 18
- Tailwind CSS
- Clerk Authentication
- Google Generative AI
- Drizzle ORM
- Various UI components (Radix UI, Headless UI)

### Backend (QuasarAI)
- Django 5.1
- SQLite Database
- Gunicorn
- Groq AI Integration
- PDF Processing capabilities

### GazeML Component
- Python
- Eye-tracking libraries
- WebSocket integration

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- Python 3.8+
- Git

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Siddharth-Basale/Quasar3.oFinalRepo.git
cd Quasar3.oFinalRepo
```

2. Set up the AI Mock Interview component:
```bash
cd aimockinterview
npm install
npm run dev
```

3. Set up the QuasarAI backend:
```bash
cd quasarai
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

4. Set up the GazeML component:
```bash
cd gazeml
pip install -r requirements.txt
python app.py
```

## 🔧 Environment Variables

Create appropriate `.env` files in each component directory with the following variables:

### AI Mock Interview
```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_key
CLERK_SECRET_KEY=your_clerk_secret
DATABASE_URL=your_database_url
GOOGLE_AI_API_KEY=your_google_ai_key
```

### QuasarAI
```
SECRET_KEY=your_django_secret_key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
```

## 📝 Features

- AI-powered mock interviews
- Real-time video and audio processing
- Eye-tracking analysis
- Interview feedback generation
- Candidate management system
- Interview scheduling
- PDF resume parsing
- User authentication and authorization

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Authors

- Your Name - Initial work

## 🙏 Acknowledgments

- Google AI for providing the AI capabilities
- Clerk for authentication services
- All other open-source contributors

## 📞 Support

For support, please open an issue in the GitHub repository or contact the maintainers.
