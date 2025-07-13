# LegalDoc RAG System

**A context-aware Retrieval-Augmented Generation (RAG) system for legal document Q&A** — enabling precise, source-attributed answers from contracts, policies, and regulatory documents using semantic + keyword hybrid search.

---

## Overview

LegalDoc RAG System processes and indexes over **100+ legal documents** (contracts, ToS, privacy policies) and enables **interactive, traceable question-answering** using **RAG architecture** built with LangChain, OpenAI/HuggingFace, and FAISS.

> Designed for legal analysts, compliance teams, and enterprises needing reliable legal insights at scale — with attribution, semantic understanding, and audit history.

---

## Tech Stack

| Component          | Tool / Library                |
|--------------------|-------------------------------|
| Vector Search       | FAISS / Pinecone              |
| Embedding Models    | OpenAI / HuggingFace Transformers |
| RAG Framework       | LangChain                     |
| Backend API         | FastAPI                       |
| Frontend (UI)       | React / Gradio / HTML+JS      |
| Data Pipeline       | PDF/Text parser + chunker     |

---

## Key Features

-  **Hybrid Search** (semantic + keyword weighting)
-  **Context-Aware Answer Generation**
-  **Source Attribution** (document & chunk traceability)
-  **Query History + Analytics**
-  **Multi-Document Comparison Mode**
-  **Upload + Process 100+ Legal Docs**
-  **FastAPI REST API + Web UI Integration**

---

##  Business Impact

| Use Case                             | Solution Provided                        |
|--------------------------------------|------------------------------------------|
| Legal research bottlenecks           | Instant retrieval + summarized response  |
| No doc traceability in answers       | Full source attribution in every reply   |
| Cross-document inconsistencies       | Multi-doc comparison mode                |
| Repetitive compliance Q&A            | Automated response generation w/ logs    |

---

## How It Works

```mermaid
graph TD
    A[Legal Docs (.pdf/.txt)] --> B[Chunking + Embedding]
    B --> C[FAISS / Pinecone Index]
    D[User Query] --> E[Hybrid Retriever]
    C --> E
    E --> F[Context Injection]
    F --> G[LLM Answer Generation]
    G --> H[Answer + Source Attribution + Logs]
