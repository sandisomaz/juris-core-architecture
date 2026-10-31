# JurisCore
### Supervised Agentic AI Graph & Deterministic Legal Compliance Engine

[![Python 3.11+](https://img.shields.io/badge/Python-3.11%2B-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688.svg)](https://fastapi.tiangolo.com/)
[![POPIA Compliant](https://img.shields.io/badge/Compliance-POPIA%20%7C%20Companies%20Act-purple.svg)](#statutory-compliance--playbook-rules)
[![Architecture](https://img.shields.io/badge/Architecture-Proprietary%20Engine-black.svg)](#data-privacy--verification-notice)

---

> ### 🔒 Data Privacy & Verification Notice
> **Proprietary Codebase:** The complete source codebase for this project is hosted in a private repository to maintain local system sovereignty, protect proprietary legal prompt engineering, and safeguard client legal analysis workflows.
> 
> **Live Verification:** This repository serves as the public system architecture map and technical documentation. I am highly comfortable performing a live, end-to-end system demonstration and code walk-through during an interview to verify all architectural implementations and logic flows.

---

## 🎥 System Walkthrough & Interactive Demo

<div align="center">
  <a href="media/juriscore_walkthrough.mp4">
    <img src="media/demo.gif" alt="JurisCore System Walkthrough Demo" width="100%" style="border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);" />
  </a>
  <p><em>Click the preview above or <a href="media/juriscore_walkthrough.mp4">click here to watch the full HD video walkthrough (MP4)</a>.</em></p>
</div>

---

## 🏛️ Executive Summary

**JurisCore** is a specialized legal technology application combining deterministic statutory rules engines with supervised agentic AI workflows. Engineered specifically for corporate commercial law and regulatory audit in the South African jurisdiction, it bridges the gap between deep statutory analysis and clean, readable legal user experiences.

It empowers legal teams to audit complex commercial agreements, redline non-compliant terms, detect statutory compliance gaps (such as POPIA data processing terms and Companies Act director indemnities), and explore contracts through an distraction-free editorial interface.

---

## 🧠 System Architecture & Workflow

JurisCore separates non-deterministic AI inference from deterministic statutory verification rules:

```mermaid
flowchart TD
    subgraph Intake["Document Ingestion"]
        Doc[Commercial Agreement / PDF / DOCX] --> Extractor[Structured Clause Parser]
    end

    subgraph DualAudit["Dual-Engine Legal Audit Pipeline"]
        Extractor --> DeterministicEngine[Deterministic Rules Engine]
        Extractor --> AgenticGraph[Supervised Agentic Graph]

        DeterministicEngine -->|Statutory Checklist| StatRules[POPIA, Companies Act, CPA Baselines]
        AgenticGraph -->|Contextual Reasoning| RiskAudit[Risk & Ambiguity Identification]
    end

    subgraph Output["Editorial Workspace & Delivery"]
        StatRules --> UnifiedReport[Unified Audit Report & Redline Proposal]
        RiskAudit --> UnifiedReport
        UnifiedReport --> ReaderView[Editorial Clause Reader & Side-by-Side Redline]
        UnifiedReport --> Export[Export Clean / Redlined DOCX]
    end
```

---

## ⚖️ Statutory Compliance & Playbook Rules

JurisCore comes pre-loaded with commercial playbook rules mapped directly to South African statutes and common law standards:

1. **POPIA Section 19 & 21 Compliance:** Audits Operator and Responsible Party obligations, mandatory breach notification windows, and cross-border data transfer limitations.
2. **Companies Act 71 of 2008:** Scans director indemnification clauses against Section 78 restrictions to detect prohibited liability waivers.
3. **Consumer Protection Act (CPA) Section 48 & 49:** Identifies unfair, unreasonable, or unjust contract terms and mandatory notice requirements for indemnity risks.
4. **Commercial Risk Redlining:** Automatically proposes surgical redline amendments with statutory citations and lawyer-ready commentary.

---

## ✨ Interface & Editorial Design

JurisCore departs from cluttered multi-chart dashboards in favor of an **editorial, typography-first legal workspace**:
- **Editorial Paper Light Mode:** Clean, serif and clean sans typography calibrated for prolonged document review.
- **Distraction-Free Clause Reader:** Side-by-side comparative viewing of original clauses alongside AI-assisted redlines and statutory risk scores.
- **Instant Filtering:** Filter clauses by risk severity (High, Medium, Low), statutory category, or review status.

---

## 🛠️ Technology Stack & Engine Specs

- **Backend:** Python 3.11+, FastAPI asynchronous REST endpoints.
- **Frontend:** Modern responsive web interface, customized light/dark typography-first layout.
- **LLM Orchestration:** Supervised agentic graph with structured Pydantic schema validation.
- **Document Processing:** Streamlined DOCX/PDF text extraction and reconstruction.

---

Architected and maintained by **Sandiso Mazibuko**.
