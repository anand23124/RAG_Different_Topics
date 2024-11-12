# Reranking Exploration for Enhanced Document Retrieval

## Overview
This project delves into reranking techniques aimed at improving document retrieval quality. It serves as an exploration of different reranking methods in the context of RAG (Retrieval-Augmented Generation) without fully implementing RAG.

## Project Structure
1. **Initial Ranking** - A first-pass ranking is performed using `SentenceTransformer`, a transformer-based model suited for capturing semantic similarity.
2. **Reranking** - The ranked results are then refined using a layered reranking approach:
   - **BM25** - A classic ranking function based on term frequency, useful for text search.
   - **CrossEncoder** - Refines ranking by evaluating the relevance of each document relative to the query.
   - **Cohere API** - Adds an additional semantic reranking layer to ensure precision.

## Key Concepts
- **Reranking** - By layering multiple reranking methods, the project highlights the potential to improve retrieval quality without directly implementing a RAG setup.
- **Exploration of Reranking Methods** - Showcases the application of different ranking models to optimize search results.