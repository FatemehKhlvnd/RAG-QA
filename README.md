# RAG-based Document Question Answering

This project implements a simple Retrieval-Augmented Generation (RAG) pipeline for question answering over documents.

## Overview

The system combines:

- Text chunking
- Sentence embeddings
- Vector search using FAISS
- Context-aware answer generation using a Transformer model
- Basic retrieval evaluation metrics

## Architecture

1. Documents are split into chunks.
2. Each chunk is converted into embeddings using Sentence-Transformers.
3. FAISS is used for similarity-based retrieval.
4. Top-k relevant chunks are passed to a generation model (FLAN-T5).
5. The system returns an answer with citations.

## Tech Stack

- Python
- Sentence-Transformers
- FAISS
- Hugging Face Transformers
- NumPy

## Example Features

- Vector-based document retrieval
- Citation-based answer generation
- Precision@k / MRR evaluation (optional extension)

## How to Run

Install dependencies:

```bash
pip install faiss-cpu sentence-transformers transformers accelerate
