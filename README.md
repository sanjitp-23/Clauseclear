# Clauseclear
<img width="709" height="659" alt="image" src="https://github.com/user-attachments/assets/2f875204-4c2c-4383-8d6d-76361e0e7118" />

ClauseClear is a web app that simplifies legal documents for ordinary users. The prototype accepts text or PDF uploads, splits the document into meaningful sections, generates concise plain-language summaries for each section, and automatically flags high-risk clauses with short reasons and recommended actions.


**Technologies:** Python, Pandas, Streamlit, RAG (Retrieval-Augmented Generation), LLMs  

Simplifying legal documents with AI — summarize contracts, agreements, and other dense legal texts in a few clicks.  

---

## 📌 Overview
Legal documents are often **dense, complex, and hard for non-lawyers to understand**. This project leverages **Information Retrieval + Context Augmentation using Large Language Models (LLMs)** to:  
- Extract key insights  
- Summarize complex clauses into **easy-to-read formats**  
- Make legal content **accessible for everyone**, not just lawyers

<img width="833" height="512" alt="image" src="https://github.com/user-attachments/assets/0727528c-f241-477b-8f43-7126fe0bdac7" />


---

## 🚨 The Problem
- Legal docs use **complex terminologies** requiring domain expertise.  
- Sentences are **long and dense**, making it hard to extract key info.  
- References to **statutes, legal citations, and prior knowledge** are common.  
- Conservative, risk-averse phrasing makes interpretation tricky.  
- Misinterpretation can lead to **serious consequences**.  

---

## 🤖 The Solution: AI-Powered Legal Summarization
With LLMs and RAG, we can now:  
✅ Extract **key insights** from legal documents  
✅ Summarize complex clauses into **plain language**  
✅ Retrieve relevant info using **RAG-based search**  
✅ Make legal content **easy and accessible**  

---

## 📌 How It Works

### 🔍 Retrieval-Augmented Generation (RAG)
RAG **improves summarization** by first retrieving relevant text and then generating a readable summary with an LLM.

**Step 1: Document Processing**  
- OCR or text extraction from PDFs/docs  
- Chunking large texts and tagging for easy search  

**Step 2: Document Retrieval**  
- BM25 ranking (keyword-based) or **Semantic Search** (context-based) to fetch relevant sections  

**Step 3: Context Augmentation**  
- Retrieved text is passed to an LLM for **structured, human-readable summaries**  

💡 Learn more: [Exploring the Power of RAG & OpenAI Function Calling for Q&A](#)

---

## 🛠 Installation & Setup

1️⃣ **Create a Virtual Environment**  
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
````

2️⃣ **Install Dependencies**

```bash
pip install -r requirements.txt
```

3️⃣ **Run the Application**

```bash
streamlit run summarize.py
```

---




