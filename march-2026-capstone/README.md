# March 2026 — Capstone Project: AI Career Coach

**Month:** March 2026  
**Program:** Pursuit AI Fellowship — Level 2  
**Author:** Paula Lawton

---

## Description

The capstone project synthesizes all skills developed throughout the fellowship into a single, production-ready AI application. The **AI Career Coach** is a full-stack web app that helps job seekers improve their resumes and prepare for technical interviews. It uses Retrieval-Augmented Generation (RAG) to ground LLM responses in real job descriptions and career coaching best practices.

## Topics Covered

- Retrieval-Augmented Generation (RAG) architecture
- Vector databases: storing and querying embeddings with `ChromaDB`
- OpenAI embeddings API (`text-embedding-ada-002`) for semantic search
- Full-stack integration: React frontend, FastAPI backend
- Prompt chaining and multi-step reasoning
- Deployment: containerized with Docker, deployed to a cloud platform

## Project Highlights

- **Resume Analyzer:** Users upload a resume (PDF) and paste a target job description. The app uses an LLM to identify skill gaps, suggest improvements, and highlight transferable experience — grounded by retrieved context from similar job postings.
- **Mock Interview Bot:** A chat-based interface where users practice answering behavioral and technical interview questions. The bot follows up with probing questions and provides scored feedback using a rubric stored in the vector database.
- **RAG Pipeline:** Job descriptions and coaching rubrics are chunked, embedded, and stored in ChromaDB. At query time, the top-k most relevant chunks are retrieved and injected into the LLM prompt to reduce hallucinations.
- **Evaluation Framework:** Built a small evaluation suite to measure answer relevance and faithfulness using the RAGAS framework.

## Architecture

```
User (Browser)
    │
    ▼
React Frontend (Vite + Tailwind CSS)
    │
    ▼
FastAPI Backend
    ├── /analyze-resume   → LLM + RAG pipeline
    ├── /interview-chat   → Conversational LLM with memory
    └── /upload-doc       → Embedding + ChromaDB ingestion
    │
    ├── OpenAI API (GPT-4o + text-embedding-ada-002)
    └── ChromaDB (local vector store)
```

## Skills Demonstrated

- End-to-end RAG system design and implementation
- Prompt engineering for structured outputs (JSON mode)
- PDF parsing and text chunking strategies
- Docker containerization and cloud deployment
- Building a user-facing AI product with real utility

## How to Run

```bash
# Clone and set up environment
cp .env.example .env   # Add OPENAI_API_KEY

# Backend
cd backend
pip install fastapi uvicorn openai chromadb pypdf python-dotenv ragas
uvicorn main:app --reload

# Frontend (separate terminal)
cd frontend
npm install
npm run dev
```

## Key Takeaways

Building an end-to-end AI product revealed the gap between a working demo and a production-ready application. RAG dramatically improves answer quality for domain-specific queries, but chunking strategy and retrieval tuning are where the real engineering effort lives. This project is the foundation for continued development beyond the fellowship.
