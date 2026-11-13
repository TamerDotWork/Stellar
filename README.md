# Enterprise Banking Hybrid RAG Engine

A minimal, auditable, and air-gapped Retrieval-Augmented Generation (RAG) architecture designed for **Tier-1 banking, financial services, and regulated enterprise environments**. 

Built with zero external SaaS dependencies, it combines **Hybrid Search (Dense + Sparse BM25 with Reciprocal Rank Fusion)**, **pre-retrieval RBAC security filtering**, **Cross-Encoder reranking**, and **Pydantic-enforced verbatim source citations**.

---

## Architecture Overview

Standard naive vector RAG fails in banking due to exact regulatory clause lookups (e.g., `Basel III LCR-402`), strict access boundaries, and zero tolerance for hallucinated compliance figures. This pipeline enforces a 5-stage auditable workflow:

