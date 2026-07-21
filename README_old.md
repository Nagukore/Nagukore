<div align="center">
  <img src="assets/premium-hero.svg" alt="Nagesh Kore — AI Engineer & Full Stack Developer" style="width:100%;max-width:1200px;border-radius:12px;box-shadow:0 10px 30px rgba(0,0,0,0.6)" />
</div>

<div align="center" style="margin-top:14px">
  <h1 style="margin:6px 0;font-family:Inter, Roboto, -apple-system, sans-serif">Nagesh Kore</h1>
  <p style="margin:6px 0;color:#9fb6c9;max-width:860px">AI Engineer · Full‑Stack Systems Builder — I design and operate production AI platforms: RAG, local LLM orchestration, memory systems, and realtime infrastructure.</p>
  <p style="margin:8px 0">
    <a href="https://github.com/Nagukore">GitHub</a> •
    <a href="https://nageshs.vercel.app/">Portfolio</a> •
    <a href="https://www.linkedin.com/in/nagesh-kore-7566b6254">LinkedIn</a>
  </p>
</div>

---

<style>
/* Readability & spacing tuned for GitHub (dark mode friendly) */
:root{--muted:#9fb6c9;--accent:#9ed6ff;--bg:#060b10}
body{background:var(--bg)}
.card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:12px;padding:14px;margin:12px 0;border:1px solid rgba(255,255,255,0.03)}
.card h3{margin:0 0 8px 0}
.small{color:var(--muted);font-size:13px}
.kv{display:flex;gap:8px;flex-wrap:wrap}
.kv > span{background:rgba(158,214,255,0.04);padding:6px 10px;border-radius:999px;color:var(--accent);font-weight:600}
summary{outline:none}
summary::-webkit-details-marker{display:none}
.details-summary{display:flex;justify-content:space-between;align-items:center;padding:8px 0}
@media (max-width:720px){.card{padding:12px;margin:10px 0}}
</style>

## Quick facts

<div class="card">
  <div class="kv">
    <span>AI Workflow Architect</span>
    <span>RAG & Semantic Search</span>
    <span>Local LLMs & Orchestration</span>
    <span>Production Deployments</span>
  </div>
  <p class="small" style="margin-top:10px">Bangalore 🇮🇳 • nagesh.amcec@gmail.com • Open to senior roles and system‑level consulting</p>
</div>

---

## Focus (short)

<details class="card">
  <summary class="details-summary"><strong>Current focus</strong><span class="small">click to expand</span></summary>
  <div style="padding-top:8px">
    <ul>
      <li>Local LLM infrastructure & inference orchestration</li>
      <li>Retrieval‑first systems (RAG) with metadata filters and re‑ranking</li>
      <li>Agentic flows with auditable actions & safe confirmations</li>
      <li>Memory architectures (session → work → long‑term) optimized for cost & relevance</li>
      <li>Realtime pipelines, observability and production runbooks</li>
    </ul>
  </div>
</details>

---

## Engineering principles (one line each)

<div class="card">
  <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:10px">
    <div><strong>Production‑first</strong><div class="small">ship observability, not a black box</div></div>
    <div><strong>API‑first</strong><div class="small">clean contracts for each service</div></div>
    <div><strong>Idempotent actions</strong><div class="small">compensating transactions & safe defaults</div></div>
    <div><strong>Measure impact</strong><div class="small">latency SLOs, MTTR, automation coverage</div></div>
  </div>
</div>

---

## Architecture & Diagrams

<div class="card">
  <h3>AI Workflow (overview)</h3>
  <div style="display:flex;gap:12px;align-items:flex-start;flex-wrap:wrap">
    <img src="assets/architecture.svg" alt="AI Architecture" style="width:100%;max-width:760px;border-radius:8px" />
    <div style="flex:1;min-width:260px">
      <p class="small">Ingress → Intent Router → Retrieval (ANN + re‑rank) → Orchestration → Actions & Sync. Each stage emits traces and events for debugging.</p>
      <details style="margin-top:8px"><summary class="small">Why this matters</summary>
        <p class="small">Separation reduces blast radius: failures localize to retrieval, inference, or orchestration. Observability enables replay and faster post‑mortems.</p>
      </details>
    </div>
  </div>
</div>

---

## Agentic AI — safe actions (card)

<details class="card">
  <summary class="details-summary"><strong>Agent design</strong><span class="small">dry‑run • audit • confirm</span></summary>
  <div style="padding-top:8px">
    <p class="small">Actions are callable, idempotent functions with a dry‑run mode. All agent decisions log inputs, rationale and outcome; high‑impact actions require an approval token before execution.</p>

    <pre style="background:#021018;color:#9ed6ff;padding:12px;border-radius:8px;overflow:auto"><code># dry run example
$ agent run --task "sync meeting tasks" --dry
[DRY] extracted=12 tasks (3 duplicates)  
# approve:
$ agent approve --id=agent/2026-07-21/xyz
</code></pre>
  </div>
</details>

---

## RAG Pipeline (concise)

<details class="card">
  <summary class="details-summary"><strong>Retrieval architecture</strong><span class="small">chunk → embed → store → recall → re‑rank</span></summary>
  <div style="padding-top:8px">
    <ul>
      <li><strong>Chunking:</strong> semantic size tuned per domain (technical docs vs transcripts)</li>
      <li><strong>Metadata filters:</strong> filters run before ranking to reduce false positives</li>
      <li><strong>Two‑stage recall:</strong> ANN for speed, cross‑encoder for precision</li>
    </ul>
    <p class="small">Result: fewer hallucinations, higher precision and stable latency profiles in production.</p>
  </div>
</details>

---

## Local LLMs & Inference

<details class="card">
  <summary class="details-summary"><strong>Inference orchestration</strong><span class="small">routing • batching • fallbacks</span></summary>
  <div style="padding-top:8px">
    <p class="small">Route low‑latency queries to local models, heavy reasoning to cloud LLMs. Use batching for throughput and circuit breakers to avoid overload. Cache safe responses and degrade gracefully.</p>
    <pre style="background:#021018;color:#9ed6ff;padding:12px;border-radius:8px;overflow:auto"><code>$ orchestrator --pool local,remote --model-priority local:vicuna-13b,remote:gptx
[DISPATCH] req=abc -> local:vicuna-13b
[OK] req=abc completed 152ms
</code></pre>
  </div>
</details>

---

## Memory Architecture

<details class="card">
  <summary class="details-summary"><strong>Tiered memory</strong><span class="small">session → work → profile</span></summary>
  <div style="padding-top:8px">
    <p class="small">Store structured memories with entities and relations. Use TTL and relevance decay to keep prompts small and costs predictable.</p>
    <pre style="background:#021018;color:#9ed6ff;padding:12px;border-radius:8px;overflow:auto"><code>memory.write({type:'meeting_action',entities:[task,assignee],ts:now()})
query -> memory.search({entities:[task],window:'30d'})
</code></pre>
  </div>
</details>

---

## Semantic Search & Vector DB

<details class="card">
  <summary class="details-summary"><strong>Operational checklist (Qdrant)</strong><span class="small">snapshots • health • partitions</span></summary>
  <div style="padding-top:8px">
    <ol>
      <li>Nightly snapshots to S3</li>
      <li>Partition by tenant to avoid leakage</li>
      <li>Monitor recall stability & embedding drift</li>
    </ol>
    <p class="small">With autoscaling and snapshots we keep p99 query latency under 60ms at peak for our production workloads.</p>
  </div>
</details>

---

## System Design & Deployments

<details class="card">
  <summary class="details-summary"><strong>Design trade‑offs</strong><span class="small">observability • idempotency • SLOs</span></summary>
  <div style="padding-top:8px">
    <p class="small">Favor small services with clear contracts. Observe every state change. Prefer eventual consistency on notification paths to achieve sub‑200ms UX while keeping DB of record strongly consistent.</p>

    <p class="small"><strong>Deploy pattern:</strong> API‑first CI, canary rollouts, feature flags, runbooks and automated rollback hooks.</p>
  </div>
</details>

---

## Selected projects (impact cards)

<div class="card">
  <details>
    <summary><strong>FOSYS</strong> — AI workflow automation (IC‑AISMART Best Paper)</summary>
    <p class="small">Impact: reduced manual triage time by 60% in pilots. Architecture: transcription → task extraction → dependency graphs → RBAC orchestration.</p>
    <p class="small">Repo: https://github.com/Nagukore/fosys</p>
  </details>

  <details>
    <summary><strong>Enterprise RAG</strong> — production retrieval</summary>
    <p class="small">Impact: reduced avg time‑to‑answer from 7m → 90s in support flows. Uses metadata filters + re‑ranking for precision.</p>
    <p class="small">Repo: https://github.com/Nagukore/enterprise-rag-system</p>
  </details>

  <details>
    <summary><strong>VoxFlow</strong> — voice assistant</summary>
    <p class="small">Impact: improved task completion with streaming & intent routing. Repo: https://github.com/Nagukore/voxflow-ai</p>
  </details>

  <details>
    <summary><strong>SS Clinic</strong> — healthcare production delivery</summary>
    <p class="small">Impact: first real client deployment; PWA + AI chatbot. Live: https://www.ssclinickudlu.com</p>
  </details>
</div>

---

## Contact

<div class="card">
  <p class="small">Interested in senior engineering roles, system design reviews, or RAG/LLM architecture consulting. Email: nagesh.amcec@gmail.com • Portfolio: https://nageshs.vercel.app/</p>
</div>

---

<div align="center" style="margin-top:6px">
  <small style="color:#7f8c8d">Optimized for dark mode and mobile. This README is curated to present architecture, impact, and operational rigor — a living document maintained by Nagesh Kore © 2026</small>
</div>
