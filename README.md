# Prompt Wars '26 
# 📚 AI Lecture Revision Engine
# 🎓 AI Lecture Revision Engine

> **AI-Powered Student Workspace**: Transform dense lecture materials (PDF, DOCX, TXT) into a high-yield study kit with executive summaries, key definitions & formulas cheat sheets, and 5-question interactive practice quizzes.

Powered by **Google Gemini 2.5 Flash** (`gemini-2.5-flash`) via the official `google-genai` SDK and Streamlit.

---

## ✨ Features

- **Multi-Format Ingestion**:
  - 📄 **PDF**: Page-by-page text parsing via `pypdf`.
  - 📝 **Word DOCX**: Structured paragraph and table extraction via `python-docx`.
  - 📃 **Plain Text / Markdown**: Robust multi-encoding decoding (UTF-8, Latin-1, CP1252).
  - ✍️ **Direct Notes Input**: Paste lecture notes or slide transcripts directly.
  - ⚡ **One-Click Academic Demo Presets**: Includes pre-loaded lectures for Computer Science (Neural Networks & Backprop), Bioengineering (CRISPR-Cas9), and Business Strategy (Porter's Five Forces).
- **Subject-Specific Tutoring Personalization**:
  - `General Academic`: Holistic, high-retention concept breakdown.
  - `Bioengineering & Life Sciences`: Pathways, molecular mechanisms, biochemical notation.
  - `Computer Science & Math`: Time/space complexity ($O(N)$), mathematical formulas, algorithms.
  - `Business & Social Sciences`: Strategic frameworks, economic models, market metrics.
- **High-Yield 3-Part Revision Kit**:
  1. **📋 Section 1: Core Summary & Executive Key Concepts**: Dense overview, key pillars, and high-probability exam hotspots.
  2. **🧪 Section 2: Terminology, Definitions & Formulas Cheat Sheet**: Formatted reference tables and exact equations.
  3. **🎯 Section 3: 5-Question Multiple Choice Quiz**: University-level questions with 4 plausible options, interactive self-test, and collapsible answer explanations.
- **Export & Download**:
  - Export complete study kit directly to Markdown format: `lecture_study_notes.md`.
- **Performance & Safety**:
  - Live character, word, and estimated read-time counters.
  - Automatic safe context cap (12,000 characters) to ensure ultra-fast response times without context overflow.

---

## 🚀 Quick Start

### 1. Install Dependencies
```bash
python -m pip install -r requirements.txt
```

### 2. Configure Gemini API Key
You can set your Gemini API key in your environment or enter it directly in the app's sidebar:
```powershell
$env:GEMINI_API_KEY="your-api-key-here"
```

### 3. Launch the Application
```bash
python -m streamlit run app.py
```
Open your browser at `http://localhost:8501`.

---

## 🏗️ Project Architecture

```
Prompt Wars '26/
├── app.py              # Main Streamlit single-page application & UI
├── requirements.txt    # Dependencies (streamlit, google-genai, pypdf, python-docx)
└── README.md           # Documentation
```
