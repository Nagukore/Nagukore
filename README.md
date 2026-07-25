<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=220&text=Nagesh%20Kore&fontAlign=50&fontAlignY=40&color=0:0F2027,50:203A43,100:2C5364&fontColor=ffffff&fontSize=52&desc=Full-Stack%20Engineer%20%7C%20AI%20Systems%20Builder&descAlignY=60&animation=fadeIn" width="100%"/>

### Full-Stack Engineer • AI Systems Builder • Production-Focused Developer

Building AI-integrated platforms, realtime systems, automation pipelines, and production-ready applications.

![Production Systems](https://img.shields.io/badge/Production_Systems-1D9E75?style=for-the-badge)
![AI Engineer](https://img.shields.io/badge/AI_Integrated_Development-0A66C2?style=for-the-badge)
![Realtime Systems](https://img.shields.io/badge/Realtime_Infrastructure-7F77DD?style=for-the-badge)

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nagesh-kore-7566b6254)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Nagukore)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=vercel&logoColor=white)](https://nageshs.netlify.app/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/the.nagesh)

**[About](#about-me) · [What I Solve](#what-i-solve) · [Featured Systems](#featured-engineering-systems) · [Projects](#core-engineering-projects) · [Stack](#technical-expertise) · [Deployments](#production-deployments) · [Connect](#connect)**

</div>

---

## About Me

```yaml
name:        Nagesh Kore
location:    Bangalore, India
role:        Full-Stack Engineer & AI Systems Builder
education:   B.E. in AI & ML — AMC Engineering College (2026)
experience:  Developer Intern @ ThoughtsCrest (Core Banking Domain)

focus:
  - AI-integrated full-stack systems
  - Realtime infrastructure & orchestration
  - Retrieval-Augmented Generation systems
  - Automation pipelines & developer tooling
  - Production deployment & scalable architecture

currently_exploring:
  - Local LLM deployment pipelines
  - Multi-agent orchestration
  - Agent memory architectures
  - Realtime streaming AI infrastructure

engineering_principles:
  - Build for production, not just demos
  - API-first architecture
  - Systems should scale cleanly
  - If it's not deployed, it's not done
```

---

## What I Solve

I build systems where the AI layer has to survive contact with real users and real data — not demos.

**Problem space I keep returning to:**
- **Fragmented workflows** → orchestration systems that route intent (KNOWLEDGE / ACTION / GENERAL) instead of hardcoding every path
- **Stale or unstructured knowledge** → retrieval pipelines (RAG) that make enterprise/document data queryable in plain language
- **Manual, repetitive coordination** → automation that extracts structure from unstructured input (meetings → tasks → dependency graphs)
- **Production gaps between prototype and deployment** → I ship end-to-end: auth, RBAC, realtime sync, hosting — not just the model call

**How I approach it:**
1. Start from the operational bottleneck, not the tech
2. Design API-first so the frontend/backend can evolve independently
3. Treat realtime + auth + RBAC as first-class, not afterthoughts
4. Deploy early — debugging in production teaches things staging can't

---

## Portfolio

> Single-page portfolio with a built-in AI chatbot (NagiBot), glassmorphism animations, dynamic project modals, and a dark-mode aesthetic — React + TypeScript + Vite.

**Live:** [nageshs.netlify.app](https://nageshs.netlify.app/) · **Repo:** [Nagesh-portfolio](https://github.com/Nagukore/Nagesh-portfolio)

`React 18` `TypeScript` `Vite` `Custom CSS Animations` `Glassmorphism`

---

## Featured Engineering Systems

<details>
<summary><h3>⭐ FOSYS — AI Workflow Automation & SCRUM Intelligence Platform 🏆 Best Paper Winner, IC-AISMART 2025</h3></summary>

Production-oriented AI orchestration platform automating SCRUM workflows, meeting intelligence, and task coordination across teams.

**Core Capabilities**
- AI-powered meeting transcription and task extraction
- Dependency graph generation for task orchestration
- Role-Based Access Control (RBAC)
- Realtime synchronization via Supabase Realtime
- Intelligent PR workflow automation
- API-first modular backend architecture

**Architecture**
```text
Meeting Input → Speech Processing → AI Task Extraction Engine
→ Dependency Graph Builder → Realtime Sync Layer → RBAC Dashboard
```

**Stack:** `React` `FastAPI` `Supabase` `Prisma` `PostgreSQL` `Realtime APIs`

</details>

<details>
<summary><h3>⭐ SS Clinic — AI-Integrated Healthcare Website (First Production Client Delivery)</h3></summary>

My first end-to-end full-stack production deployment — delivered to a real healthcare client. Patient-facing platform for SS Clinic, Kudlu.

**Features**
- AI chatbot integration for patient navigation
- Doctor availability & appointment booking workflows
- Progressive Web App with offline mode
- API-driven appointment scheduling

**Why it matters:** this project set the bar for what "production" means to me — real auth, real routing, real users, debugging in prod instead of dev. Every system since has built on it.

**Stack:** `React` `Firebase` `PWA` `AI Chatbot`

**Live:** [ssclinickudlu.com](https://www.ssclinickudlu.com)

</details>

---

## Core Engineering Projects

<details>
<summary><h3>i. VoxFlow — Voice-First AI Assistant</h3></summary>

Multi-stage AI assistant with intelligent intent routing and long-term memory architecture.

**Key Features**
- KNOWLEDGE / ACTION / GENERAL intent routing
- Long-term memory using Qdrant vector database
- SSE-based realtime reminder system
- AI-powered email intelligence
- Voice interaction via Vapi

**Pipeline**
```text
Voice Input → Intent Classifier → Router → Memory Retrieval
→ LLM Orchestration → Realtime Response Streaming
```

**Stack:** `Node.js` `FastAPI` `Qdrant` `Gemini` `SSE` `Vapi`
**Repo:** [voxflow-ai](https://github.com/Nagukore/voxflow-ai)

</details>

<details>
<summary><h3>ii. Enterprise RAG System — Retrieval-Augmented Knowledge Platform</h3></summary>

Production-oriented semantic retrieval system for structured and unstructured enterprise knowledge bases.

**Retrieval Architecture**
```text
Document Upload → Chunking Pipeline → Embedding Generation
→ Qdrant Vector Storage → Semantic Retrieval → LLM Context Injection → AI Response
```

**Stack:** `Python` `FastAPI` `Qdrant` `Gemini Embeddings` `NLP`
**Repo:** [enterprise-rag-system](https://github.com/Nagukore/enterprise-rag-system)

</details>

<details>
<summary><h3>iii. Clinichealthtree — Production Healthcare Infrastructure</h3></summary>

End-to-end clinic management platform: appointment scheduling, JWT auth, role-based dashboards (admin/doctor/patient), realtime updates via Firebase.

**Stack:** `React` `Firebase` `PostgreSQL` `JWT Authentication`
**Live:** [cliniquehealthtree.com](https://www.cliniquehealthtree.com)

</details>

<details>
<summary><h3>iv. Siddeshwara Global Services — Business Platform + E-Commerce</h3></summary>

Multi-page production platform for a Bangalore-based cleaning products supplier, with a full e-commerce storefront: catalog, browsing, ordering, and Google Maps location integration.

**Stack:** `React` `TypeScript` `TailwindCSS` `Firebase` `React Router` `Google Maps API`
**Live:** [siddeshwaraglobalservices.com](https://www.siddeshwaraglobalservices.com)

</details>

<details>
<summary><h3>v. Virtual AI Mouse — Gesture-Controlled Contactless Mouse (Published Research)</h3></summary>

Real-time gesture-controlled virtual mouse using computer vision and hand tracking — no hardware beyond a webcam.

> 📄 **Published:** *Hands-Free Computing: A Gesture-Controlled Virtual AI Mouse* — JETIR, Vol. 12, Issue 5, May 2025 (Paper ID: JETIR2505760)

**Stack:** `Python` `OpenCV` `MediaPipe` `PyAutoGUI`
**Repo:** [VIRTUAL-AI-MOUSE](https://github.com/Nagukore/VIRTUAL-AI-MOUSE)

</details>

<details>
<summary><h3>vi. Advanced Book Scraper CLI — Multithreaded Web Scraping Tool</h3></summary>

High-performance concurrent CLI scraper with retry strategies, filtering, and analytics export.

**Features:** concurrent processing via `ThreadPoolExecutor`, exponential backoff, CSV analytics export

**Stack:** `Python` `BeautifulSoup4` `requests` `ThreadPoolExecutor`
**Repo:** [advanced-book-scraper](https://github.com/Nagukore/advanced-book-scraper)

</details>

<details>
<summary><h3>vii. Hunt the Wumpus — Browser Game (Built in Under 4 Minutes, One Prompt)</h3></summary>

A rapid AI-prototyping experiment: a complete cave exploration game generated from a single, precisely-scoped prompt — no iteration loop, deployed the same session. A small proof of concept that clear problem framing multiplies AI leverage.

**Stack:** `Vanilla JavaScript` `HTML5` `CSS3`
**Live:** [wumpusgames.netlify.app](https://wumpusgames.netlify.app/)

</details>

---

## Technical Expertise

<div align="center">
<img src="https://skillicons.dev/icons?i=react,ts,js,python,fastapi,nodejs,postgres,mongodb,firebase,supabase,docker,linux,git,github,vscode,tailwind" />
</div>

<details>
<summary><h3>Frontend Engineering</h3></summary>

React ecosystem & multi-page architecture · TypeScript · Responsive UI & TailwindCSS · Progressive Web Apps (offline mode) · State management · E-commerce UI/workflow design

</details>

<details>
<summary><h3>Backend & APIs</h3></summary>

FastAPI microservices · Node.js backend systems · REST API design & JWT auth · Role-Based Access Control (RBAC) · Realtime infrastructure · Event-driven workflows

</details>

<details>
<summary><h3>Databases & Cloud</h3></summary>

PostgreSQL schema design · Supabase Realtime · MongoDB · Vector databases (Qdrant) · Firebase hosting & integration

</details>

<details>
<summary><h3>AI / ML Engineering</h3></summary>

Retrieval-Augmented Generation (RAG) · AI orchestration & intent routing · Semantic search & vector embeddings · NLP workflows · Computer vision (MediaPipe, OpenCV) · Multi-agent orchestration (exploring)

</details>

<details>
<summary><h3>DevOps & Tooling</h3></summary>

Git & GitHub workflows · Linux environments · Vercel & Firebase deployment pipelines · API testing & automation

</details>

---

## Production Deployments

| Platform | Type | Live Link | Status |
|---|---|---|---|
| Personal Portfolio | Developer Portfolio + NagiBot | [nageshs.netlify.app](https://nageshs.netlify.app/) | ✅ Production |
| SS Clinic | AI Healthcare Website (Client) | [ssclinickudlu.com](https://www.ssclinickudlu.com) | ✅ Production |
| Clinichealthtree | Full-Stack Healthcare Platform | [cliniquehealthtree.com](https://www.cliniquehealthtree.com) | ✅ Production |
| Siddeshwara Global Services | Business Platform + E-Commerce | [siddeshwaraglobalservices.com](https://www.siddeshwaraglobalservices.com) | ✅ Production |
| Hunt the Wumpus | Browser Game (built in 4 min, 1 prompt) | [wumpusgames.netlify.app](https://wumpusgames.netlify.app/) | ✅ Live |

---

## Engineering Philosophy

```text
▸ Design systems that solve real operational problems
▸ Build modular architectures that scale cleanly
▸ Use AI as a force multiplier, not a gimmick
▸ Prioritize deployment, usability, and reliability
▸ If it's not shipped, it doesn't count
```

---

## GitHub Analytics

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Nagukore&show_icons=true&theme=tokyonight&hide_border=true&border_radius=15" />
<img height="170" src="https://github-readme-streak-stats.herokuapp.com/?user=Nagukore&theme=tokyonight&hide_border=true&border_radius=15" />

<br/><br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Nagukore&theme=tokyo-night&hide_border=true&radius=16" width="95%" />

</div>

---

## Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nagesh-kore-7566b6254)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Nagukore)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=vercel&logoColor=white)](https://nageshs.netlify.app/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/the.nagesh)

📧 nagesh.amcec@gmail.com

**Open to:** open-source collaboration · AI engineering projects · freelance development · startup engineering opportunities

⭐ If something here helps or inspires you, consider starring the repositories.

<img src="https://capsule-render.vercel.app/api?type=waving&height=120&color=0:0F2027,50:203A43,100:2C5364&section=footer" width="100%"/>

</div>
