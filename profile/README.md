<div align="center">
  <!-- Dynamic Waving Header Banner -->
  <img width="2172" height="724" alt="AI Engineering Lab Banner" src="https://github.com/user-attachments/assets/4c98edf8-e5f8-4129-9282-cc319d54f677" />

  <p align="center">
    A collection of AI Engineering projects in pursuit of continuous learning.
  </p>
</div>

---

## NALIWANAGAN — Agentic AI Engineering Portfolio

Welcome to *Naliwanagan*, an open-source engineering lab dedicated to building production-grade autonomous AI systems. Every repository in this organization is part of my structured, hands-on journey to master Agentic AI Engineering—moving beyond fragile prompt wrappers to build deterministic, observable, and fault-tolerant software around non-deterministic models.

All codebases here are open-source (MIT License), containerized, and built for reproducibility.

### Engineering Philosophy

Raw model intelligence is only ~20% of a production agent; the remaining 80% is rigorous software engineering. Across these repositories, every system is designed around four core principles:
- **Deterministic Guardrails**: Safety boundaries, schema validation, and destructive-command filtering live in traditional code (e.g., Pydantic v2 schemas and SQLGlot AST parsing), never in LLM prompt instructions alone.
- **Protocol-First Tooling**: External integrations are decoupled from model logic using standardized interfaces like the Model Context Protocol (MCP).
- **State Persistence & Human-in-the-Loop (HITL)**: Long-running workflows use durable checkpointing and explicit approval gates before executing mutating operations.
- **Eval-Driven Reliability**: Systems are backed by automated CI test suites, trajectory evaluations, and cost/iteration circuit breakers.

---

### 🚀 Project
- **[Data Extractor](https://github.com/NALIWANAGAN/AI-ENG-P1) 📕**: A self-correcting data extraction service that converts PDF invoices into validated PostgreSQL entries, using an LLM that acts through a sandboxed MCP server. Every generated query passes a deterministic sqlglot guardrail and a least-privilege database role, and failed queries are returned to the model with the database error so it can fix them.

---

### Note for Recruiters & Engineering Leaders

If you are reviewing this organization as part of an engineering evaluation, here is what these repositories demonstrate about how I build:
- **Systems Engineering Over Prompt Tuning**: I treat LLMs as probabilistic reasoning components inside deterministic software boundaries—enforcing typed contracts, bounded retries, rate-limit handling, and async execution queues.
- **Security & Defense-in-Depth**: Tools are built with least-privilege permissions, containerized sandboxing, and AST-level query validation to protect against indirect prompt injection and unintended state mutations.
- **Production Readiness**: Projects ship with docker-compose.yml environments, automated pytest verification suites, and CI pipelines so you can clone, boot, and test every architecture locally in minutes.

---

### Connect

- **[Portfolio / Website](https:benjineer.vercel.app)**
- **[LinkedIn](https://linkedin.com/in/benji-cañones)**
- **Email**: benjicanones6@gmail.com
  
