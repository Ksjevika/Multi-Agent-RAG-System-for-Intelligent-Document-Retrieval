# Multi-Agent RAG System for Intelligent Document Retrieval

A modular **Multi-Agent Retrieval-Augmented Generation (RAG)** system built with **LangGraph**, **LangChain**, and **Qdrant** for intelligent document retrieval and context-aware question answering. The system leverages hierarchical indexing, hybrid retrieval, conversation memory, query refinement, and multi-agent orchestration to deliver accurate and reliable responses from enterprise knowledge bases.

---

## 🚀 Overview

This project implements an advanced Agentic RAG pipeline designed for document-centric AI applications. Instead of relying on a single retrieval step, it employs multiple specialized agents that collaborate to analyze user queries, retrieve relevant information, refine search results, and generate context-aware answers.

The architecture is modular and provider-agnostic, making it easy to integrate different LLMs, embedding models, vector databases, and retrieval strategies.

---

# ✨ Key Features

- Multi-Agent workflow orchestration using **LangGraph**
- Hierarchical **Parent–Child document chunking**
- Hybrid retrieval combining semantic vector search and keyword search
- Context-aware conversation memory
- Intelligent query rewriting for improved retrieval accuracy
- Human-in-the-loop query clarification for ambiguous questions
- Self-correcting retrieval loop with automatic re-search
- Context compression for efficient prompt management
- Parallel agent execution for complex and multi-part queries
- Modular architecture supporting multiple LLM providers
- Built-in observability and tracing using Langfuse

---

# 🏗 Architecture

```
                     Documents
                         │
                         ▼
             Document Preprocessing
                         │
                         ▼
          Parent–Child Hierarchical Chunking
                         │
                         ▼
               Embedding Generation
                         │
                         ▼
                  Qdrant Vector Store
                         │
                         ▼
                 User Question
                         │
                         ▼
            Conversation Summarization
                         │
                         ▼
                 Query Rewriting
                         │
                         ▼
            Query Clarification (if needed)
                         │
                         ▼
        Multi-Agent Parallel Retrieval
                         │
                         ▼
          Parent Context Reconstruction
                         │
                         ▼
             Context Compression
                         │
                         ▼
            Response Aggregation
                         │
                         ▼
                  Final Answer
```

---

# ⚙️ Tech Stack

### Programming Language

- Python

### Frameworks & Libraries

- LangGraph
- LangChain
- Gradio

### Vector Database

- Qdrant

### Observability

- Langfuse

### Supported LLM Providers

- OpenAI
- Anthropic
- Google Gemini
- Ollama
- OpenRouter
- Other LangChain-compatible providers

### Embedding Models

- Configurable embedding providers

---

# 🔄 Workflow

1. Upload one or more documents.
2. Split documents into hierarchical parent and child chunks.
3. Generate embeddings for child chunks.
4. Store embeddings in the Qdrant vector database.
5. Accept user queries.
6. Summarize previous conversation history.
7. Rewrite user queries for improved retrieval.
8. Request clarification for ambiguous queries when necessary.
9. Execute parallel retrieval through multiple specialized agents.
10. Retrieve parent context from matching child chunks.
11. Perform automatic self-correction if retrieved context is insufficient.
12. Compress retrieved context for efficient LLM prompting.
13. Aggregate agent responses into a single coherent answer.
14. Generate the final response.

---

# 📦 Installation

Clone the repository

```bash
git clone https://github.com/<your-username>/Multi-Agent-RAG-System-for-Intelligent-Document-Retrieval.git

cd Multi-Agent-RAG-System-for-Intelligent-Document-Retrieval
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
cd project

python app.py
```

---

# 💡 Applications

- Enterprise Knowledge Assistant
- Intelligent Document Search
- Internal Documentation Retrieval
- Research Paper Assistant
- Technical Documentation QA
- Policy & Compliance Search
- Customer Support Knowledge Base
- AI-powered Knowledge Management Systems

---

# 🔮 Future Enhancements

- REST API support
- React-based frontend
- User authentication and authorization
- Docker Compose deployment
- Streaming LLM responses
- Citation-aware answer generation
- RAG evaluation dashboard (RAGAS)
- Support for additional document formats
- Multi-user workspace management

---

# 🎯 Core Concepts Demonstrated

- Retrieval-Augmented Generation (RAG)
- Agentic AI Workflows
- LangGraph State Machines
- Hierarchical Document Indexing
- Hybrid Search
- Vector Databases
- Embedding Models
- Conversation Memory
- Query Rewriting
- Human-in-the-Loop Systems
- Context Compression
- Multi-Agent Orchestration

---
 
