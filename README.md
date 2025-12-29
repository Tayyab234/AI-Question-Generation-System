AI Question Generation System

A two-stage Large Language Model (LLM) pipeline that converts raw educational text into structured learning content such as MCQs, Q&A, True/False, Fill-in-the-Blanks, and Summaries.

This project is designed to work efficiently with free-tier LLMs by controlling token usage, chunking large documents, and separating reasoning from generation.

🚀 Key Features

🔁 Two-stage LLM architecture

Stage 1: Text → Structured Ideas / Summary

Stage 2: Ideas → Questions or Learning Content

🧠 Token-aware chunking for large documents

📚 Supports multiple learning formats:

MCQ

Question–Answer

True / False

Fill-in-the-Blank

Summary

🎯 Difficulty control using Bloom’s Taxonomy (Easy / Medium / Hard)

🧪 Free-tier friendly (Gemini / local LLM compatible)

🖥️ Optional Gradio-based UI

📄 Clean JSON outputs for downstream use

🏗️ Architecture Overview
Raw Text
   ↓
[ Chunking + Token Control ]
   ↓
Stage 1 LLM (Idea Extraction / Summary)
   ↓
ideas.txt
   ↓
Stage 2 LLM (Question Generation)
   ↓
Structured JSON Output


⚙️ How It Works
Stage 1 — Idea Extraction

Large documents are chunked using token limits

Each chunk is processed independently

Output is merged into a clean ideas.txt file

Stage 2 — Content Generation

Ideas are converted into:

MCQs

Q&A

True/False

Fill-in-the-Blanks

Summaries

Difficulty level controls cognitive depth

Output is saved as structured JSON

🖥️ Running the Gradio UI
python ui/gradio_app.py


Paste text or upload a file, select output type and difficulty, and generate learning material instantly.

🧪 Use Cases

Educational content generation

Exam preparation tools

Learning management systems (LMS)

AI tutoring systems

Automated assessment generation

📌 Future Improvements

Multi-language support

PDF & DOCX ingestion

Evaluation metrics for question quality

Deployment as an API

🤝 Contributing

Contributions, suggestions, and improvements are welcome!
