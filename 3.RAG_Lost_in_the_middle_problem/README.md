# Enhancing RAG with MergerRetriever and LongContextReorder

## Overview
This project addresses the "Lost in Middle Phenomenon" in Retrieval-Augmented Generation (RAG), where essential information in long contexts can get overlooked. By merging retrievers and optimizing context ordering, this project enhances RAG's relevance and accuracy.

## Approach
1. **Vector Storage and Retrieval**:
   - **ChromaDB** - Used as the primary vector storage and retrieval system.
   - **Hugging Face embeddings** - Created embeddings to represent document semantics accurately.

2. **Merging and Context Optimization**:
   - **MergerRetriever** - Merges multiple retrievers to unify and enhance retrieval results.
   - **LongContextReorder** - Utilizes a combination of:
     - **EmbeddingsClusteringFilter**
     - **EmbeddingsRedundantFilter**
     - **LongContextReorder**

3. **Model and Chain Setup**:
   - **Llama Zephyr-7b-beta** - Loaded via **Llama.cpp** from a local drive.
   - **Retrieval Chain** - Built using **LangChain** for inference, providing highly relevant results surpassing the standard RAG pipeline.

## Key Takeaways
- **Mitigates Lost in Middle Phenomenon** - Ensures that critical information within long contexts is accurately retrieved.
- **Enhanced Relevance** - By merging retrievers and reordering contexts, retrieval quality is significantly improved.
