
# MedGPT: An Autonomous AI Physician for Healthcare

MedGPT is an AI-powered medical assistant designed to simulate physician-patient interactions and assist users with symptom analysis, triage scoring, and general health-related questions.

## 🚀 Features

- Chat-based interface for medical queries
- LLM-powered responses using Gemini API
- Triage scoring and risk assessment based on symptoms
- Auto-initialization status for LLM
- Backend using FastAPI
- Frontend using Next.js and Axios

## 🧠 Tech Stack

- **Frontend**: Next.js, Tailwind CSS, Axios
- **Backend**: FastAPI, LangChain, Gemini Pro
- **LLM**: Gemini API (Google AI Studio)

## ⚙️ Installation

### Backend

1. Create a virtual environment:
   ```bash
   python -m venv env
   source env/bin/activate
   ```

2. Install dependencies:
   ```bash
   pip install fastapi uvicorn langchain google-generativeai
   ```

3. Add your Gemini API key to `.env`:
   ```env
   GOOGLE_API_KEY=your_gemini_api_key
   ```

4. Run backend server:
   ```bash
   uvicorn main:app --reload
   ```

### Frontend

1. Navigate to frontend folder:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run development server:
   ```bash
   npm run dev
   ```

## 📡 Deployment

### Frontend - Netlify

1. Push frontend code to GitHub
2. Link repo to Netlify
3. Set build command: `npm run build`
4. Set publish directory: `.next` or `out` (if using static export)

### Backend - Render

1. Push backend code to GitHub
2. Create new Render web service
3. Set environment variable `GOOGLE_API_KEY`
4. Use build command:
   ```bash
   pip install -r requirements.txt
   uvicorn main:app --host 0.0.0.0 --port 8000
   ```

## 📜 License

This project is for educational purposes only and not a substitute for professional medical advice.

---

