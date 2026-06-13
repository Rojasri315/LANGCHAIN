# LangChain RAG Pipeline

A Retrieval-Augmented Generation (RAG) project built using LangChain, ChromaDB, and document loaders. This project demonstrates how to load documents, split text into chunks, generate embeddings, store vectors in a vector database, and retrieve relevant context for question answering.

## Features

* Load documents from text files and web pages
* Split documents into manageable chunks
* Generate embeddings
* Store embeddings in Chroma Vector Database
* Semantic similarity search
* Retrieval-Augmented Generation (RAG) workflow
* Modular LangChain architecture

## Tech Stack

* Python 3.10
* LangChain
* ChromaDB
* LangChain Community
* LangChain OpenAI
* LangChain Ollama
* BeautifulSoup4
* Jupyter Notebook

## Project Structure

```text
LANGCHAIN/
│
├── rag/
│   ├── simplerag.ipynb
│   ├── speech.txt
│   └── research_paper.pdf
│
├── requirements.txt
├── README.md
└── .gitignore
```

## RAG Pipeline

```text
Documents
    ↓
Document Loader
    ↓
Text Splitter
    ↓
Embeddings
    ↓
Chroma Vector Store
    ↓
Retriever
    ↓
LLM
    ↓
Generated Response
```

## Workflow

### 1. Load Documents

Supported loaders:

* TextLoader
* WebBaseLoader
* PDF Loaders

### 2. Split Documents

Documents are divided into smaller chunks using LangChain text splitters to improve retrieval quality.

### 3. Generate Embeddings

Embeddings convert text into vector representations.

Options explored:

* OpenAI Embeddings
* Ollama Embeddings (planned)

### 4. Store in Chroma

Embeddings are stored in ChromaDB for efficient similarity search.

### 5. Retrieve Relevant Context

The retriever finds the most relevant document chunks for a user query.

### 6. Generate Answers

The retrieved context can be passed to an LLM for context-aware responses.

## Installation

Clone the repository:

```bash
git clone https://github.com/Rojasri315/LANGCHAIN.git
cd LANGCHAIN
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate the environment:

### Windows

```bash
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Current Status

* Document Loading: Completed
* Text Splitting: Completed
* Chroma Vector Database: Completed
* Embeddings: In Progress
* Ollama Integration: Pending Local Setup
* End-to-End RAG Pipeline: In Progress

## Learning Outcomes

This project helped me understand:

* Vector Databases
* Embeddings
* Semantic Search
* Retrieval-Augmented Generation (RAG)
* LangChain Components
* Document Processing Pipelines

## Future Improvements

* Integrate Ollama local models
* Add PDF ingestion
* Build a conversational RAG chatbot
* Add Streamlit frontend
* Deploy as a web application

## Author

**Rojasri**

Learning and exploring Generative AI, LangChain, RAG systems, and LLM application development.
