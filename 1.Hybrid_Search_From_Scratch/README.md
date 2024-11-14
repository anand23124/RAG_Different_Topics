# Exploring Hybrid Search and Reranking in RAG Context

## Overview
This project explores hybrid search techniques within the Retrieval-Augmented Generation (RAG) framework. While it doesn't fully implement RAG, it focuses on combining multiple search strategies for optimized document retrieval.

## Project Structure
1. **Hybrid Search Implementation**:
   - **ChromaDB** + **BM25Retriever** - A custom-built hybrid search from scratch that combines vector similarity with traditional keyword search.
   - **Weaviate** - Utilized Weaviate's native support for hybrid search, providing a seamless and efficient retrieval experience.

2. **Reranking with Cohere API**:
   - After initial retrieval, documents are reranked using the Cohere API to enhance relevance based on semantic similarity.

## Key Concepts
- **Hybrid Search** - Combines vector-based and keyword-based retrieval methods for more accurate results, essential in RAG.
- **Reranking** - Refines initial results by prioritizing relevance, showcasing how reranking adds value in RAG pipelines.

