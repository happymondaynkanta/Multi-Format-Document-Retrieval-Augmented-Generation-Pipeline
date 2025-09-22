# Multi-Format-Document-Retrieval-Augmented-Generation-Pipeline
An end-to-end Retrieval-Augmented Generation (RAG) system for multi-format documents (PDF, Word, and PowerPoint). This project ingests documents from Google Drive, extracts and cleans text, splits content into chunks, generates embeddings with HuggingFace models, stores them in ChromaDB, and provides context-aware answers with source citations.   



# Multi-Format RAG Pipeline: Intelligent Document Knowledge Assistant

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![LangChain](https://img.shields.io/badge/LangChain-Framework-orange.svg)
![ChromaDB](https://img.shields.io/badge/Chroma-VectorDB-green.svg)
![HuggingFace](https://img.shields.io/badge/Embeddings-HuggingFace-yellow.svg)

---

## 📖 Overview

This repository demonstrates how to build a **Retrieval-Augmented Generation (RAG) system** that transforms **multi-format documents (PDF, Word, PowerPoint)** into an **interactive AI-powered knowledge assistant**.

The pipeline:

1. **Ingests documents from Google Drive** (PDF, DOCX, PPTX).
2. **Extracts and cleans text** with specialized format-specific loaders.
3. **Splits content into manageable chunks** with semantic overlap.
4. **Generates embeddings** using HuggingFace’s Sentence-Transformers.
5. **Stores embeddings in ChromaDB** for semantic similarity search.
6. **Retrieves context-aware chunks** in response to user queries.
7. **Generates grounded answers** with a large language model, including **source citations**.

This project highlights practical expertise in **LangChain, HuggingFace embeddings, document ingestion pipelines, and RAG architectures**, making it directly relevant for **AI/ML engineering and applied NLP roles**.

---

## ✨ Features

* 📂 **Google Drive Integration** for document ingestion in Colab
* 📑 **Multi-Format Support** (PDF, DOCX, PPTX) with specialized loaders
* 🧹 **Text Cleaning** to remove formatting noise and artifacts
* ✂️ **Document Chunking** with overlap for context preservation
* 🧠 **Embeddings via HuggingFace** (`all-MiniLM-L6-v2`)
* 📦 **ChromaDB Integration** for efficient semantic retrieval
* 🔍 **Retriever Interface** for top-k context selection
* 🤖 **RAG Answering Function** with context-grounded LLM outputs
* 📑 **Source Transparency** — every answer includes references

---

---

## ⚡ Usage

1. **Mount Google Drive** in Colab and set the path to your documents folder.
2. **Run loaders** to process PDF, Word, and PowerPoint files.
3. **Split, embed, and store documents** in ChromaDB.
4. **Query the system** through `rag_answer.py` or interactively in `notebook_demo.ipynb`.

### Example Interaction

**Question:**

```
"What topics are covered in the training slides?"  
```

**Answer:**

```
The training slides cover project management, agile workflows, and risk analysis.  
```

**Sources:**

```
- /content/drive/MyDrive/project_two/training_slides.pptx  
- /content/drive/MyDrive/project_two/project_overview.docx  
```

---

## 🎯 Applications

* **Education** → Semantic search across lecture slides, assignments, and notes
* **Enterprise** → Internal assistants for reports, policies, and training manuals
* **Research** → Retrieval over academic papers, presentations, and reference documents
* **Customer Support** → Multi-format knowledge assistants with verifiable answers

---

## 📑 Documentation

A detailed **Technical Report** is included in the `docs/` folder, covering design choices, workflow, and use cases.

---

## 🧑‍💻 Author

Developed by **\Happy Nkanta Monday** — AI/ML Engineer specializing in **Retrieval-Augmented Generation, Natural Language Processing, and Applied Machine Learning**.

If you find this project useful, ⭐ star the repo.

---



