# RAG System - PDF Question Answering

A Retrieval-Augmented Generation (RAG) system that answers questions from PDF documents using LangChain and OpenAI.

## What This Does

This system allows you to:
- Upload any PDF document
- Ask questions about its content
- Get accurate answers with page number citations

## How It Works

1. **Loads** your PDF document
2. **Splits** text into smart chunks (1000 characters with 200 overlap)
3. **Creates embeddings** using OpenAI
4. **Stores** vectors in ChromaDB for fast search
5. **Retrieves** relevant chunks when you ask a question
6. **Answers** using GPT-4o-mini with source citations

## Quick Start

### 1. Install Requirements
```bash
pip install -r requirements.txt
