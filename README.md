<div align="center">

<img src="assets/snake.svg" alt="snake" width="100%"/>

**[▶ Play it](https://Hussain0327.github.io/Hussain0327/)** · arrows to move, space to pause

# Raja Hussain

CS & Econ @ NYU. I build AI systems that show their work: retrieval and LLM tools that cite sources, say "I don't know" when they should, and get tested before they ship.

Every project here follows the same rule: an answer is only as good as what it points back to.

[Website](https://raja-builds-ai.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/raja-hussain-ai) · rajahh7865@gmail.com

</div>

---

## Projects                            

### REGWATCH — Regulatory RAG System                            

Built during my 2026 internship for a pharma regulatory affairs team. Turns a research task that used to take days into cited answers in minutes. Private repo. [Case study](CASE_STUDY_LINK)                            

- Every answer comes with a source and page, or an honest "not found" — enforced by tests, not just prompted                            
- Pulls from six FDA databases (Orange Book, Drugs@FDA, DailyMed, and others), locking in the right product before retrieval so citations never mix up drugs                            
- Runs through a CI eval gate checking recall, citation accuracy, and refusal behavior before anything merges                            
- Python, FastAPI, ChromaDB/pgvector, SQLModel, Dagster, Next.js/TypeScript                            

### CloudSearch — Hybrid Search Backend                            

A fast Go service combining vector and keyword search with live streaming results. [Repo](LINK)                            

- Combines pgvector and keyword search using Reciprocal Rank Fusion, hitting 100% recall@5 on a 24-query test set                            
- Go API with goroutine fan-out, a two-level cache, and per-IP rate limiting                            
- Python ingestion pipeline with crawling, smart chunking, and dedup on upsert                            
- Go, Python, PostgreSQL, pgvector, Ollama, Docker                            

### Atlas Intel — SEC EDGAR Data Platform                            

An async pipeline and API serving normalized financial data for 13K+ public companies. [Repo](LINK)                            

- Full pipeline from raw SEC filings to a queryable API                            
- Cross-company screening across 50+ financial metrics                            
- Python, FastAPI, PostgreSQL, async SQLAlchemy, Docker                            

### Inversion Thesis Engine — Document Intelligence Backend                            

A service that ingests deal documents and flags diligence risks, with every flag traceable to source text. [Repo](LINK)                            

- Contradiction detection that links every flag back to the original document                            
- Structured extraction from deal documents using the Claude API                              
- Deterministic financial modeling with base, downside, and partial-adoption scenarios               
- Python, FastAPI, PostgreSQL, Claude API, PyMuPDF                

### EvidentAI — Open-Source LLM Eval & Security CLI

A CI/CD-friendly eval suite and runtime gateway for LLM apps (co-authored). [Repo](LINK) · [npm](LINK)                                

- Six built-in evaluators (LLM-judge, PII detection, prompt-injection checks), backed by 211 passing tests          
- CLI for running evals in CI/CD, plus a gateway for runtime protection              
- TypeScript, Node.js, Python        

## Skills

| Area | Tools |
| --- | --- |
| Languages | Java, Python, Go, SQL, TypeScript |              
| Backend | FastAPI, Chi, asyncpg, SQLAlchemy, Alembic, REST, SSE |              
| Data | PostgreSQL, pgvector, ETL pipelines, vector search |              
| AI/ML | RAG, embeddings, LLM evaluation, Ollama |            
| Infra | Docker, GitHub Actions, CI/CD |                    
