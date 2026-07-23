# RAG Bootcamp Projects

This repository documents hands-on projects built while learning and teaching Retrieval-Augmented Generation (RAG) using LangChain, LangGraph, and LangSmith. Each project explores a different RAG architecture, from foundational retrieval pipelines to more advanced agentic and graph-based approaches.

This work supports my broader research interest in applying LLM-based systems to security and threat intelligence contexts, particularly how retrieval-augmented architectures can be used to ground AI systems in verifiable, trustworthy information sources.

## Repository Structure

```
rag-bootcamp-projects/
│
├── 0_Embedding-Semantic-Similarities/ # Embedding generation and a mini semantic search engine
│
├── 1_DataIngestParsing/               # Document loading and parsing (PDF, Word, CSV/Excel, JSON, databases)
│
├── 2_Vector_Embeddings_And_DBs/       # Vector embeddings (HuggingFace, OpenAI) and similarity search
│
├── 3_Vector_Store_and_DBs/            # Vector stores with ChromaDB (native client + LangChain) and a RAG pipeline
│
├── main.py                            # Entry point for running core demos
├── pyproject.toml                     # Project dependencies (uv)
├── requirements.txt                   # Project dependencies (pip)
└── uv.lock                            # Locked dependency versions
```

Each project folder is self-contained with its own code, dependencies, and notes, allowing individual components to be run and studied independently.

## Topics Covered

- **Data Ingestion and Parsing** — loading and chunking documents for retrieval pipelines
- **Embeddings and Semantic Similarity** — generating vector embeddings and measuring semantic similarity between text passages
- **Traditional RAG** — standard retrieve-then-generate pipelines
- **Hybrid Search** — combining sparse (keyword-based) and dense (vector-based) retrieval methods
- **Multimodal Retrieval** — retrieval across text and non-text data sources
- **Agentic and Multi-Agent RAG** — pipelines where agents reason about what and when to retrieve
- **Corrective and Adaptive RAG** — pipelines that evaluate and self-correct retrieval quality
- **GraphRAG** — retrieval over structured knowledge graphs
- **Evaluation** — methods for assessing RAG pipeline performance and retrieval quality

## Setup

This project uses [uv](https://github.com/astral-sh/uv) for dependency management, with `requirements.txt` provided as an alternative for pip users.

```bash
# Using uv
uv sync

# Or using pip
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Running Projects

Each numbered project folder can be run independently. Navigate into the relevant folder and follow any project-specific instructions in its own notes.

```bash
cd 1_DataIngestParsing
```

## Tools and Frameworks

- **LangChain** — core framework for building LLM-powered pipelines
- **LangGraph** — for building agentic and multi-step RAG workflows
- **LangSmith** — for tracing, debugging, and evaluating pipeline runs

## Goals

- Build a practical, working understanding of RAG architectures from first principles to advanced patterns
- Document each approach clearly enough to teach it to others
- Apply RAG concepts toward trustworthy, verifiable AI systems relevant to security and threat intelligence use cases

## About

Hands-on RAG projects built while teaching Retrieval-Augmented Generation with LangChain, LangGraph, and LangSmith. Covers traditional RAG, hybrid search, multimodal retrieval, agentic and multi-agent pipelines, corrective/adaptive RAG, GraphRAG, and evaluation. Each project isolates its own code, dependencies, and notes.
