# Atlas — RAG Knowledge Base Assistant

A source-grounded enterprise knowledge assistant built as a portfolio project by Alper Sancar.

## Architecture
Atlas implements a compact Retrieval-Augmented Generation pipeline rather than sending the entire knowledge base to an LLM.

1. Knowledge documents are split into passages.
2. Client-side TF-IDF-style lexical scoring ranks passages against the user's question.
3. Only the top retrieved passages are sent to the serverless generation endpoint.
4. The LLM is instructed to answer only from retrieved context and cite source numbers.
5. The UI displays the source documents associated with the retrieved passages.

## Features
- Editable local knowledge base
- Document chunking
- Stop-word filtering and lexical retrieval
- IDF-weighted relevance ranking
- Top-k context selection
- Source-grounded OpenRouter generation
- Inline source-number prompting
- Visible retrieved source labels
- Responsive enterprise UI
- Server-side API key protection

## Stack
HTML5, CSS3, Vanilla JavaScript, Vercel Serverless Functions, OpenRouter API, browser LocalStorage.

## Environment variables
- `OPENROUTER_API_KEY` — required
- `OPENROUTER_MODEL` — optional; defaults to `openai/gpt-4.1-mini`

## Scope and accuracy
This is a portfolio RAG demonstration. Retrieval uses local lexical TF-IDF-style ranking, not a vector database or embedding model. Added documents persist in the current browser only. It is not presented as a production multi-user knowledge platform.

## Portfolio
Built by Alper Sancar to demonstrate retrieval, grounding, RAG architecture, serverless AI integration and knowledge-oriented product design.