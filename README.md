# 🧠 Knowledge Nexus
### Cross-Referential Intelligence System | AI-Powered Collaborative Knowledge Management

![AI](https://img.shields.io/badge/AI-Powered-00d9ff?style=for-the-badge)
![Prompt Engineering](https://img.shields.io/badge/Prompt%20Engineering-Advanced-8b5cf6?style=for-the-badge)
![Business Intelligence](https://img.shields.io/badge/Business%20Intelligence-AI%20Native-10b981?style=for-the-badge)
![React](https://img.shields.io/badge/React-18-61dafb?style=for-the-badge&logo=react)
![Status](https://img.shields.io/badge/Status-Production-success?style=for-the-badge)

---

> **Knowledge Nexus** is a full-stack collaborative intelligence platform that transforms unstructured documents, conversations, and ideas into synthesized, queryable knowledge — using a structured three-stage AI pipeline, multi-user project collaboration, and a 5W synthesis engine (Who, What, When, Where, Why).

---

## 🎯 Core Skills Demonstrated

| Domain | Skills Applied |
|---|---|
| **Prompt Engineering** | Structured prompt chaining, JSON schema enforcement, multi-stage LLM orchestration, chunked context management |
| **Business Intelligence** | KPI dashboards, pipeline health metrics, activity timelines, knowledge density scoring |
| **AI System Design** | Multi-stage data transformation pipelines, semantic compression, synthesis generation |
| **Data Architecture** | Entity-relationship modeling, real-time subscriptions, metadata enrichment |
| **Collaborative Systems** | Role-based access, shared workspaces, threaded comments, real-time sync |
| **Frontend Engineering** | React 18, Tailwind CSS, TanStack Query, Recharts, Framer Motion |

---

## 🔬 Prompt Engineering — Technical Depth

### Stage 1 — Primary Pipeline: Compression Prompt
- Accepts raw text from `.docx`, `.json`, `.txt`, and manual input
- Prompt enforces: *succinctness, precision, redundancy elimination, English-only output*
- Large documents are **chunked** and processed iteratively with a progress callback
- Final output is a semantically compressed representation stored as `compressed_content`

---

### Stage 2 — Secondary Pipeline: Concept Evolution
- Prompt drives a four-stage evolution: `idea → concept → paradigm shift → understanding`
- Extracts structured WHO / WHAT / WHY metadata per note
- Creates linked `Concept` entities tracking each evolution step
- Designed to surface **non-obvious meaning** from compressed inputs

---

### Stage 3 — Tertiary Pipeline: Synthesis Engine *(Flagship Feature)*
- Cross-references up to 15 related notes simultaneously in a single prompt
- Enforces **structured JSON schema output** with the following synthesis dimensions:
  - `who` — key actors and stakeholders
  - `what` — unified conceptual understanding
  - `when` — temporal patterns and sequences
  - `where` — contextual environments and domains
  - `why` — root causes, motivations, purposes
  - `synthesis` — emergent understanding from connected knowledge
  - `breakthrough_insights[]` — novel insights that only appear at scale
  - `connections[]` — explicit knowledge graph edges

---

### Insights Engine — Interactive Q&A
- Users submit natural language questions against the full knowledge base
- System injects compressed notes + synthesis metadata into context window
- LLM returns structured 5W answers + ranked breakthrough insights
- Designed around **retrieval-augmented generation (RAG)** principles without a vector database

---

## 🏗️ System Architecture

Raw Content │ ▼ ┌─────────────────────┐ │ Primary Pipeline │ ← Compression + Normalization │ (Text → Signal) │ └────────┬────────────┘ │ ▼ ┌─────────────────────┐ │ Secondary Pipeline │ ← Concept Evolution + Metadata Extraction │ (Signal → Meaning) │ └────────┬────────────┘ │ ▼ ┌─────────────────────┐ │ Tertiary Pipeline │ ← Cross-Referential Synthesis │ (Meaning → Insight) │ └────────┬────────────┘ │ ▼ Insights Engine (Query → 5W Answer)


---

## 📊 Business Intelligence Features

- 📈 **Knowledge Density Score** — % of notes that have passed through full synthesis pipeline
- 🔢 **Pipeline Stage Counters** — Live counts at each transformation stage
- 👥 **Team Engagement Metrics** — Per-member activity tracking inside projects
- 📅 **Activity Timelines** — Recharts-powered time series of knowledge creation
- 🧮 **Stage Distribution Charts** — Visual breakdown of pipeline health
- 🏆 **Project Health Score** — Composite metric across collaboration + pipeline progress
- 💡 **Breakthrough Insight Counter** — Tracks AI-generated novel connections

---

## 🤝 Collaboration Features

- **Multi-user Projects** with color-coded workspaces
- **Role-based access** (admin / user / contributor)
- **Shared notes** with live co-editing and `last_edited_by` tracking
- **Threaded comments** with resolve/unresolve workflow
- **Real-time subscriptions** — UI updates without polling
- **Invite by email** — onboard teammates directly from the app

---

## 🗄️ Data Model

| Entity | Purpose |
|---|---|
| `Note` | Core knowledge unit with compression, tags, pipeline stage, sharing metadata |
| `Project` | Collaborative workspace with member management |
| `Concept` | Tracks 4-stage evolution of a note through secondary pipeline |
| `Relationship` | Typed edges between notes (references, contradicts, supports, extends) |
| `Comment` | Threaded discussion attached to notes |
| `PipelineConfig` | Configurable pipeline steps per stage |

---

## 🧰 Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | React 18, Tailwind CSS, TypeScript |
| **State Management** | TanStack Query (React Query v5) |
| **Charts** | Recharts |
| **Animations** | Framer Motion |
| **File Parsing** | Mammoth.js (DOCX extraction) |
| **Backend / DB** | Base44 BaaS (real-time subscriptions, auth, entity storage) |
| **AI / LLM** | Base44 InvokeLLM (structured JSON schema prompting, chunked processing) |
| **Auth** | Built-in JWT-based role authentication |

---

## 🧠 Skills for Recruiters

### Prompt Engineering
> Structured multi-stage prompt chains • JSON schema-enforced outputs • Context window management • Chunked iterative processing • Few-shot instruction framing • RAG-style knowledge injection • Multi-document synthesis prompting

---

### Business Intelligence with AI
> KPI dashboard design • AI-generated metrics • Knowledge density scoring • Pipeline throughput tracking • Activity analytics • Recharts data visualization • Composite health scoring • Real-time BI updates

---

### System Thinking / Architecture
> Three-tier data transformation pipeline • Entity-relationship modeling • Real-time pub/sub design • Separation of concerns across pipeline stages • Scalable chunking strategies for large documents • Metadata enrichment at each pipeline stage

---

### Collaboration & Product Design
> Multi-tenancy patterns • Role-based access control • Threaded discussion systems • Real-time sync architecture • User onboarding flows • Workspace isolation

---

## 📁 Project Structure

├── pages/ │ ├── Dashboard.js # BI metrics and overview │ ├── Upload.js # File ingestion + primary pipeline │ ├── KnowledgeBase.js # Search, filter, note management │ ├── Insights.js # 5W Q&A + synthesis viewer │ ├── Projects.js # Collaborative workspaces │ ├── Pipelines.js # Pipeline management + triggers │ └── Profile.js # User settings + membership ├── components/ │ ├── upload/ # FileDropzone, ManualNoteForm │ ├── knowledge/ # NoteCard │ ├── collaboration/ # NoteEditor, CommentSection, ProjectCard, ProjectDashboard │ ├── pipelines/ # PipelineStageCard │ └── utils/ # contentProcessor (chunking, summarization) └── entities/ ├── Note.json ├── Project.json ├── Concept.json ├── Relationship.json ├── Comment.json └── PipelineConfig.json

https://nexus-mind-e24f2206.base44.app

---

*Built with React 18 · Base44 · LLM Orchestration · Real-time Collaboration*
