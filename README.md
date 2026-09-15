# Interview Simulator

An intelligent AI-powered interview simulation platform that combines **Large Language Models (LLMs)** with **Machine Learning** to generate interview questions, evaluate candidate responses, and provide personalized feedback.

## 🚀 Live Demo

[Interview Simulator](https://interview-simulator-1-vl0h.onrender.com)

## 📌 Overview

The Interview Simulator provides an interactive environment for practicing technical interviews.

The system combines:

* **LLM-based question generation**
* **Machine Learning-based answer evaluation**
* **Personalized feedback**
* **Adaptive interview difficulty**
* **Session tracking**

The application is designed as a modular pipeline where interview questions are generated, candidate answers are evaluated, and feedback is provided based on the candidate's performance.

## ✨ Features

* 🤖 **AI Question Generation**
  Generates interview questions dynamically using Google's Gemini API.

* 📊 **ML-Based Answer Scoring**
  Uses a **Random Forest** model to evaluate candidate responses.

* 🎯 **Adaptive Difficulty**
  Adjusts the interview experience based on candidate performance.

* 💡 **Personalized Feedback**
  Provides feedback to help candidates identify strengths and areas for improvement.

* 🔄 **Interactive Interview Flow**
  Supports a structured question → answer → evaluation → feedback workflow.

* 🔐 **Session Tracking**
  Uses Firebase to manage interview sessions and candidate progress.

* 🖥️ **Full-Stack Architecture**
  React frontend with a FastAPI backend.

## 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │      React UI       │
                    │     Frontend        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │     FastAPI API     │
                    │      Backend        │
                    └──────────┬──────────┘
                               │
                 ┌─────────────┼─────────────┐
                 ▼             ▼             ▼
        ┌──────────────┐ ┌────────────┐ ┌─────────────┐
        │ Gemini API   │ │ ML Model   │ │  Firebase   │
        │ Question &   │ │  Random    │ │   Session   │
        │ Feedback     │ │  Forest    │ │   Tracking  │
        └──────────────┘ └────────────┘ └─────────────┘
```

## 🛠️ Tech Stack

### Frontend

* React.js
* JavaScript
* HTML
* CSS

### Backend

* Python
* FastAPI
* REST APIs

### AI / Machine Learning

* Google Gemini API
* Scikit-learn
* Random Forest
* Prompt Engineering

### Database / Services

* Firebase

### Deployment

* Render

## 📁 Project Structure

```text
INTERVIEW_SIMULATOR/
│
├── backend/
│   ├── ...
│   └── ...
│
├── frontend/
│   ├── ...
│   └── ...
│
├── README.md
└── ...
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/tabrealamsyed/INTERVIEW_SIMULATOR.git
cd INTERVIEW_SIMULATOR
```

### 2. Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```bash
venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

### 3. Environment Variables

Create a `.env` file inside the backend directory and add the required API credentials and configuration.

Example:

```env
GEMINI_API_KEY=your_gemini_api_key
```

Add any additional Firebase or application-specific variables required by the backend configuration.

**Do not commit your `.env` file or API keys to GitHub.**

### 4. Start the Backend

Run the FastAPI application using the project's configured entry point.

For example:

```bash
uvicorn main:app --reload
```

### 5. Frontend Setup

Open a new terminal:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

The frontend will then be available at the local URL shown in your terminal.

## 🔄 Application Workflow

```text
Start Interview
       │
       ▼
Generate Question
       │
       ▼
Candidate Provides Answer
       │
       ▼
Evaluate Answer
       │
       ├──────────────► ML Model
       │                  │
       ▼                  ▼
Generate Feedback ◄──── Score
       │
       ▼
Adjust Difficulty
       │
       ▼
Next Question
```

## 📈 Future Improvements

* Voice-based interview interaction
* Speech-to-text answer evaluation
* More advanced candidate performance analytics
* Additional ML models for answer scoring
* Interview history and progress dashboards
* Support for multiple interview domains
* Improved adaptive difficulty algorithms

## 👨‍💻 Author

**Syed Tabre Alam Khadri**

* GitHub: [@tabrealamsyed](https://github.com/tabrealamsyed)
* LinkedIn: [Syed Tabre Alam Khadri](https://www.linkedin.com/in/tabre-alam-syed-74583532b/)

## 📄 License

This project is intended for educational and portfolio purposes.
