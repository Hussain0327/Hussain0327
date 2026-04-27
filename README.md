<h1 align="center">
  <a href="https://git.io/typing-svg">
    <img
      alt="Hello, I'm Raja Hussain"
      src="https://readme-typing-svg.herokuapp.com?lines=Hey%2C+I'm+Hussain;Backend+%26+Distributed+Systems&center=true&size=26&width=600"
    />
  </a>
</h1>
<p align="center">
  CS & Econ @ NYU | Building backend systems, data infrastructure, and AI tooling
</p>
<p align="center">
  <a href="mailto:rajahh7865@gmail.com">
    <img alt="Email" src="https://img.shields.io/badge/Email-rajahh7865@gmail.com-1d72b8?logo=gmail&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/raja-hussain-ai/">
    <img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-raja--hussain-blue?logo=linkedin&logoColor=white" />
  </a>
</p>

---

## Projects

### CloudSearch — Hybrid Search Backend
**Low-latency Go search service combining vector and keyword retrieval with SSE streaming.**
[Repo](https://github.com/Hussain0327/cloudsearch)

- Built a Go API server (Chi) with goroutine fan-out, two-level LRU cache (15min TTL), and per-IP rate limiting for concurrent vector and keyword query handling
- Implemented hybrid retrieval (pgvector cosine + tsvector keyword) fused via Reciprocal Rank Fusion, hitting 100% recall@5 on a 24-query test suite
- Engineered a Python ingestion pipeline with BFS crawling, type-aware chunking (prose/code/table/config), BGE-large embeddings, and SHA-256 content hashing for deduplicated upserts

**Stack:** Go, Python, PostgreSQL, pgvector, Ollama, Docker

---

### Atlas Intel — SEC EDGAR Data Platform
**Async ingestion pipeline and REST API serving normalized XBRL data for 13K+ public companies.**
[Repo](https://github.com/Hussain0327/atlas-intel)

- Built async ingestion processing 10-K and 10-Q filings end-to-end (fetch, parse, store, serve)
- Designed EAV data model and queryable FastAPI endpoints supporting cross-company screening across 50+ metrics
- Containerized with Docker; PostgreSQL with async SQLAlchemy under the hood

**Stack:** Python, FastAPI, PostgreSQL, async SQLAlchemy, Docker

---

### Inversion Thesis Engine — Document Intelligence Backend
**FastAPI service that ingests deal documents and surfaces auditable diligence risks.**
[Repo](https://github.com/Hussain0327/inversion-thesis-engine)

- Designed a PostgreSQL data model for deals, documents, and extracted metrics, powered by Claude API for structured extraction from CIMs and financial statements
- Implemented rule-based contradiction detection that links every flag to source text via auditable evidence chains
- Built a deterministic EBITDA bridge calculator with configurable assumptions for base, downside, and partial-adoption scenarios

**Stack:** Python, FastAPI, PostgreSQL, Claude API, PyMuPDF

---

### EvidentAI — Open-Source LLM Eval & Security CLI
**CI/CD-friendly evaluation suite and runtime gateway for LLM applications.**
[Repo](https://github.com/Hussain0327/evidentai) | [npm](https://www.npmjs.com/package/evidentai)

- Co-authored an open-source platform shipping 6 built-in evaluators (exact match, LLM judge, PII detection, prompt injection, custom) with 211 passing tests
- Built a CLI that runs evaluation suites in CI/CD pipelines and a gateway proxy for runtime protection

**Stack:** TypeScript, Node.js, Python, npm

---

## Technical Skills

| Category | Tools |
|----------|-------|
| **Languages** | Python, Go, SQL, Java, TypeScript |
| **Backend** | FastAPI, Chi, asyncpg, SQLAlchemy, Alembic, REST, SSE |
| **Data & Warehousing** | ETL/ELT, dbt, Prefect, star schema, CDC, PostgreSQL, pgvector, Redshift |
| **Infrastructure** | AWS (S3, Redshift), Docker, Kubernetes, Kafka, Redis, GitHub Actions, CI/CD |
| **AI/ML** | RAG, sentence-transformers, LLM evaluation, scikit-learn, XGBoost, Ollama |

---

<p align="center">
  Building backend systems and the data + AI plumbing around them.
</p>
