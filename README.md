# Hi, I'm Michelle Han 👋

I'm a Master's student in Computer and Information Science at the University of Pennsylvania.

- 🎓 MSE in Computer and Information Science, University of Pennsylvania
- 📐 B.A. in Applied Mathematics & Computer Science, minor in Psychology and Brain Sciences, Washington University in St. Louis
- 🔭 Currently building projects in backend engineering, AI Agents, and applied ML
- 🌱 Interested in software engineering, machine learning, and AI systems
- 📫 Reach me on [LinkedIn](www.linkedin.com/in/michellehan7) or at hanmich@engineering.upenn.edu


## 🚀 Featured Projects

### 🔥 [HeatOps](https://github.com/MichelleHan7/HeatOps) — Heat-aware field-crew scheduling
[![CI](https://github.com/MichelleHan7/HeatOps/actions/workflows/ci.yml/badge.svg)](https://github.com/MichelleHan7/HeatOps/actions/workflows/ci.yml)
· [**Live demo**](https://heatops-fortyguard.streamlit.app/) · FortyGuard Hackathon '26

Multi-crew scheduler that assigns utility jobs to qualified crews while trading off workers' heat exposure against operational delay.

- **OR-Tools CP-SAT** model scheduling up to **100 jobs across 10 heterogeneous crews** under skill, shift, time-window, availability, and non-overlap constraints, with an independent validator checking every returned schedule
- Four scheduling policies evaluated on **165 seeded scenarios**; heat-first achieved an **8.47% mean reduction** in modeled heat load, with timeouts and added delay reported alongside it
- Pluggable weather providers (**Strategy pattern**) normalizing FortyGuard GeoJSON heatmaps and Open-Meteo time series, with live → cache → offline-snapshot fallback
- **160+ pytest tests**, Ruff lint/format, and CLI smoke tests in **GitHub Actions** across Python 3.11 / 3.12

`Python` · `OR-Tools` · `Streamlit` · `Pytest` · `GitHub Actions`

### 🧪 [ClinTrialSync](https://github.com/MichelleHan7/ClinTrialSync) — Clinical-trial data platform

Backend that unifies clinical-trial records and imaging-scan metadata behind one versioned API, replacing ad-hoc SQL queries by lab staff.

- ✅ **Spring Boot** REST service on **PostgreSQL** with **Flyway** schema migrations and JPA
- ✅ Containerized local environment with **Docker Compose** and health-checked Postgres
- 🚧 OpenAPI-documented, versioned endpoints for trials and scan metadata
- 🚧 **Kafka** topics decoupling ingestion from validation and analytics consumers
- 🚧 **Redis**-cached patient-cohort summaries, precomputed on every data update

`Java` · `Spring Boot` · `PostgreSQL` · `Flyway` · `Kafka` · `Redis` · `Docker`

### 🧠 LLM Transcript Scoring — WashU Dynamic Cognition Lab
*Research code; private because it contains participant data.*

Replaced manual scoring of participants' recall transcripts against 200+-item checklists, cutting scoring time from **~15 min to ~30 s per participant**.

- **FastAPI** service with the **OpenAI API** and **PostgreSQL**; **Celery + Redis** fan-out across 600+ transcripts with `asyncio`-bounded concurrency and backoff on rate limits
- Two-stage **RAG**: bi-encoder retrieval in **pgvector**, then cross-encoder reranking to select few-shot examples; **Pydantic**-validated JSON output with quoted transcript evidence
- Evaluation harness benchmarking models against human consensus, with **GitHub Actions** regression checks on every prompt change and **Langfuse** tracing for failure analysis

`Python` · `FastAPI` · `LLMs` · `RAG` · `pgvector` · `Celery` · `Langfuse`

---

## 🛠️ Tech Stack

[![Tech stack](https://skillicons.dev/icons?i=python,java,js,ts,cpp,go,spring,nodejs,express,fastapi,react,nextjs,postgres,mysql,redis,kafka,mongodb,docker,kubernetes,aws,githubactions,linux,pytorch,tensorflow&perline=12)](https://skillicons.dev)

| Area | Tools |
|---|---|
| **Languages** | Python, Java, JavaScript, TypeScript, C++, Go, SQL, R |
| **Backend** | Spring Boot, Node.js, Express, FastAPI, REST APIs, Celery, Pydantic |
| **Data & Messaging** | PostgreSQL, MySQL, Redis, Kafka, MongoDB, pgvector |
| **Cloud & DevOps** | Docker, Kubernetes, AWS (EC2, S3, Lambda), GitHub Actions, Linux |
| **AI / ML** | OpenAI API, LangChain, LangGraph, Langfuse, Hugging Face, PyTorch, TensorFlow, scikit-learn |
| **Testing** | pytest, JUnit, Jest, k6 |

