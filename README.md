# langchain-projects

This repository contains experiments and sample projects using [LangChain](https://github.com/langchain-ai/langchain) for building LLM-powered applications, including Retrieval-Augmented Generation (RAG) pipelines.

## Features

- **Chat with OpenAI models** using LangChain's `ChatOpenAI`
- **Document loading and splitting** (PDFs, text)
- **Embeddings generation** with OpenAI models
- **Vector storage and retrieval** using Pinecone
- **Retrieval-Augmented Generation (RAG)** with LangChain's `RetrievalQA` chain

## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/langchain-projects.git
   cd langchain-projects
   ```

2. **Install dependencies:**
   ```bash
   poetry install
   # or, if using pip:
   pip install -r requirements.txt
   ```

3. **Set environment variables:**
   - `OPENAI_API_KEY` for OpenAI access
   - `PINECONE_API_KEY` for Pinecone access

4. **Activate your virtual environment:**
   ```bash
   poetry shell
   ```

## Usage

- Run Jupyter notebooks for interactive experiments:
  ```bash
  jupyter notebook
  ```
- Example notebooks:
  - `chat_model.ipynb`: Basic chat with OpenAI models
  - `rag.ipynb`: Full RAG pipeline with PDF ingestion, chunking, embedding, and retrieval

## Notes

- Adjust chunk sizes in text splitters to avoid Pinecone's per-vector and per-request size limits.
- Ensure your embedding model's output dimension matches your Pinecone index dimension.
