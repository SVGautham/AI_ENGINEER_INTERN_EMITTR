# AI_ENGINEER_INTERN_EMITTR
# 🧠 Medical NLP Pipeline — Summarization, Sentiment, and SOAP Note Generation

This project implements a **Medical NLP Pipeline** capable of:
- Extracting structured **medical entities** (Symptoms, Diagnosis, Treatment, etc.)
- Performing **summarization** and **keyword extraction**
- Running **sentiment and intent analysis**
- Generating a **SOAP Note (Subjective, Objective, Assessment, Plan)** from doctor-patient conversations.

---

## 🚀 Features

| Module | Functionality |
|--------|----------------|
| **NER Extraction** | Identifies Symptoms, Diagnosis, Treatment, Prognosis from transcripts using spaCy |
| **Summarization** | Converts transcripts into structured medical summaries using `facebook/bart-large-cnn` |
| **Keyword Extraction** | Extracts key medical terms using `KeyBERT` |
| **Sentiment Analysis** | Detects emotional tone (Anxious / Neutral / Reassured) using DistilBERT |
| **Intent Detection** | Detects intent like “Reporting Symptoms” or “Seeking Reassurance” |
| **SOAP Note Generation** | Formats transcript into Subjective, Objective, Assessment, and Plan structure |

---

## 🛠️ Setup Instructions

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/SVGAUTHAM/AI_ENGINEER_INTERN_EMITTR.git
cd AI_ENGINEER_INTERN_EMITTR
```

### 2️⃣ Create and Activate Virtual Environment
Windows:
```bash
python -m venv venv
venv\Scripts\activate
```
macOS/Linux:
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
If you don’t have a requirements.txt file yet, create one using:
```
```bash
pip freeze > requirements.txt
```
Recommended contents:

```bash
spacy
transformers
torch
keybert
sentence-transformers
```

### 4️⃣ Download spaCy Model
```bash
python -m spacy download en_core_web_sm
```
