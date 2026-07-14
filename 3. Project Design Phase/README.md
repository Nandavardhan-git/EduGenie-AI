# Phase 3: Project Design Phase

This document describes the overall system architecture, application workflow, database design, and core modules of **EduGenie AI – AI Powered Educational Assistant**.

---

# 1. System Architecture

EduGenie AI follows a client-server architecture where the frontend communicates with the FastAPI backend through REST APIs. The backend processes user requests, interacts with the AI models, and returns structured educational responses.

### Technology Overview

| Layer | Technology |
|--------|------------|
| Frontend | HTML, CSS, JavaScript |
| Backend | FastAPI |
| Database | MongoDB |
| AI Models | Google Gemini 2.5 Flash, LaMini-Flan-T5 |
| Authentication | JWT |
| Testing | FastAPI TestClient |

---

# 2. System Workflow

The application processes user requests using the following workflow:

1. User opens EduGenie AI.
2. User selects a learning feature.
3. Request is sent to the FastAPI backend.
4. Backend validates the request.
5. Appropriate AI model processes the request.
6. Generated response is returned to the frontend.
7. Results are displayed to the user.

### Workflow Diagram

> *(Insert your System Flow Diagram here)*

```text
images/System_Workflow.png
```

---

# 3. Database Design

EduGenie AI stores user information and AI-generated educational content using MongoDB.

### Main Collections

| Collection | Purpose |
|------------|---------|
| Users | Stores user account information |
| User Queries | Stores user requests |
| AI Responses | Stores generated responses |
| Quiz | Stores generated quizzes |
| Summary | Stores summarized notes |
| Learning Path | Stores personalized learning recommendations |

### Entity Relationship Diagram

> *(Insert your ER Diagram here)*

```text
images/ER_Diagram.png
```

---

# 4. Core Modules

The project is divided into the following functional modules.

| Module | Description |
|---------|-------------|
| Authentication | User Registration & Login |
| Question Answering | Answers academic questions |
| Concept Explainer | Explains concepts based on learning level |
| Quiz Generator | Generates MCQs |
| Notes Summarizer | Summarizes educational content |
| Learning Roadmap | Creates personalized study plans |

---

# Design Outcome

✔ Client–Server Architecture Finalized

✔ Database Schema Designed

✔ Application Workflow Defined

✔ Core Modules Identified