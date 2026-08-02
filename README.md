# Simple RAG Demo — HR Policy Assistant

This project demonstrates a **Retrieval-Augmented Generation (RAG)** application built using **LangChain**, **FAISS**, **Jina AI Embeddings**, and **Groq LLM**.

The application answers questions about an HR policy document by retrieving the most relevant sections from the document and providing them as context to a Large Language Model (LLM). This approach produces responses that are grounded in the document instead of relying solely on the model's internal knowledge.

## Project Overview

The RAG pipeline implemented in this project consists of the following steps:

1. Load the HR policy document.
2. Split the document into smaller chunks.
3. Generate embeddings for each chunk using **Jina AI Embeddings**.
4. Store the embeddings in a **FAISS** vector database.
5. Retrieve the most relevant chunks for a user's query using semantic search.
6. Pass the retrieved context to the **Groq LLM** to generate a context-aware response.

This project demonstrates the core concepts behind Retrieval-Augmented Generation, including document preprocessing, vector search, semantic retrieval, and LLM integration.

---

# Technology Stack

| Component            | Technology       |
| -------------------- | ---------------- |
| Framework            | LangChain        |
| Language Model       | Groq             |
| Embeddings           | Jina AI          |
| Vector Database      | FAISS            |
| Programming Language | Python           |
| Notebook             | Jupyter Notebook |
| Web Framework        | Streamlit        |



# Getting Started

## 1. Install UV

```bash
pip install uv
```

## 2. Create a Virtual Environment

```bash
uv venv ragenv
```

## 3. Activate the Virtual Environment

### Windows

```bash
ragenv\Scripts\activate
```

### macOS / Linux

```bash
source ragenv/bin/activate
```

---

# Install Dependencies

Create a `requirements.txt` file containing:

```text
python-dotenv

langchain
langchain-core
langchain-community
langchain-text-splitters

langchain-groq

faiss-cpu

jupyter
ipykernel

streamlit
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

---

# Environment Variables

Create a `.env` file in the project root and add your API keys:

```env
GROQ_API_KEY=your_groq_api_key
JINA_API_KEY=your_jina_api_key
```

---

# Running the Project

### Jupyter Notebook

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Make sure the notebook is using the **`ragenv`** virtual environment.

### Streamlit Application

```bash
streamlit run app.py
```

---

# Git & GitHub Workflow

## Initialize Git

```bash
git init
```

## Stage Changes

```bash
git add .
```

## Commit Changes

```bash
git commit -m "Initial commit"
```

## Push to GitHub

```bash
git push origin main
```

---

# Key Concepts Demonstrated

* Retrieval-Augmented Generation (RAG)
* Semantic Search
* Document Chunking
* Text Embeddings
* Vector Databases
* Similarity Search
* LangChain Retrievers
* Prompt Engineering
* LLM Integration
* Environment Variable Management

---

# Learning Outcomes

Through this project, I explored the complete RAG workflow, including document ingestion, embedding generation, vector storage, semantic retrieval, and response generation using a Large Language Model. The implementation highlights how external knowledge can be integrated with LLMs to produce more accurate, context-aware, and reliable responses.

---

