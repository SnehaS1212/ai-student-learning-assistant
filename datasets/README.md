# 📊 AI Student Learning Assistant - Datasets Hub

This directory contains the curated datasets, benchmark evaluation sets, standardized question banks, and synthetic student learning telemetry powering the **AI Student Learning Assistant**.

---

## 📁 Datasets Overview

| Dataset File | Format | Record Count | Description | Primary Usage |
| :--- | :---: | :---: | :--- | :--- |
| [`quiz_question_bank.json`](file:///c:/Users/anuja/AI-Student-Learning-Assistant/datasets/quiz_question_bank.json) | JSON | 50+ Questions | Standardized multi-choice questions across Computer Science, AI/ML, Math, and Data Structures | AI Quiz Generation fallback & evaluation benchmark |
| [`student_performance_dataset.csv`](file:///c:/Users/anuja/AI-Student-Learning-Assistant/datasets/student_performance_dataset.csv) | CSV | 100 Student Records | Student quiz scores, response times, topic mastery ratings, and study durations | Analytics, Leaderboard & GPA Predictor model training |
| [`sample_study_materials.json`](file:///c:/Users/anuja/AI-Student-Learning-Assistant/datasets/sample_study_materials.json) | JSON | 10 Subjects | Curriculum topic summaries, key concepts, bullet points, and key terms | AI Summarizer, Flashcard Player, and Research Lab testing |

---

## 🧬 Dataset Schemas

### 1. Quiz Question Bank (`quiz_question_bank.json`)
```json
{
  "question_id": "CS_DS_001",
  "category": "Data Structures",
  "difficulty": "Medium",
  "question": "What is the worst-case time complexity of QuickSort?",
  "options": ["O(N log N)", "O(N^2)", "O(N)", "O(1)"],
  "correct_answer": "O(N^2)",
  "explanation": "QuickSort degrades to O(N^2) worst-case time complexity when the pivot selection consistently yields unbalanced partitions."
}
```

### 2. Student Performance Dataset (`student_performance_dataset.csv`)
Columns: `student_id`, `username`, `quizzes_taken`, `avg_score`, `study_hours_weekly`, `flashcards_reviewed`, `mastery_level`, `predicted_gpa`

---

## 🛡️ Data Privacy & Compliance
All records in this directory are anonymized and generated for educational validation and code verification purposes.
