# migration-rag-assistant

> RAG assistant that answers Lithuanian residence-permit and language-exam questions only from official sources, with citations, evals and an "I don't know" fallback.

![status](https://img.shields.io/badge/status-in%20progress-yellow) ![area](https://img.shields.io/badge/area-AI%20Engineering-blue) ![license](https://img.shields.io/badge/license-MIT-green)

🚧 **Work in progress.** This repo is part of my public learning roadmap (**Phase 4 — AI engineering**). I build in the open — follow the commits and the roadmap below.

## Why this project

Build retrieval-augmented generation responsibly for a real audience: foreigners in Lithuania who need correct answers, always backed by an official source.

## What I'm learning

- Document ingestion and chunking
- Embeddings and vector search with pgvector
- Hybrid search + reranking
- Grounded answers with citations and refusal when unsure
- Evaluation sets for retrieval and answer quality
- Observability with Langfuse

## Planned stack

Python · FastAPI · PostgreSQL + pgvector · embeddings + LLM API · Langfuse · pytest

## Roadmap

- [ ] Ingest official pages (migracija.lt, nsa.smsm.lt) with source URLs and dates
- [ ] Chunking + embeddings into pgvector
- [ ] Retrieval with hybrid search and reranking
- [ ] Answers with citations; "I don't know" when sources don't cover it
- [ ] Eval set of real questions with expected sources
- [ ] FastAPI endpoint + simple web UI
- [ ] Scheduled re-ingestion when sources change
- [ ] README: architecture, eval scores and limitations

## Part of a 10-repo learning roadmap

I'm a full-stack developer in Vilnius ([armansalek.com](https://armansalek.com)) growing into **Python, Go, DevOps, cloud and AI engineering**. These repos connect: the Python and Go services are containerised, deployed and monitored by the DevOps and cloud repos, and the AI projects run on that infrastructure.

| # | Repo | Area | Phase |
|---|---|---|---|
| 1 | [lt-jobs-scraper](https://github.com/arman-aru/lt-jobs-scraper) | Python | 1 |
| 2 | [lt-vocab-api](https://github.com/arman-aru/lt-vocab-api) | Python | 1 |
| 3 | [parcel-locker-api](https://github.com/arman-aru/parcel-locker-api) | Golang | 1 |
| 4 | [go-uptime](https://github.com/arman-aru/go-uptime) | Golang | 1 |
| 5 | [ci-cd-pipelines](https://github.com/arman-aru/ci-cd-pipelines) | DevOps | 2 |
| 6 | [k8s-gitops-lab](https://github.com/arman-aru/k8s-gitops-lab) | DevOps | 2 |
| 7 | [terraform-aws-platform](https://github.com/arman-aru/terraform-aws-platform) | Cloud Computing | 3 |
| 8 | [serverless-media-pipeline](https://github.com/arman-aru/serverless-media-pipeline) | Cloud Computing | 3 |
| 9 | [site-audit-agent](https://github.com/arman-aru/site-audit-agent) | AI Engineering | 4 |
| 10 | **migration-rag-assistant** (this repo) | AI Engineering | 4 |

## License

[MIT](LICENSE) © Arman Salek
