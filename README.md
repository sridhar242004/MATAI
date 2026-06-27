<div align="center">

# ∑ Mathematical Conjecture Proposer

### AI-Powered Mathematical Discovery, Engineered as a Single-File Application

*Harnessing large language models to generate novel, mathematically rigorous conjectures across eight domains of pure mathematics.*

[![Made with JavaScript](https://img.shields.io/badge/JavaScript-ES2020+-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](#)
[![Powered by Groq](https://img.shields.io/badge/Inference-Groq%20LPU-FF6B35?style=flat-square)](#)
[![Bootstrap 5](https://img.shields.io/badge/UI-Bootstrap%205-7952B3?style=flat-square&logo=bootstrap&logoColor=white)](#)
[![MathJax](https://img.shields.io/badge/Math-MathJax%203-2D7D9A?style=flat-square)](#)
[![GSAP](https://img.shields.io/badge/Motion-GSAP%203-88CE02?style=flat-square)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](#license)

[Live Demo](#) · [Architecture](#-architecture) · [API Contract](#-backend-api-contract) · [Engineering Notes](#-engineering-deep-dive)

</div>

---

## Overview

**Mathematical Conjecture Proposer** is a zero-build, single-file frontend that turns a large language model into a structured **conjecture engine**. Instead of treating the LLM as a free-text chatbot, the app constrains it with a parameter matrix — **8 mathematical domains × 7 statement types × 4 complexity tiers × continuous creativity control** — and a strict, header-driven output contract that the client parses deterministically into title, statement, motivation, related results, proof approaches, difficulty, and keywords.

The result is a tool that feels less like "ask AI a question" and more like a **research idea-generation instrument**: rigorous LaTeX rendering, persistent history with analytics, batch generation, and an educational reference layer covering real open problems (Riemann Hypothesis, Goldbach, Twin Primes, P vs NP, Poincaré, BSD).

> ⚠️ **Disclaimer:** Conjectures are AI-generated starting points for exploration, not verified mathematics. Every output is explicitly labeled and requires human/expert review before any claim of correctness.

---

## ✦ Feature Matrix

| Capability | Detail |
|---|---|
| **Multi-model inference** | Runtime-switchable between `llama-3.3-70b-versatile`, `llama-3.1-8b-instant`, `openai/gpt-oss-120b`, `openai/gpt-oss-20b`, `meta-llama/llama-4-scout-17b-16e-instruct`, `qwen/qwen3-32b` via Groq's LPU inference |
| **Parametric generation** | 8 domains (Number Theory, Topology, Abstract Algebra, Real Analysis, Combinatorics, Differential Geometry, Probability Theory, Set Theory) × 7 statement types (Existence, Inequality, Equivalence, Asymptotic, Classification, Structural, Open-ended) |
| **Tunable creativity** | Continuous temperature slider (0.1–1.5) and 4-tier complexity ladder (Undergraduate → Graduate → Research-level → Millennium-level) |
| **Custom prompt engineering** | User-editable system prompt with `{domain}` `{type}` `{complexity}` `{context}` template interpolation — power users can fully rewrite the generation strategy without touching code |
| **Batch generation** | Generates 2–5 conjectures per run with live progress bar, per-item success/failure handling, and a "Mixed" domain mode for variety |
| **Deterministic response parsing** | A single regex-driven parser (`parseResp`) decomposes free-form LLM markdown into seven structured fields — no JSON-mode dependency, resilient to model drift |
| **Rigorous math rendering** | MathJax 3 (TeX → CHTML) renders every statement as publication-quality notation, lazily re-typeset on tab switch / accordion open |
| **Persistent history** | LocalStorage-backed log with live search, per-domain filter chips, like/save, JSON export & re-import, native Web Share API with clipboard fallback |
| **Analytics dashboard** | Chart.js-powered domain distribution (doughnut), complexity breakdown (bar), and a real 7-day rolling activity histogram computed from history timestamps |
| **Educational layer** | Accordion of 6 historically significant conjectures with year, status, domain, LaTeX statement, and context; click-to-copy LaTeX cheat-sheet for 12 common symbols |
| **Generative ambient UI** | Canvas-based particle field of 55 animated mathematical glyphs (∑ ∫ ∂ ∈ ∞ π …) with proximity-based connective lines, plus an infinite marquee ticker of 12 famous theorems |
| **Motion system** | GSAP + ScrollTrigger for scroll-scrubbed hero parallax and staggered section reveals |
| **Security-conscious by design** | API key never touches the browser — every model call is proxied through a backend; all AI-generated HTML is run through an `esc()`/`san()` sanitization pass that strips `<script>` and inline event handlers before DOM injection |
| **Accessible & responsive** | `aria-hidden` on every decorative layer, `aria-label`/`role="button"` on interactive non-native elements, mobile-first breakpoints at 400 / 768 / 992 / 1400 / 1800px, and a dedicated print stylesheet |

---

## 🏗 Architecture

This repository ships the **presentation + orchestration layer** as a single self-contained file. There is intentionally **no bundler, no framework runtime, and no build step** — every dependency is a CDN `<script>`/`<link>` tag, and the entire client logic (~115 functions) lives in one inline `<script>` block.

```
┌─────────────────────────────────────────────────────────────┐
│                        index.html                            │
│  ┌───────────────┐  ┌───────────────┐  ┌──────────────────┐ │
│  │  Design Token  │  │   Markup       │  │   Application     │ │
│  │  CSS System    │  │   (6 tabs:     │  │   Logic (vanilla  │ │
│  │  (custom props)│  │   Generate /   │  │   JS, ~115 fns)    │ │
│  │                │  │   Batch /      │  │                    │ │
│  │  + @property   │  │   Analytics /  │  │  State (S) ──┐     │ │
│  │    --glow-angle│  │   History /    │  │              │     │ │
│  │  + responsive  │  │   Learn /      │  │  Settings ───┤     │ │
│  │    breakpoints │  │   Settings)    │  │              │     │ │
│  └───────────────┘  └───────────────┘  │  History ────┤     │ │
│                                          │  (LocalStorage)    │ │
│                                          └────────┬──────────┘ │
└───────────────────────────────────────────────────┼────────────┘
                                                     │ fetch()
                                                     ▼
                                  ┌──────────────────────────────┐
                                  │   Backend Proxy (not in this  │
                                  │   bundle — see API Contract)  │
                                  │   /api/health                 │
                                  │   /api/generate                │
                                  │   /api/batch                   │
                                  │   • holds GROQ_API_KEY server-  │
                                  │     side via env var            │
                                  └────────────┬───────────────────┘
                                               │
                                               ▼
                                      ┌─────────────────┐
                                      │   Groq LPU API    │
                                      │  (LLaMA 3.x / 4,   │
                                      │  GPT-OSS, Qwen3)   │
                                      └─────────────────┘
```

**Why a thin backend proxy, instead of calling Groq directly from the browser?** The Settings tab is explicit about this: *"The Groq API key is stored securely on the backend server via environment variables. It is never exposed to the browser."* This is a deliberate security boundary — client-side API keys in a static HTML file are trivially extractable from devtools/network tab, so all three endpoints (`/api/health`, `/api/generate`, `/api/batch`) are designed to be implemented by any backend of your choice (Node/Express, Cloudflare Workers, a serverless function, etc.).

---

## 🔌 Backend API Contract

The frontend is backend-agnostic — it only requires three endpoints with the shapes below. Implement these in **any** stack and the UI works unmodified.

### `GET /api/health`
Used by the **Test Backend** button in Settings.
```json
// 200 OK
{ "keyConfigured": true }
```

### `POST /api/generate`
Used by single-conjecture generation.
```jsonc
// Request
{
  "domain": "Number Theory",
  "type": "Existence",
  "complexity": "Graduate",
  "temperature": 0.7,
  "maxTokens": 1200,
  "context": "",
  "model": "llama-3.3-70b-versatile",
  "systemPrompt": "You are a world-class mathematician…"
}

// Response — `content` is parsed client-side by parseResp()
{ "content": "**CONJECTURE TITLE**: …\n**STATEMENT**: …\n**MOTIVATION**: …" }
```

### `POST /api/batch`
Used by the Batch Generation tab.
```jsonc
// Request
{ "domain": "Mixed", "count": 3, "complexity": "Graduate", "temperature": 0.7, "maxTokens": 1000, "context": "", "model": "...", "systemPrompt": "..." }

// Response
{
  "results": [
    { "ok": true, "domain": "Topology", "type": "Structural", "content": "**CONJECTURE TITLE**: …" },
    { "ok": false, "error": "rate limited" }
  ]
}
```

> **Reference implementation skeleton** (Node/Express, drop into any host):
> ```js
> app.post('/api/generate', async (req, res) => {
>   const { systemPrompt, domain, type, complexity, context, model, temperature, maxTokens } = req.body;
>   const r = await fetch('https://api.groq.com/openai/v1/chat/completions', {
>     method: 'POST',
>     headers: { 'Authorization': `Bearer ${process.env.GROQ_API_KEY}`, 'Content-Type': 'application/json' },
>     body: JSON.stringify({
>       model,
>       temperature,
>       max_tokens: maxTokens,
>       messages: [
>         { role: 'system', content: systemPrompt },
>         { role: 'user', content: `Generate a novel ${type.toLowerCase()} conjecture in ${domain}. Difficulty: ${complexity}-level. ${context}` }
>       ]
>     })
>   });
>   const data = await r.json();
>   res.json({ content: data.choices[0].message.content });
> });
> ```

---

## 🧠 Engineering Deep-Dive

A few decisions worth calling out for reviewers auditing this codebase:

- **Header-driven parsing over JSON mode** — `parseResp()` uses a single parameterized regex (`` `\\*\\*${k}\\*\\*:?\\s*([\\s\\S]*?)(?=\\*\\*[A-Z]|$)` ``) to slice seven fields out of free-form markdown. This sidesteps brittle JSON-mode failures on some models/providers and degrades gracefully — any missing section just renders empty instead of throwing.
- **Single mutable state object (`S`)** — domain, type, complexity index, temperature, model, history, and active chart instances all live in one plain object, keeping ~115 functions referencing a single, debuggable source of truth instead of scattered globals.
- **Defensive DOM access throughout** — virtually every DOM read uses optional chaining (`document.getElementById('x')?.value`), so the script never throws if a tab hasn't been rendered yet (tabs are lazily initialized).
- **XSS-aware rendering pipeline** — `esc()` escapes HTML entities for plain text injection; `san()` additionally strips `<script>` blocks and inline `on*` handlers before any AI-generated content is written via `innerHTML`. This matters specifically *because* the content originates from an LLM — an indirect, lower-trust input source.
- **Chart lifecycle management** — `renderAnalytics()` explicitly destroys (`Chart.getChart(id)?.destroy()`) and recreates Chart.js instances on every refresh, avoiding the classic "ghost canvas" memory leak from repeated `new Chart()` calls on the same `<canvas>`.
- **CSS `@property` for animated gradients** — `--glow-angle` is registered as a typed custom property (`syntax: '<angle>'`), enabling hardware-accelerated, GPU-friendly conic gradient rotation without per-frame JS.
- **Progressive enhancement on Share** — `shareConj()` tries `navigator.share()` first and silently falls back to `navigator.clipboard.writeText()`, covering both mobile share-sheet and desktop browsers in one code path.
- **Self-healing settings** — `loadSettings()` validates the persisted model against `VALID_MODELS` on every load and silently resets to `DEFAULT_MODEL` if Groq deprecates/renames a model id, preventing a stale `localStorage` entry from permanently breaking generation.

---

## 🚀 Getting Started

```bash
# 1. Clone
git clone https://github.com/<your-username>/mathematical-conjecture-proposer.git
cd mathematical-conjecture-proposer

# 2. Stand up any backend implementing the 3-endpoint contract above,
#    with GROQ_API_KEY set in its environment.

# 3. Serve the frontend (no build step required)
npx serve .
# or simply open index.html if your backend allows same-origin/static hosting
```

Then open the app, go to **Settings → Test Backend** to confirm `keyConfigured: true`, pick a model card, and hit **Generate Conjecture**.

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Markup / Styling | Semantic HTML5, Bootstrap 5.3 grid + components, custom CSS design-token system (`:root` variables), CSS `@property` |
| Typography | Cormorant Garamond (display serif), DM Sans / Inter (UI), JetBrains Mono (code & formulas) |
| Math Rendering | MathJax 3 (TeX-CHTML) |
| Data Visualization | Chart.js 4 |
| Motion | GSAP 3 + ScrollTrigger, CSS keyframe animations, Canvas 2D particle system |
| Icons | Bootstrap Icons |
| State / Persistence | Vanilla JS state object, `localStorage` (settings + history) |
| AI Inference | Groq LPU — LLaMA 3.1 / 3.3 / 4-Scout, GPT-OSS 20B/120B, Qwen3-32B |
| Backend (bring your own) | Any HTTP server implementing the `/api/health`, `/api/generate`, `/api/batch` contract |

---

## 🗺 Roadmap

- [ ] Reference backend implementation (Express + serverless variants) committed to `/server`
- [ ] Streaming token rendering for generation (SSE)
- [ ] Per-conjecture formal verification hooks (Lean/Coq sketch generation)
- [ ] Multi-user history sync (currently device-local via `localStorage`)
- [ ] Automated regression tests for `parseResp()` against model output drift

## 🤝 Contributing

Issues and PRs are welcome. Please open an issue describing the change before submitting a PR for anything beyond a trivial fix.

## 📄 License

MIT — see [`LICENSE`](LICENSE).

---

<div align="center">
<sub>Built for explorers of the mathematical unknown. All conjectures are AI-generated and require rigorous verification before any claim of truth.</sub>
</div>
