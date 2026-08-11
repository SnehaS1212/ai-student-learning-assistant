# 🎓 AI Student Learning Assistant

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-3.1.1-000000?style=for-the-badge&logo=flask&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-AI_Powered-F55036?style=for-the-badge&logo=groq&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Ready-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**An intelligent, AI-powered web application that transforms study materials into interactive learning experiences — summaries, flashcards, quizzes, study plans, research lab, and performance analytics.**

[🐛 Report Bug](https://github.com/SnehaS1212/ai-student-learning-assistant/issues) · [✨ Request Feature](https://github.com/SnehaS1212/ai-student-learning-assistant/issues)

</div>

---

## 📌 Repository & Code Validation

| Evaluation Category | Status | Details & Artifact Paths |
| :--- | :---: | :--- |
| **Source Code** | ✅ Validated | Modular Flask backend (`app.py`), HTML5 Jinja2 templates (`templates/`), custom CSS design system (`static/css/style.css`), and dependencies (`requirements.txt`). |
| **Datasets** | ✅ Uploaded | Curated datasets in [`datasets/`](./datasets/):<br>• [`quiz_question_bank.json`](./datasets/quiz_question_bank.json) (50+ CS/AI/DS questions)<br>• [`student_performance_dataset.csv`](./datasets/student_performance_dataset.csv) (100 student records)<br>• [`sample_study_materials.json`](./datasets/sample_study_materials.json) (Study material corpora) |
| **Logs** | ✅ Uploaded | Application execution & AI inference logs in [`logs/app.log`](./logs/app.log) with automatic file logging enabled in `app.py`. |
| **PPT & Report** | ✅ Uploaded | Documentation uploaded in [`docs/`](./docs/):<br>• 📊 **Presentation**: [`internship ppt.pptx`](./docs/internship%20ppt.pptx)<br>• 📑 **Report**: [`internship report.docx`](./docs/internship%20report.docx) |
| **Version Control** | ✅ Maintained | Full Git version history maintained and synchronized on GitHub (`SnehaS1212/ai-student-learning-assistant`). |

---

## 📋 Table of Contents

- [Repository & Code Validation](#-repository--code-validation)
- [Overview](#-overview)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
  - [Running Locally](#running-locally)
- [Project Structure](#-project-structure)
- [Project Artifacts (PPT, Report, Datasets, Logs)](#-project-artifacts)
- [AI Models & Pipeline](#-ai-models--pipeline)
- [Database Schema](#-database-schema)
- [License](#-license)

---

## 🌟 Overview

The **AI Student Learning Assistant** is a full-stack Flask web application powered by **Groq's ultra-fast LLM inference engines**. Students can upload any study material — PDF, DOCX, TXT, Markdown, or image scans — and the application automatically generates:

- 📝 **Comprehensive Summaries** (Detailed, Short, Exam Revision, and One-Page Notes)
- 🎴 **Interactive Flashcards** with flip animation and Leitner spaced-repetition tracking
- ❓ **Adaptive Quizzes** with instant feedback and AI tutor error explanations
- 📅 **Personalized Study Plans** (1-Day, 3-Day, and 7-Day exam schedules)
- 📊 **Performance Analytics**, class leaderboards, GPA predictor, and achievement certificates

---

## 🚀 Key Features

| Feature Module | Functionality & Capabilities |
| :--- | :--- |
| **📁 Multi-Format Upload** | Supports `.pdf`, `.docx`, `.txt`, `.md`, and image OCR (`.png`, `.jpg`, `.jpeg`) |
| **📝 Smart Summarizer** | Generates detailed summaries, key concepts, bullet points, and key terms |
| **🎴 Flashcard Deck** | Auto-generates Q&A flashcards per material with active recall flip mode |
| **❓ Adaptive Quiz Engine** | Configurable difficulty (Easy/Medium/Hard), automatic scoring, & weak topic breakdown |
| **🎓 AI Tutor Explanations** | Provides step-by-step reasoning for every incorrectly answered question |
| **🗓 Study Planner** | Exam-targeted daily study routines generated on-the-fly by Groq LLM |
| **🏆 Leaderboard & XP** | Gamified learning with experience points, achievement badges, and top student rankings |
| **🔁 Spaced Repetition** | Smart review scheduling algorithm based on retention intervals |
| **🔬 Research Lab** | Interactive AI assistant for deep-dive academic research and topic queries |
| **📈 GPA Predictor** | Machine-learning model estimating GPA based on study telemetry |
| **🗺 Career Navigator** | Maps student strengths and studied topics to industry career paths |
| **🏅 Certificate Generator** | Generates downloadable completion certificates upon topic mastery |
| **🔄 Self-Healing Pipeline** | Automatically regenerates corrupted summaries or missing flashcards on demand |

---

## 🛠 Tech Stack

### Backend & AI Pipeline
- **[Python 3.10+](https://www.python.org/)** — Core programming language
- **[Flask 3.1.1](https://flask.palletsprojects.com/)** — Web application framework
- **[Groq SDK](https://console.groq.com/)** — High-speed LLM inference engine (`llama-3.3-70b-versatile`, `llama-3.1-8b-instant`, `llama-3.2-11b-vision-preview`)
- **[PyMuPDF (fitz)](https://pymupdf.readthedocs.io/) & [pypdf](https://pypdf.readthedocs.io/)** — Robust PDF text parsing
- **[python-docx](https://python-docx.readthedocs.io/)** — Word document processing
- **[SQLite3](https://docs.python.org/3/library/sqlite3.html)** / **PostgreSQL** — Dual database support

### Frontend
- **HTML5 & Vanilla CSS3** — Modern UI with custom glassmorphism, responsive grid, and dark aesthetics
- **Jinja2** — Server-side template rendering

---

## 🚀 Getting Started

### Prerequisites

- Python **3.10+** installed
- A **[Groq API Key](https://console.groq.com/)** (Free tier available)
- `git` version control tool

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/SnehaS1212/ai-student-learning-assistant.git
   cd ai-student-learning-assistant
   ```

2. **Create and activate a virtual environment:**
   ```bash
   # Windows (PowerShell / CMD)
   python -m venv venv
   venv\Scripts\activate

   # macOS / Linux
   python -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

### Environment Variables

Create a `.env` file in the project root directory:

```env
# Required: Groq API Key
GROQ_API_KEY=your_groq_api_key_here

# Optional: Flask Secret Key
FLASK_SECRET_KEY=eduai-pro-secret-key-99881122
```

### Running Locally

```bash
python app.py
```

Open your browser and navigate to `http://localhost:5000`

---

## 📁 Project Structure

```
ai-student-learning-assistant/
│
├── app.py                  # Main Flask application (routes, AI inference, DB logic)
├── requirements.txt        # Python package dependencies
├── .gitignore              # Git exclusions
├── README.md               # Main project documentation & validation sheet
│
├── docs/                   # Internship presentation & report documentation
│   ├── internship ppt.pptx # Final Presentation slides
│   └── internship report.docx # Complete Internship Report
│
├── datasets/               # Quiz question banks, study material corpora, & student CSVs
│   ├── quiz_question_bank.json
│   ├── student_performance_dataset.csv
│   └── sample_study_materials.json
│
├── logs/                   # System runtime logs & AI audit logs
│   └── app.log             # Real-time application event log
│
├── templates/              # Jinja2 HTML templates
│   ├── base.html           # Layout shell & navigation
│   ├── index.html          # Main dashboard & material uploader
│   ├── summary.html        # AI summary viewer
│   ├── flashcards.html     # Interactive flashcard player
│   ├── quiz_setup.html     # Quiz configuration page
│   ├── quiz.html           # Interactive quiz interface
│   ├── result.html         # Quiz score report & AI tutor feedback
│   ├── study_plan.html     # Exam study schedule
│   ├── leaderboard.html    # Leaderboard & badges
│   ├── certificate.html    # Completion certificate
│   ├── spaced_repetition.html # Leitner review scheduler
│   ├── career_navigator.html  # Career path guidance
│   ├── research_lab.html   # AI research assistant
│   ├── gpa_predictor.html  # GPA prediction analytics
│   └── admin_panel.html    # Admin management panel
│
└── static/                 # CSS stylesheets, JavaScript, and background assets
    └── css/style.css
```

---

## 📂 Project Artifacts

### 1. Presentation Slides & Report ([`docs/`](./docs/))
- **📊 PPT Presentation**: [`docs/internship ppt.pptx`](./docs/internship%20ppt.pptx) — Presentation detailing architecture, Groq LLM integration, and user features.
- **📑 Internship Report**: [`docs/internship report.docx`](./docs/internship%20report.docx) — Full technical report documenting domain background, requirements, design diagrams, implementation details, and evaluation.

### 2. Datasets ([`datasets/`](./datasets/))
- **`quiz_question_bank.json`**: Standardized multi-choice questions across Computer Science, Machine Learning, Data Structures, Web Development, and Databases.
- **`student_performance_dataset.csv`**: Synthetic dataset containing student quiz scores, response times, weekly study hours, and GPA predictions.
- **`sample_study_materials.json`**: Sample curriculum summaries and flashcard decks used for automated offline testing.

### 3. Application Logs ([`logs/`](./logs/))
- **`app.log`**: System logs tracking database initialization, file upload text extraction, Groq API inference calls, primary/fallback model switches, and route request status.

---

## 🤖 AI Models & Pipeline

| Model | Purpose & Function |
| :--- | :--- |
| `llama-3.3-70b-versatile` | **Primary Model**: Generates detailed summaries, flashcards, quizzes, study plans, and tutor explanations. |
| `llama-3.1-8b-instant` | **Fallback Model**: Automatically takes over if the primary model hits rate limits or latency thresholds. |
| `meta-llama/llama-4-scout-17b-16e-instruct` | **Vision Model**: Performs text extraction / OCR on uploaded study images (`.png`, `.jpg`). |

---

## 🗃 Database Schema

The SQLite database (`database.db`) consists of three primary tables:

### 1. `materials`
| Column | Type | Description |
| :--- | :--- | :--- |
| `id` | INTEGER PK | Auto-increment primary key |
| `filename` | TEXT | Original uploaded filename |
| `filepath` | TEXT | Storage path in `uploads/` |
| `extracted_text` | TEXT | Full extracted text content |
| `summary_detailed` | TEXT | Comprehensive AI summary |
| `summary_short` | TEXT | Executive 2-3 sentence summary |
| `summary_revision` | TEXT | Key revision bullet points |
| `summary_onepage` | TEXT | Quick cheat-sheet notes |
| `created_at` | DATETIME | Upload timestamp |

### 2. `flashcards`
| Column | Type | Description |
| :--- | :--- | :--- |
| `id` | INTEGER PK | Auto-increment primary key |
| `material_id` | INTEGER FK | Foreign key referencing `materials.id` |
| `front` | TEXT | Question, prompt, or term |
| `back` | TEXT | Answer, explanation, or formula |

### 3. `quiz_results`
| Column | Type | Description |
| :--- | :--- | :--- |
| `id` | INTEGER PK | Auto-increment primary key |
| `username` | TEXT | Student username |
| `filename` | TEXT | Source material name |
| `topic` | TEXT | Quiz topic |
| `difficulty` | TEXT | Easy / Medium / Hard |
| `score` | INTEGER | Correct answer count |
| `total` | INTEGER | Total question count |
| `percentage` | REAL | Percentage score |
| `weak_topics` | TEXT | Identified weak topics (JSON) |
| `study_plan_1d` | TEXT | 1-Day study schedule (JSON) |
| `study_plan_3d` | TEXT | 3-Day study schedule (JSON) |
| `study_plan_7d` | TEXT | 7-Day study schedule (JSON) |
| `readiness_score` | INTEGER | Readiness percentage (0-100) |
| `tutor_feedback` | TEXT | AI tutor step-by-step feedback (JSON) |
| `timestamp` | DATETIME | Attempt submission timestamp |

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

<div align="center">

Made with ❤️ by **[Sneha S](https://github.com/SnehaS1212)**

</div>
