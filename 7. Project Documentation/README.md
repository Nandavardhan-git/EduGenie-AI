# Phase 7: Project Documentation

This document provides the setup instructions, project configuration, API overview, and user guide for **EduGenie AI**.

---

# 1. System Requirements

### Hardware

- Processor: Intel i3 / AMD Ryzen 3 or higher
- RAM: Minimum 4 GB (8 GB Recommended)
- Storage: 2 GB Free Space
- Internet Connection

### Software

- Windows / Linux / macOS
- Python 3.10+
- FastAPI
- MongoDB
- Git & GitHub
- Visual Studio Code
- Google Gemini API Key

---

# 2. Installation & Setup

### Clone the Repository

```bash
git clone https://github.com/<your-username>/EduGenie-AI.git

cd EduGenie-AI
```

### Create Virtual Environment

```bash
python -m venv .venv
```

### Activate Environment

**Windows**

```bash
.venv\Scripts\activate
```

**Linux / macOS**

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file and add:

```env
GEMINI_API_KEY=your_api_key
MONGODB_URL=your_mongodb_connection
JWT_SECRET=your_secret_key
```

---

# 3. Running the Application

Start the FastAPI server:

```bash
python -m uvicorn app.main:app --reload
```

or

```bash
uvicorn app.main:app --reload
```

Open your browser:

```
http://127.0.0.1:8000
```

Swagger Documentation:

```
http://127.0.0.1:8000/docs
```

---

# 4. API Endpoints

| Endpoint | Method | Description |
|-----------|--------|-------------|
| /auth/signup | POST | User Registration |
| /auth/login | POST | User Login |
| /qa | POST | Educational Question Answering |
| /explain | POST | Concept Explanation |
| /quiz | POST | Quiz Generation |
| /summarize | POST | Notes Summarization |
| /recommend | POST | Study Roadmap Generation |
| /health | GET | Health Check |

---

# 5. User Guide

### Step 1

Register or login to the application.

### Step 2

Choose any educational module:

- Question Answering
- Concept Explanation
- Quiz Generator
- Notes Summarizer
- Learning Roadmap

### Step 3

Provide the required input.

### Step 4

The AI processes the request and returns the generated educational content.

---

# 6. Project Structure

```
EduGenie-AI/

├── app/
│   ├── ai/
│   ├── routes/
│   ├── services/
│   ├── prompts/
│   ├── models/
│   ├── utils/
│   ├── static/
│   ├── templates/
│   ├── config.py
│   └── main.py
│
├── .env.example
├── requirements.txt
├── verify_endpoints.py
└── README.md
```

---

# Documentation Outcome

✔ Installation Guide Prepared

✔ Environment Configuration Documented

✔ API Documentation Included

✔ User Guide Completed

✔ Project Structure Explained