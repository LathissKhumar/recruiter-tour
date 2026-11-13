# 🎯 Recruiter Tour — PK Lathiss Khumar

> **A guided walkthrough of my best work for hiring managers and recruiters**  
> *Designed to be read in 5–10 minutes — each project has: problem, approach, tech, results, and a "what I'd do next" section*

---

## 👤 Quick Profile

| | |
|---|---|
| **Name** | PK Lathiss Khumar |
| **Target Role** | Software Engineering Intern / AI Software Engineer Intern |
| **Graduation** | B.E. CSE, May 2028 (Chennai Institute of Technology) |
| **CGPA** | 8.29 / 10.0 |
| **Location** | Chennai, India • Open to Remote / Relocation |
| **LeetCode** | 650+ problems |
| **Key Differentiator** | Production-shaped AI systems (RAG, agents, evaluation) — not just notebooks |

**LinkedIn:** [linkedin.com/in/lathisskhumar](https://linkedin.com/in/lathisskhumar)  
**Email:** [pklathisskhumar.cse2024@citchennai.net](mailto:pklathisskhumar.cse2024@citchennai.net)  
**GitHub:** [github.com/LathissKhumar](https://github.com/LathissKhumar)

**Repo Links:** [AgencyOS-](https://github.com/LathissKhumar/AgencyOS-) • [RAG_PIPELINE](https://github.com/LathissKhumar/RAG_PIPELINE) • [CanonPulse](https://github.com/LathissKhumar/CanonPulse) • [DepthWizard](https://github.com/LathissKhumar/DepthWizard)

---

## 🗂️ Project Index

| # | Project | Type | Key Tech | Why It Matters |
|---|---------|------|----------|----------------|
| 1 | **AgencyOS** | Self-directed | LangGraph, A2A, FastAPI, PostgreSQL | 5-microservice agentic platform with self-healing — full stack AI engineering |
| 2 | **RAG Document QA** | Self-directed | LlamaIndex, ChromaDB, MiniLM, BM25 | Production RAG with hybrid retrieval + evaluation harness |
| 3 | **CanonPulse** | Self-directed | Databricks, LangGraph, Graph DB | Agentic reasoning with 269-test offline-first validation |
| 4 | **DepthWizard 2.0** | Self-directed | PyTorch, Depth Anything V3, Conformal Prediction | CV + uncertainty quantification — research-grade engineering |
| 5 | **AI YouTube Shorts Generator** | Open Source (PR #57) | Whisper, FFmpeg, Python | 4.2k⭐ repo; fixed transcription 0→59 segments |

---

## 1️⃣ AgencyOS — Self-Healing Agentic AI Platform

**🔗 Repo:** `github.com/LathissKhumar/AgencyOS-`  
**🎯 Problem:** Building reliable multi-agent systems is hard — agents fail silently, schemas drift, and there's no deterministic way to verify health.

**🛠️ My Approach:**
- Architected **5 LangGraph-orchestrated microservices** (Planner, Executor, Validator, Repairer, Monitor)
- Implemented **Agent-to-Agent (A2A) protocol** for inter-agent communication
- Built **self-healing web-intelligence layer** with:
  - Deterministic health scoring (not LLM-as-judge)
  - Automated schema-drift detection & repair
  - Event-driven recovery loops
- Full **FastAPI + PostgreSQL** backend with Docker Compose deployment

**📈 Results:**
- End-to-end autonomous workflow execution
- Self-recovery from schema changes without human intervention
- Modular architecture — each service independently deployable

**🔮 What I'd Do Next:**
- Add distributed tracing (OpenTelemetry) across A2A calls
- Implement agent-to-agent evaluation benchmarks
- Explore Kubernetes deployment with service mesh

**💡 Recruiter Signal:** This isn't a toy — it's a **production-shaped architecture** with real engineering trade-offs (consistency vs availability, sync vs async, deterministic vs probabilistic verification).

---

## 2️⃣ RAG-Based Intelligent Document QA — Production RAG Pipeline

**🔗 Repo:** `github.com/LathissKhumar/RAG_PIPELINE`  
**🎯 Problem:** Naive RAG fails on real documents — poor chunking, no evaluation, hallucinations.

**🛠️ My Approach:**
- **Semantic chunking** with overlap-aware splitting (not fixed-size)
- **Async document ingestion** pipeline with progress tracking
- **Scalable embedding generation** with batching + caching
- **Hybrid retrieval**: BM25 (lexical) + Dense Vector (semantic) + **MiniLM cross-encoder reranking**
- Built **evaluation harness** — not just "looks good" but measured metrics

**📈 Results:**
- Grounded, context-aware answers with citation tracking
- Retrieval quality measured, not guessed
- Modular — swap retrievers, rerankers, LLMs independently

**🔮 What I'd Do Next:**
- Add query rewriting / decomposition for complex questions
- Implement RAGAS / TruLens evaluation dashboard
- Optimize embedding latency with ONNX / TensorRT

**💡 Recruiter Signal:** I understand **RAG as an engineering system**, not a prompt template — chunking strategy, retrieval fusion, reranking, evaluation, observability.

---

## 3️⃣ CanonPulse — Agentic Narrative Intelligence on Databricks

**🔗 Repo:** `github.com/LathissKhumar/CanonPulse`  
**🎯 Problem:** LLMs hallucinate on long-form narrative reasoning. Need evidence-first, verifiable answers.

**🛠️ My Approach:**
- **Dual-layer temporal graph**: Entity layer (characters, locations, events) + Narrative layer (plot arcs, causality)
- **Evidence-first pipeline**: LLM extracts candidates → **Deterministic ledger resolves** conflicts, verifies consistency
- **269-test offline-first validation suite** — every claim traceable to source text
- Built on **Databricks** for scalable graph processing

**📈 Results:**
- Zero-hallucination narrative queries (by design — unverified claims rejected)
- Temporal reasoning: "What did Character X know at Chapter Y?"
- Scales to full novel corpora

**🔮 What I'd Do Next:**
- Add incremental graph updates for streaming narratives
- Explore neuro-symbolic integration for softer reasoning
- Multi-modal: integrate screenplay / audio transcripts

**💡 Recruiter Signal:** **Verification-first AI engineering** — I build systems where correctness is enforceable, not hoped for. The 269-test suite proves it.

---

## 4️⃣ DepthWizard 2.0 — Single-View 3D Reconstruction with Uncertainty

**🔗 Repo:** `github.com/LathissKhumar/DepthWizard-2.0`  
**🎯 Problem:** Monocular depth estimation is confident but wrong. Need calibrated uncertainty for downstream use.

**🛠️ My Approach:**
- **Depth Anything V3** backbone for strong priors
- **Physical solar-shadow verification** — uses physics (sun position, shadows) as ground truth signal
- **Split conformal prediction** for calibrated uncertainty intervals
- **GPU clipmap rendering** for real-time terrain visualization

**📈 Results:**
- Uncertainty estimates that actually correlate with error (not just variance)
- Physical verification catches systematic failures (e.g., textureless surfaces)
- Real-time rendering at 60+ FPS

**🔮 What I'd Do Next:**
- Extend to video with temporal consistency
- Add semantic segmentation for object-aware depth
- Deploy on edge (Jetson / mobile) with quantization

**💡 Recruiter Signal:** **Research-grade engineering** — combines SOTA deep learning, classical CV (physics), statistical rigor (conformal prediction), and systems optimization (GPU rendering).

---

## 5️⃣ AI YouTube Shorts Generator — Open Source Contribution (4.2k ⭐)

**🔗 Repo:** `github.com/SamurAIGPT/AI-Youtube-Shorts-Generator`  
**🎯 My Contribution:** **PR #57** — Fixed transcription pipeline: **0 → 59 segments** output

**🛠️ What I Did:**
- Diagnosed Whisper + FFmpeg integration failure
- Fixed audio segmentation logic causing empty outputs
- Added robustness for variable-length inputs
- Improved error handling & logging

**📈 Impact:**
- Merged into 4.2k star / 750+ fork project
- Enabled core feature for thousands of users
- Demonstrates: **debugging complex AV pipelines**, **open-source collaboration**, **shipping fixes to production**

**💡 Recruiter Signal:** I contribute to **real-world, high-visibility projects** — not toy repos. I read unfamiliar codebases, diagnose root causes, and ship fixes that stick.

---

## 💼 Professional Experience

### AI/ML Intern — Indium Software (Nov 2025 – Jan 2026)
**Project:** Liftr — AI-powered legacy code modernization platform

| Responsibility | Outcome |
|----------------|---------|
| Built RAG pipeline for codebase ingestion | Processed source code, README, TOML, YAML, configs at scale |
| Shipped production PRs in live client codebase | Code reviewed by senior engineers; passed CI/CD |
| Authored technical design documents | Architecture decisions communicated to cross-functional stakeholders |
| Validated AI-generated output critically | Applied judgement — didn't blindly merge LLM suggestions |

**💡 Recruiter Signal:** I've **worked in a professional engineering environment** — code review, design docs, CI/CD, client-facing delivery. Not just academic projects.

---

## 🧪 How I Think (Engineering Philosophy)

| Principle | In Practice |
|-----------|-------------|
| **Verification > Vibes** | 269-test suites, conformal prediction, deterministic ledgers |
| **Systems > Scripts** | Microservices, A2A protocol, event-driven, Docker, CI/CD |
| **Production-shaped from day 1** | Evaluation harnesses, observability, error handling, deployment |
| **Critical judgement on AI output** | Design docs, code review, human-in-the-loop validation |
| **Fast prototyping, rigorous delivery** | Idea → working demo in days → hardened in weeks |

---

## 🎓 Education & Credentials

- **B.E. Computer Science & Engineering** — Chennai Institute of Technology (2024–2028), CGPA: 8.29/10.0
- **650+ LeetCode** — DSA rigor, contest participation
- **NextGenHacks Winner** — Best Idea Track
- **Continuous learner** — Papers with Code, ArXiv daily, reproducing SOTA

---

## 📋 Quick Reference for Interviewers

### Ask Me About:
- **RAG evaluation** — how to measure retrieval quality beyond "looks good"
- **Agent reliability** — self-healing, schema drift, deterministic vs probabilistic verification
- **Uncertainty quantification** — conformal prediction, calibration, when to trust the model
- **Multi-agent orchestration** — A2A, LangGraph, communication patterns, failure modes
- **Open source contribution** — PR #57, debugging AV pipelines, collaborating on 4k⭐ repo

### Technical Deep-Dives I Enjoy:
- Hybrid retrieval fusion strategies (BM25 + dense + rerank)
- Graph-based reasoning with evidence tracing
- Split conformal prediction for depth/uncertainty
- Event-driven agent architectures
- Testing strategies for non-deterministic AI systems

---

## 🤝 Next Steps

1. **Review the code** — all repos are public with READMEs, docs, tests
2. **Pick a project** — I can walk through architecture, trade-offs, what I'd change
3. **Technical conversation** — happy to whiteboard, pair program, or discuss papers
4. **Culture fit** — I value: small flat teams, ownership, learning culture, engineering rigor

---

## 📞 Contact

**Ready to chat?**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn_Message-0A66C2?logo=linkedin&logoColor=white&style=for-the-badge)](https://linkedin.com/in/lathisskhumar)  
[![Email](https://img.shields.io/badge/Email-D14836?logo=maildotru&logoColor=white&style=for-the-badge)](mailto:pklathisskhumar.cse2024@citchennai.net)

> **Availability:** Immediate for internships • 4–6 month duration preferred • Conversion to full-time expected

---

*Last updated: November 2026 • This tour is maintained alongside my active projects*