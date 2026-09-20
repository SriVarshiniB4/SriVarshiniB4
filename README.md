# Hi, I'm Sri Varshini 👋

Final-year CS (AI & ML) undergraduate building production-oriented backend systems in Java and Python. I like understanding how things actually work under the hood — concurrency control, distributed systems, RAG pipelines — not just calling a library and moving on.

Currently looking for **backend / systems engineering roles**.

📫 srivarshinib04@gmail.com

---

## Featured projects

### 🧵 [Distributed Job Scheduler + Observability Dashboard](https://github.com/SriVarshiniB4/job-scheduler)
A Postgres-backed distributed job queue with lease-based fault tolerance and a live React dashboard.
- Safe concurrent job claiming across multiple workers via `FOR UPDATE SKIP LOCKED` — verified with 8 concurrent worker processes against 500 jobs, 0 duplicate executions
- Automatic crash recovery via a renewable lease/heartbeat mechanism, verified with chaos testing (hard-killing a worker mid-job)
- Live job/worker state streamed to a React dashboard via Postgres `LISTEN`/`NOTIFY` → Server-Sent Events, zero polling
- `Python · FastAPI · PostgreSQL · SQLAlchemy (async) · React · SSE`

### 📄 [AI-Powered Document Q&A Platform](https://document-qa-platform-phi.vercel.app/)
A multi-user RAG platform with real cost tracking and quota enforcement, not just an API wrapper.
- PDF parsing, chunking (1500 chars / 150 overlap), embeddings via `gemini-embedding-001`, retrieval via `pgvector` cosine similarity
- Per-user token quota enforcement (Bucket4j + Redis) with real-time USD cost tracking at Gemini's published pricing
- Secured with Spring Security + JWT, stateless filter chain, multi-user isolation
- `Spring Boot · Spring AI · React · PostgreSQL/pgvector · Gemini API · Redis`

### 🧠 Neurological Disease Detection — Alzheimer's & Parkinson's
Two modality-appropriate ML pipelines: CNN on spiral/wave motor-drawing images for Parkinson's, and linguistic-feature classification on speech transcripts for Alzheimer's.
- Strict patient-level train/test splits throughout, avoiding the data-leakage failure mode common in public tutorials on these datasets
- `Python · TensorFlow · Scikit-learn · CNN`

---

## Tech I work with

**Languages:** Java, Python, C, SQL
**Backend:** Spring Boot, FastAPI, SQLAlchemy (async), REST APIs, JWT, WebSocket/STOMP
**AI/ML:** RAG pipelines, pgvector, Scikit-learn, CNN
**Frontend:** React (Vite), JavaScript
**Databases:** PostgreSQL, MySQL, MongoDB
**Tools:** Git, Docker, Redis, Postman

---

*Secretary, Q Club (Quantum Computing) · Member, Amura (AI/ML Club) — RNS Institute of Technology*
