# Adaptive RAG Engine

Based on the proposed idea at the [Blog](https://www.mohamedishak.me/blog/agentic-rag-knows-knowledge-base/), Adaptive RAG Engine has following components:
- Adaptive Ingestion Router
- Adaptive Query Router

## Key Responsibilities for Enterprise-Ready:
- This is a modular engine inter-operable with Governance Engine (plug-and-play)
- This should fundamentally boast Multi-tenancy support
- This should existing enterprise ecosystem connectors to populate knowledge base (Google Drive, Sharepoint, Zendesk, Salesforce, SAP)
- This should focus on logical data separation layers (knowledge base, folders, association of kb with connector level or only a part of a connector(example: HR KB -> Google Drive Directory - /legal/hr_docs, HR KB -> Zendesk - Category: HR))

## Add-on Responsibilities for Enterprise-Ready:
- RBAC based document retrieval based on (user_id, team_id)
- Audit-based RAG (who did? on what? what changed?)
- Tracing based on Correlation ID(aka Request ID)
- Evaluation Gating
- Monitoring

## 1. Adaptive Ingestion Router

Uses
- [LightRAG](https://github.com/hkuds/lightrag) for Naive, Graph Routes
- [RAG-Anything](https://github.com/HKUDS/RAG-Anything) for Visual Document Route


## 2. Adaptive Query Router

Uses
- [LightRAG](https://github.com/hkuds/lightrag) for Naive, Graph Routes
- [RAG-Anything](https://github.com/HKUDS/RAG-Anything) for Visual Document Routes