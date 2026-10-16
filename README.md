# migration-rag-assistant

> RAG assistant that answers Lithuanian residence-permit and language-exam questions only from official sources, with citations, evals and an "I don't know" fallback.

![status](https://img.shields.io/badge/status-in%20development-yellow) ![license](https://img.shields.io/badge/license-MIT-green)

## Overview

An assistant that answers questions about Lithuanian residence permits and the state-language exam using only official sources — every answer cites its source, and it says "I don't know" when the sources don't cover the question.

## Features

- Ingestion of official pages (migracija.lt, nsa.smsm.lt) with source URLs and dates
- Hybrid search (vector + keyword) with reranking over pgvector
- Answers with citations to the exact source
- Refuses to guess when sources don't cover a question
- Evaluation set of real questions with expected sources
- FastAPI endpoint, simple web UI and tracing with Langfuse

## Tech stack

Python · FastAPI · PostgreSQL + pgvector · embeddings + LLM API · Langfuse · pytest

## License

[MIT](LICENSE) © Arman Salek
