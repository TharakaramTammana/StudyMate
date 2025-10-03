# 📚 StudyMate (Granite 2B Instruct Version)

StudyMate is an AI-powered academic assistant that lets you upload PDFs, ask questions, and get answers grounded in your own material. It uses **Granite 2B Instruct** as the LLM backend.

---

## 🚀 Features

* 📂 Upload one or more PDFs
* 🔎 Extract & chunk text
* 📐 Embed with **SentenceTransformers**
* 🔗 Search relevant chunks with **FAISS**
* 🤖 Answer questions using **Granite-2B-Instruct**
* 📜 Keep Q&A history & download transcript

---

## ⚙️ Setup Instructions

### 1. Clone the Project

```bash
git clone https://github.com/TharakaramTammana/StudyMate.git
cd StudyMate
```

### 2. Create & Activate Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

### 3. Install Requirements

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file with the following:

```env
API_KEY="Your API key"
PROJECT_ID="PROJECT_ID"
```

⚠️ **Do not share your API key or Project ID publicly.**

### 5. Run the App

```bash
streamlit run app.py
```

---

## 📂 Project Structure

```
StudyMate-OpenAI/
│── requirements.txt
│── app.py
│── pdf_processor.py
│── retriever.py
│── llm_openai.py
│── README.md
```

---

## 🔑 Environment Variables

* `API_KEY` → Your API key 
* `PROJECT_ID` → Unique ID for your project 

---

## 📜 Example Usage

1. Upload PDFs in the web interface
2. Ask a question like:
   *“What is the main concept explained in chapter 3?”*
3. StudyMate retrieves relevant chunks and generates an answer.

---

## 🛡️ Notes

* Make sure you **never commit `.env`** to GitHub.
* The Project ID ensures your API usage is tracked under the right project.
