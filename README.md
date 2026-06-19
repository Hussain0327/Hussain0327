# Raja Hussain

CS & Econ @ NYU. I build grounded, auditable AI systems: retrieval and LLM tooling that cites its sources, refuses when it can't, and gates on evals.

The thread across my work is evidence over guesswork. Answers trace to a source or never get made, extraction ties every claim to where it came from, and LLM behavior is tested in CI like any other code.

[Website](https://raja-builds-ai.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/raja-hussain-ai) · [ValtricAI](https://valtricai.com/) · rajahh7865@gmail.com

## Projects

### REGWATCH: Grounded Regulatory Intelligence
A RAG system that turns a multi-day FDA research task into cited answers in minutes. Built during my 2026 internship for a generic-drug Clinical Regulatory Affairs team. Private repo. [Read the case study](CASE_STUDY_LINK)

- Citation-or-refuse by design: every answer carries a source and page or an explicit "not found," enforced as tested invariants, not prompt guidelines
- Synthesizes six FDA sources (Orange Book, Drugs@FDA, DailyMed, Shortages, REMS, Product-Specific Guidances), resolving the product before retrieval so a citation can never cross drugs
- Graded in CI against a gold set with hard gates on recall@k, citation precision, and refusal accuracy before any merge
- Python, FastAPI, ChromaDB/pgvector, SQLModel, Dagster, Next.js/TypeScript

### CloudSearch: Hybrid Search Backend
A low-latency Go service that fuses vector and keyword retrieval with SSE streaming. [Repo](LINK)

- Hybrid retrieval (pgvector cosine + tsvector) fused via Reciprocal Rank Fusion, hitting 100% recall@5 on a 24-query suite
- Go API on Chi with goroutine fan-out, a two-level LRU cache, and per-IP rate limiting for concurrent queries
- Python ingestion with BFS crawling, type-aware chunking, BGE-large embeddings, and SHA-256 dedup on upsert
- Go, Python, PostgreSQL, pgvector, Ollama, Docker

### Atlas Intel: SEC EDGAR Data Platform
An async ingestion pipeline and REST API serving normalized XBRL data for 13K+ public companies. [Repo](LINK)

- End-to-end async ingestion of 10-K and 10-Q filings: fetch, parse, store, serve
- EAV data model with FastAPI endpoints for cross-company screening across 50+ financial metrics
- Python, FastAPI, PostgreSQL, async SQLAlchemy, Docker

### Inversion Thesis Engine: Document Intelligence Backend
A FastAPI service that ingests deal documents and surfaces auditable diligence risks. [Repo](LINK)

- Rule-based contradiction detection that links every flag back to source text via auditable evidence chains
- Claude API structured extraction from CIMs and financial statements over a Postgres deal and document model
- Deterministic EBITDA bridge calculator with base, downside, and partial-adoption scenarios
- Python, FastAPI, PostgreSQL, Claude API, PyMuPDF

### EvidentAI: Open-Source LLM Eval and Security CLI
A CI/CD-friendly evaluation suite and runtime gateway for LLM applications (co-authored). [Repo](LINK) · [npm](LINK)

- Six built-in evaluators including LLM-judge, PII detection, and prompt-injection checks, with 211 passing tests
- A CLI that runs eval suites inside CI/CD, plus a gateway proxy for runtime protection
- TypeScript, Node.js, Python

## Skills

| Area | Tools |
| --- | --- |
| Languages | Python, Go, SQL, TypeScript |
| Backend | FastAPI, Chi, asyncpg, SQLAlchemy, Alembic, REST, SSE |
| Data | PostgreSQL, pgvector, ETL and ingestion pipelines, vector search |
| AI/ML | RAG, embeddings (sentence-transformers / BGE), LLM evaluation, Ollama |
| Infra | Docker, GitHub Actions, CI/CD |
