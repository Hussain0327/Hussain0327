# Raja Hussain · CS @ NJIT · Founder, ValtricAI

**Focus:** Applied AI agents, ML systems, and pragmatic SWE. Open to **AI/ML/SWE internships** for **Spring/Summer 2026**.

* Building **ValtricAI** — specialized AI agents for lead capture, compliance, and ops automation
* Current courses: CS 100, MATH 110, PSY 210, STS 201
* Interest areas: conversational AI, agent orchestration, retrieval systems, government + SMB workflows

## Skills

**Languages:** Python, JavaScript/TypeScript, SQL

**Frameworks/Tools:** FastAPI, Flask, Node.js, n8n, Supabase, Redis, Docker, GitHub Actions

**ML:** NumPy, pandas, scikit‑learn, basic fine‑tuning, vector search/RAG

**Cloud/Infra:** Supabase, Vercel/Netlify, GitHub Pages

## Selected Projects

> Live demos are ideal. Add links as you publish them.

* **ValtricAI (platform)** — Multi‑agent orchestration for lead recovery and compliance checks. FastAPI + n8n + Supabase.
  Repo: [https://github.com/Hussain0327/valtric-consulting-ai](https://github.com/Hussain0327/valtric-consulting-ai) (rename to `valtricai`)

* **Echo‑Lite (web app)** — Call‑to‑booking intake with calendar handoff and CRM sync.
  Stack: FastAPI, SQLite, basic auth, GitHub Pages demo.
  Repo: [https://github.com/Hussain0327/valtric-consulting](https://github.com/Hussain0327/valtric-consulting) (rename to `echo-lite`)

* **Riona Agent** — Website AI agent integration, prompt + routing logic clean‑up.
  Repo: [https://github.com/Hussain0327/riona](https://github.com/Hussain0327/riona)

* **Spark‑a‑Wish** — TypeScript demo with API integration and clean componentization.
  Repo: [https://github.com/Hussain0327/spark-a-wish-47](https://github.com/Hussain0327/spark-a-wish-47)

* **CS‑100 Exercises** — Intro CS practice and zyBooks‑aligned labs (kept tidy for recruiters).
  Repo: [https://github.com/Hussain0327/cs-100](https://github.com/Hussain0327/cs-100)

## Experience

* **Founder, ValtricAI** — building applied AI agents for service businesses and gov/SMB workflows. WIP pilots.

## Publications & Notes

* Short technical notes and experiments (RAG, agent routing, evaluation harnesses).
  Repo: [https://github.com/Hussain0327/projects](https://github.com/Hussain0327/projects) (add `notes/` folder with brief write‑ups)

## How I work

* Small, opinionated repos with clear READMEs, reproducible `make run`, and sample data.
* Ship weekly. Document decisions. Add tests as features stabilize.

## Contact

* Email: **[hello@valtricai.com](mailto:hello@valtricai.com)**
* LinkedIn: add your handle in your profile settings

---

### Repo Template (copy into each project’s README)

# <Project Name>

One‑sentence value statement. Example: “Echo‑Lite converts missed calls into booked meetings.”

**Stack:** FastAPI · SQLite · Docker · GitHub Actions
**Live demo:** <link or GitHub Pages URL>
**Status:** WIP / Alpha / Stable

## Quickstart

```bash
# 1) clone
git clone https://github.com/Hussain0327/<repo>.git && cd <repo>

# 2) set up env
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# 3) run
uvicorn app:app --reload
```

## Features

* \<feature 1>
* \<feature 2>

## Roadmap

* [ ] next feature
* [ ] tests + simple CI

## License

MIT

---

### Pinned Repos (suggested)

1. `valtricai` (rename from `valtric-consulting-ai` or `valtriAI/vaLTAI`) — platform
2. `echo-lite` (rename from `valtric-consulting`) — web intake app
3. `riona` — website agent
4. `spark-a-wish-47` — TypeScript demo (rename to `spark-a-wish`)
5. `projects` — notes + experiments (clean)
6. `cs-100` — coursework (optional pin)

---

### Profile Bio (paste into GitHub Settings → Bio)

CS @ NJIT • Founder, ValtricAI. I build applied AI agents and pragmatic SWE. Open to AI/ML/SWE internships (Spring/Summer 2026).

### Topics to add to repos

`python` `fastapi` `n8n` `supabase` `redis` `llm` `rag` `ml` `typescript` `docker` `github-actions`

### Badges (optional)

Add these to each repo README after Quickstart:

* Build: ![CI](https://img.shields.io/badge/CI-GitHub_Actions-informational)
* License: ![MIT](https://img.shields.io/badge/License-MIT-green)

### Simple CI (drop in `.github/workflows/ci.yml`)

```yaml
name: CI
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-python@v5
        with:
          python-version: '3.12'
      - run: pip install -r requirements.txt || true
      - run: pytest || echo "no tests yet"
```
