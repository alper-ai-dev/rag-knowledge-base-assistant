# Atlas — Knowledge Retrieval & Grounded Answer Demo

A source-grounded enterprise knowledge retrieval demo built as a portfolio project by Alper Sancar.

## Architecture
1. Knowledge documents are split into passages.
2. Client-side TF-IDF-style lexical scoring ranks passages against the user's question.
3. Relevant source sentences are selected from the top retrieved passages.
4. A deterministic demo answer is assembled from those sentences with visible source references.

## Features
- Editable local knowledge base
- Document chunking
- Stop-word filtering and lexical retrieval
- IDF-weighted relevance ranking
- Top-k context selection
- Deterministic source-grounded demo answers
- Visible retrieved source labels
- Responsive enterprise UI
- No API key required

## Stack
HTML5, CSS3, Vanilla JavaScript, browser LocalStorage.

## Scope and accuracy
This public portfolio version demonstrates the retrieval and grounding stages used in RAG-style systems. It does **not** use an LLM, vector database or embedding model, and does not claim to. Added documents persist in the current browser only. A production version could connect the retrieved context to an LLM and vector database.

## Portfolio
Built by Alper Sancar to demonstrate document chunking, information retrieval, grounding, knowledge-oriented product design and RAG pipeline concepts.