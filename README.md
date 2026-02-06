# Jeex: The Agentic Business Operating System

![Status](https://img.shields.io/badge/System%20Status-Active%20Dev-success?style=for-the-badge)
![Architecture](https://img.shields.io/badge/Architecture-Event%20Driven-blue?style=for-the-badge)
![AI](https://img.shields.io/badge/Core-Agentic%20Swarm-blueviolet?style=for-the-badge)

> **⚠️ Proprietary Notice:** This repository contains the high-level system architecture and public documentation for Jeex. The core source code (`jeex-core`, `jeex-neural-engine`) is proprietary and hosted in private repositories at Infinity LAB.

## ⚡ Executive Summary
Jeex is an autonomous revenue operations system designed to replace manual CRM workflows. Unlike traditional CRMs that wait for human input, Jeex utilizes a **multi-agent architecture** to actively pursue, nurture, and close leads.

---

## 🏗 System Architecture

The Jeex ecosystem is built on a distributed microservices architecture, prioritizing low-latency data processing and stateful agent interactions.

### 1. The Neural Core (The Brain)
* **Agent Orchestrator:** Python-based supervisor that manages agent lifecycles.
* **LLM Gateway:** Route optimization layer that switches between fine-tuned Llama 3 models (for speed) and GPT-4 (for complex reasoning).
* **Memory Vector Store:** Long-term context retention using Pinecone/Milvus, allowing agents to remember client details across months of inactivity.

### 2. The Omni-Channel Bridge
* **Ingestion:** Webhooks for LinkedIn, Email (IMAP/SMTP), and WhatsApp Business API.
* **Normalization:** Converts unstructured conversation data into structured JSON objects for the agents to process.

### 3. The Frontend (The Interface)
* **Stack:** Flutter (Mobile/Desktop) & Next.js (Web Dashboard).
* **State Management:** BLoC pattern for predictable state transitions in the UI.

---

## 🧠 Core Agent Capabilities

| Agent ID | Function | Logic Description |
| :--- | :--- | :--- |
| **`scout-v1`** | Lead Identification | Scrapes public directories; verifies emails; enriches profiles with company revenue data. |
| **`sdr-auto`** | Outreach | Generates hyper-personalized hooks based on prospect's recent activity; manages follow-up cadence. |
| **`closer-bot`** | Negotiation | Handles scheduling; answers FAQ; detects buying signals to alert human sales staff. |

---

## 🛠 Technology Stack

* **Languages:** Python (AI Backend), TypeScript (API Gateway), Dart (Client).
* **Infrastructure:** Docker, Kubernetes, AWS Lambda.
* **Data:** PostgreSQL (Relational Data), Redis (Hot Cache).

---

### 📬 Access & Licensing
Jeex is currently in **Closed Alpha**.
For investor access or technical inquiries, please contact:
**Jeet** (Founder @ Infinity LAB)
