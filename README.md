<h1 align="center">
  <a href="https://git.io/typing-svg">
    <img
      alt="Hello, I'm Raja Hussain"
      src="https://readme-typing-svg.herokuapp.com?lines=Hey%2C+I'm+Hussain;SWE+%26+Data+Engineer&center=true&size=26"
    />
  </a>
</h1>
<p align="center">
  CS & Math @ NYU | Building data systems and backend infrastructure
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

### Atlas Intel — Financial Data Pipeline & API
**Backend system that ingests SEC EDGAR filings and exposes structured financial data through a REST API.**
[Repo](https://github.com/Hussain0327/atlas-intel)

- Built async ingestion pipeline processing 13K+ companies from SEC EDGAR, parsing XBRL into normalized PostgreSQL tables
- Designed EAV data model and queryable REST API (FastAPI) supporting cross-company screening across 50+ metrics
- Handles 10-K/10-Q filings end-to-end: fetch, parse, store, serve

**Stack:** Python, FastAPI, PostgreSQL, async SQLAlchemy, Docker

---

### Freight Settlement Infrastructure — Investment Research System
**Automated research pipeline and scenario modeling engine for a crypto-native PE firm's diligence process.**
[Repo](https://github.com/Hussain0327/freight-settlement-infrastructure)

- Built Monte Carlo simulation engine with configurable scenario parameters for estimating settlement cost savings
- Structured data extraction pipeline from SEC 10-K filings to quantify $560M/year in payments friction
- Designed falsifiability-ranked diligence framework with programmatic sensitivity analysis

**Stack:** Python, pandas, NumPy, SEC EDGAR API

---

### Credit Risk Scoring Platform
**End-to-end ML pipeline from feature engineering to production-ready scoring outputs across 1.3M+ records.**
[Repo](https://github.com/Hussain0327/risk_modeling)

- Engineered 50+ features and built classification pipeline (Logistic Regression, GBM, XGBoost) with class weighting
- Validated on out-of-time holdout (0.72 ROC-AUC), mapped predicted probabilities to policy decision tiers
- Operationalized scoring outputs for downstream consumption

**Stack:** Python, scikit-learn, XGBoost, pandas, NumPy

---

### Scaling Laws for Small Language Models
**Independent research quantifying neural scaling behavior in the sub-1B parameter regime.**
[Repo](https://github.com/ValtricAI/Scaling-Laws-for-Small-Language-Models)

- Identified efficiency threshold at 350M parameters using power-law fitting (R² = 0.99)
- Documented statistical limitations transparently (n=4 sample size)

**Stack:** PyTorch, HuggingFace, MobileLLM

---

## Technical Skills

| Category | Tools |
|----------|-------|
| **Languages** | Python, SQL, Java, Go, R |
| **Backend & APIs** | FastAPI, REST API design, async programming, Linux, Docker, Git |
| **Data Infrastructure** | PostgreSQL, dbt, Prefect, AWS (S3, Redshift), data pipeline design |
| **ML & Analytics** | scikit-learn, XGBoost, PyTorch, pandas, NumPy, hypothesis testing |
| **Cloud & DevOps** | AWS, Docker, CI/CD, security fundamentals |

---

<p align="center">
  I build backend systems, data pipelines, and infrastructure that turns messy data into something useful.
</p>
