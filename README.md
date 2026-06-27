<div align="center">

```
 ███╗   ██╗███████╗██╗   ██╗██████╗  █████╗ ██╗
 ████╗  ██║██╔════╝██║   ██║██╔══██╗██╔══██╗██║
 ██╔██╗ ██║█████╗  ██║   ██║██████╔╝███████║██║
 ██║╚██╗██║██╔══╝  ██║   ██║██╔══██╗██╔══██║██║
 ██║ ╚████║███████╗╚██████╔╝██║  ██║██║  ██║███████╗
 ╚═╝  ╚═══╝╚══════╝ ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝

  ██████╗ ██████╗ ███╗   ██╗     ██╗███████╗ ██████╗████████╗██╗   ██╗██████╗ ███████╗
 ██╔════╝██╔═══██╗████╗  ██║     ██║██╔════╝██╔════╝╚══██╔══╝██║   ██║██╔══██╗██╔════╝
 ██║     ██║   ██║██╔██╗ ██║     ██║█████╗  ██║        ██║   ██║   ██║██████╔╝█████╗
 ██║     ██║   ██║██║╚██╗██║██   ██║██╔══╝  ██║        ██║   ██║   ██║██╔══██╗██╔══╝
 ╚██████╗╚██████╔╝██║ ╚████║╚█████╔╝███████╗╚██████╗   ██║   ╚██████╔╝██║  ██║███████╗
  ╚═════╝ ╚═════╝ ╚═╝  ╚═══╝ ╚════╝ ╚══════╝ ╚═════╝   ╚═╝    ╚═════╝ ╚═╝  ╚═╝╚══════╝

  ██████╗ ██████╗  ██████╗ ██████╗  ██████╗ ███████╗███████╗██████╗
  ██╔══██╗██╔══██╗██╔═══██╗██╔══██╗██╔═══██╗██╔════╝██╔════╝██╔══██╗
  ██████╔╝██████╔╝██║   ██║██████╔╝██║   ██║███████╗█████╗  ██████╔╝
  ██╔═══╝ ██╔══██╗██║   ██║██╔═══╝ ██║   ██║╚════██║██╔══╝  ██╔══██╗
  ██║     ██║  ██║╚██████╔╝██║     ╚██████╔╝███████║███████╗██║  ██║
  ╚═╝     ╚═╝  ╚═╝ ╚═════╝ ╚═╝      ╚═════╝ ╚══════╝╚══════╝╚═╝  ╚═╝
```

### *"Where large language models meet the frontier of human mathematical thought"*

---

![License](https://img.shields.io/badge/License-MIT-c9a227?style=for-the-badge&logo=open-source-initiative&logoColor=fff)
![Stack](https://img.shields.io/badge/Stack-Vanilla_JS_·_Bootstrap_5-00d4f5?style=for-the-badge&logo=javascript&logoColor=fff)
![AI](https://img.shields.io/badge/Powered_by-Groq_×_LLaMA_3-7c3aed?style=for-the-badge&logo=meta&logoColor=fff)
![Math](https://img.shields.io/badge/Rendering-MathJax_3-c9a227?style=for-the-badge&logo=latex&logoColor=fff)
![Animation](https://img.shields.io/badge/Animation-GSAP_3.12-88CE02?style=for-the-badge&logo=greensock&logoColor=fff)
![Responsive](https://img.shields.io/badge/Responsive-320px_→_∞-00d4f5?style=for-the-badge&logo=css3&logoColor=fff)

</div>

---

## ∑ Table of Contents

| # | Section |
|---|---------|
| 1 | [Project Overview](#-project-overview) |
| 2 | [Live Architecture Diagram](#-live-architecture-diagram) |
| 3 | [Feature Matrix](#-feature-matrix) |
| 4 | [Visual Layer System](#-visual-layer-system-hero) |
| 5 | [Design System & Tokens](#-design-system--tokens) |
| 6 | [AI Pipeline & Response Contract](#-ai-pipeline--response-contract) |
| 7 | [Supported Models](#-supported-models) |
| 8 | [Mathematical Domains & Conjecture Types](#-mathematical-domains--conjecture-types) |
| 9 | [Frontend State Machine](#-frontend-state-machine) |
| 10 | [Backend API Reference](#-backend-api-reference) |
| 11 | [LocalStorage Schema](#-localstorage-schema) |
| 12 | [Analytics Engine](#-analytics-engine) |
| 13 | [Typography System](#-typography-system) |
| 14 | [Responsive Breakpoints](#-responsive-breakpoints) |
| 15 | [Security Architecture](#-security-architecture) |
| 16 | [Keyboard Shortcuts](#-keyboard-shortcuts) |
| 17 | [Getting Started](#-getting-started) |
| 18 | [Project Structure](#-project-structure) |
| 19 | [Performance Profile](#-performance-profile) |
| 20 | [Browser Compatibility](#-browser-compatibility) |
| 21 | [Roadmap](#-roadmap) |
| 22 | [Contributing](#-contributing) |
| 23 | [Acknowledgements](#-acknowledgements) |
| 24 | [License](#-license) |

---

## ∑ Project Overview

**Neural Conjecture Proposer** is a cinematic, single-page AI application that harnesses Groq-hosted large language models to generate *novel, mathematically rigorous conjectures* across eight major domains of pure mathematics — from Number Theory and Topology to Differential Geometry and Set Theory.

Unlike generic AI chat interfaces, NCP encodes mathematical expertise directly into its system prompt and enforces a strict seven-section output contract, ensuring every generated conjecture includes a formal statement (in LaTeX), motivation, related results, concrete proof strategies, a difficulty classification, and semantic keywords. Each conjecture is instantly rendered with MathJax, persisted to localStorage, and made available for search, filter, export, and analytics.

The interface is engineered at observatory-grade visual fidelity: a seven-layer animated hero, 55-particle canvas field with connection-graph physics, GSAP ScrollTrigger parallax, a perpetual mathematical formula ticker, and a design token system inspired by the aesthetic of mathematical manuscripts — mathematical gold on absolute void.

```
∫∂∑  A platform built where mathematics meets machine intelligence.  ∇∀∃
```

---

## ∑ Live Architecture Diagram

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                          NEURAL CONJECTURE PROPOSER                             │
│                        ∑ Full System Architecture                               │
└─────────────────────────────────────────────────────────────────────────────────┘

  ┌──────────────────────────────────────────────────────────────────────────────┐
  │                          BROWSER (CLIENT LAYER)                              │
  │                                                                              │
  │  ┌────────────────┐  ┌────────────────┐  ┌────────────────┐                 │
  │  │   HERO SECTION │  │   APP SECTION  │  │  MODAL VIEWER  │                 │
  │  │                │  │                │  │                │                 │
  │  │ 7 Visual Layers│  │ 6 Tabs:        │  │ Fullscreen     │                 │
  │  │ ─ Canvas BG    │  │ ─ Generate     │  │ conjecture     │                 │
  │  │ ─ Grid Plane   │  │ ─ Batch        │  │ viewer with    │                 │
  │  │ ─ Symbol Field │  │ ─ Analytics    │  │ MathJax        │                 │
  │  │ ─ Formula Tags │  │ ─ History      │  │ rendering      │                 │
  │  │ ─ Scan Line    │  │ ─ Learn        │  │                │                 │
  │  │ ─ Orbital Deco │  │ ─ Settings     │  └────────────────┘                 │
  │  │ ─ Hero Content │  │                │                                      │
  │  └────────────────┘  └────────────────┘                                      │
  │           │                   │                                               │
  │           ▼                   ▼                                               │
  │  ┌──────────────────────────────────────────────────────────────────────┐    │
  │  │                     STATE MACHINE  (S object)                        │    │
  │  │                                                                      │    │
  │  │  model · domain · type · cx · temp · generating                      │    │
  │  │  hist[] · charts{} · hFilter · hSearch                               │    │
  │  └──────────────────────────────────────────────────────────────────────┘    │
  │           │                   │                                               │
  │           ▼                   ▼                                               │
  │  ┌──────────────┐    ┌────────────────────┐   ┌─────────────────────────┐   │
  │  │  localStorage │    │   callBackend()     │   │     MathJax 3           │   │
  │  │              │    │                    │   │                         │   │
  │  │  ncp_h[]     │    │  POST /api/generate│   │  typesetPromise()       │   │
  │  │  ncp_s{}     │    │  POST /api/batch   │   │  TeX → CHTML rendering  │   │
  │  │              │    │  GET  /api/health  │   │  inline $ and $$        │   │
  │  └──────────────┘    └────────────────────┘   └─────────────────────────┘   │
  └──────────────────────────────────────────────────────────────────────────────┘
                                    │
                          HTTP / REST API
                                    │
  ┌─────────────────────────────────▼──────────────────────────────────────────┐
  │                         BACKEND PROXY SERVER                                │
  │                    (Node.js / Express recommended)                          │
  │                                                                             │
  │  GET  /api/health    ─────────────────▶  { keyConfigured: boolean }         │
  │  POST /api/generate  ─────────────────▶  { content: string }               │
  │  POST /api/batch     ─────────────────▶  { results: BatchResult[] }        │
  │                                                                             │
  │  ┌─────────────────────────────────────────────────────────────────────┐   │
  │  │  SECURITY LAYER                                                      │   │
  │  │  ─ GROQ_API_KEY stored server-side only (env var)                   │   │
  │  │  ─ Model whitelist validation before forwarding                     │   │
  │  │  ─ Request sanitisation                                             │   │
  │  └─────────────────────────────────────────────────────────────────────┘   │
  └─────────────────────────────────────────────────────────────────────────────┘
                                    │
                          HTTPS (TLS encrypted)
                                    │
  ┌─────────────────────────────────▼──────────────────────────────────────────┐
  │                         GROQ CLOUD API                                      │
  │                    api.groq.com/openai/v1/chat/completions                  │
  │                                                                             │
  │  LLaMA 3.3-70b-versatile  │  LLaMA 3.1-8b-instant  │  GPT-OSS-120b        │
  │  GPT-OSS-20b              │  LLaMA-4-Scout-17b-16e  │  Qwen3-32b           │
  └─────────────────────────────────────────────────────────────────────────────┘
```

---

## ∑ Feature Matrix

| Feature | Description | Tab | Storage |
|---------|-------------|-----|---------|
| **Single Generation** | Domain + Type + Complexity + Temp + Max Tokens + Custom Context | Generate | `ncp_h` |
| **Batch Generation** | Up to N conjectures in one request, real-time progress bar | Batch | `ncp_h` |
| **MathJax Rendering** | Full LaTeX rendering (inline `$` and display `$$`) on every conjecture | All | — |
| **Analytics Dashboard** | 4 stat cards + 3 Chart.js visualisations (doughnut / bar / line) | Analytics | — |
| **History CRUD** | Full-text search, domain filter, timestamp, like/save, delete | History | `ncp_h` |
| **JSON Export / Import** | Download or re-import your entire conjecture archive | History | File |
| **Learn Accordion** | 6 famous conjectures with MathJax equations + open/proved status | Learn | — |
| **LaTeX Cheatsheet** | 12 one-click copy-to-clipboard LaTeX snippets | Settings | — |
| **Model Picker** | 6 Groq-hosted LLMs selectable at runtime | Settings | `ncp_s` |
| **System Prompt Editor** | Full customisation of the mathematician persona + output format | Settings | `ncp_s` |
| **Backend Health Check** | Live test of proxy connection and API key presence | Settings | — |
| **Formula Ticker** | Perpetual marquee of 12 landmark mathematical results | Hero | — |
| **Canvas Particle System** | 55 floating math symbols with connection-graph lines | Background | — |
| **GSAP Scroll Parallax** | Orbital, grid, and hero content parallax on scroll | Hero | — |
| **Toast Notifications** | 4-max stacked, auto-dismiss, OK / Error / Info variants | Global | — |
| **Native Share API** | `navigator.share` fallback to clipboard copy | Conjecture | — |
| **Keyboard Shortcuts** | ⌘/Ctrl+Enter to generate, Esc to dismiss modal | Global | — |
| **Print Stylesheet** | Clean print layout hiding UI chrome | Global | — |

---

## ∑ Visual Layer System (Hero)

The hero section is a **seven-layer composited** canvas system. Each layer is an independent visual subsystem:

```
 Layer │ Element               │ Technology         │ Animation
 ──────┼───────────────────────┼────────────────────┼─────────────────────────────
  0    │ bgCanvas              │ Canvas 2D API      │ rAF loop, 60 fps particle field
  1    │ .hero-grid-plane      │ CSS perspective 3D │ gridPulse (6s ease-in-out)
  2    │ .hero-sym-field       │ CSS @keyframes     │ symbolFloat (8–18s, staggered)
  3    │ .hero-formulas        │ CSS @keyframes     │ formulaDrift (9–12s, staggered)
  4    │ .hero-scanline        │ CSS @keyframes     │ scanSweep (linear, continuous)
  5    │ .hero-orbital         │ CSS animation      │ 4× orbSpin + dotPulse + glowBreathe
  6    │ .hero-content-wrap    │ GSAP ScrollTrigger │ fadeOut on scroll scrub
```

### Canvas Particle Engine (Layer 0)

The background canvas runs an optimised O(n²) connection-graph algorithm:

```javascript
// Connection threshold: 90px Euclidean distance
// Each frame: clear → draw edges → animate symbols
const SYM = ['∑','∫','∂','∈','∞','π','√','∇','∀','∃', /* 47 more */];
const PARTICLE_COUNT = 55;
const EDGE_OPACITY_FORMULA = 0.018 * (1 - dist / 90);  // linear falloff

// Each particle carries:
{ x, y, vx, vy, sym, sz, op, top, life }
// op = top × (0.65 + 0.35 × sin(life))  — breathing opacity
// Color: gold (#d4af37) or blue (#4f9cf9) based on sin(life × 1.3) > 0.3
```

### Orbital Decoration (Layer 5)

Four concentric rings animate independently via CSS:

```
Ring 1 (100%)  — rgba(201,162,39, 0.12) — orbSpin 25s linear
Ring 2 ( 76%)  — rgba(0,212,245,  0.10) — orbSpin 18s linear reverse
Ring 3 ( 52%)  — rgba(124,58,237, 0.14) — orbSpin 13s linear
Ring 4 ( 28%)  — rgba(201,162,39, 0.20) — orbSpin  8s linear reverse
Core: "∑"     — corePulse (3.5s, dual text-shadow intensity)
```

---

## ∑ Design System & Tokens

The entire visual language is encoded in CSS Custom Properties at `:root`. Every colour, spacing, easing, and font decision flows from this single source of truth:

### Colour Palette

```css
/* ── Void Palette ── */
--void:      #000000;   /* true black — body background */
--overlay:   rgba(3,3,10,0.85);

/* ── Mathematical Gold (Primary) ── */
--gold:       #c9a227;
--gold-l:     #e8c040;   /* light gold — headings, active states */
--gold-d:     #8a6e18;   /* dark gold  — muted accents, scrollbar */
--gold-glow:  rgba(201,162,39,0.45);
--gold-sub:   rgba(201,162,39,0.08);  /* active tab backgrounds */
--gold-bdr:   rgba(201,162,39,0.22);  /* active borders */
--gold-grad:  linear-gradient(135deg, #e8c040, #c9a227, #8a6e18);

/* ── Electric Cyan (Secondary) ── */
--cyan:      #00d4f5;
--cyan-d:    #0098b0;
--cyan-glow: rgba(0,212,245,0.3);

/* ── Deep Purple (Tertiary) ── */
--purple:      #7c3aed;
--purple-l:    #9d5cf6;

/* ── Semantic ── */
--err:  #f87171;   /* error / open conjecture status */
--ok:   #34d399;   /* success / proved status */
--warn: #fbbf24;   /* loading / warning state */
```

### Easing Library

```css
--ease:        cubic-bezier(0.4, 0, 0.2, 1);    /* material standard */
--ease-out:    cubic-bezier(0, 0, 0.2, 1);       /* decelerate — enters */
--ease-spring: cubic-bezier(0.34, 1.56, 0.64, 1); /* spring — brand logo hover */
--dur:         0.28s;                             /* base transition duration */
```

### CSS `@property` Declaration

```css
@property --glow-angle {
  syntax: '<angle>';
  initial-value: 0deg;
  inherits: false;
}
```
> This enables Houdini-powered animated conic-gradient glows without the usual `background-position` hack.

---

## ∑ AI Pipeline & Response Contract

### Request Payload

Every generation call sends a validated payload to the backend:

```typescript
interface GeneratePayload {
  domain:       string;   // e.g. "Number Theory"
  type:         string;   // e.g. "Existence"
  complexity:   string;   // "Undergraduate" | "Graduate" | "Research-level" | "Millennium-level"
  temperature:  number;   // 0.1 – 1.5
  maxTokens:    number;   // 800 | 1200 | 2000 | 3000
  context:      string;   // optional free-text constraint
  model:        string;   // validated against VALID_MODELS whitelist
  systemPrompt: string;   // customisable mathematician persona
}
```

### Batch Payload Extension

```typescript
interface BatchPayload extends Omit<GeneratePayload, 'domain' | 'type'> {
  domain: string;   // may be "Mixed" — backend resolves to random domain per item
  count:  number;   // number of conjectures to generate
  theme:  string;   // optional thematic constraint shared across batch
}
```

### Structured Output Contract

The system prompt enforces a **strict seven-section Markdown output format**:

```
**CONJECTURE TITLE**: [A specific, descriptive title]

**STATEMENT**: [Precise mathematical statement using LaTeX]

**MOTIVATION**: [2-3 sentences: why interesting? what patterns suggest truth?]

**RELATED RESULTS**: [Known theorems contextualising the conjecture]

**PROOF APPROACHES**: [2-3 concrete strategies — specific techniques or reductions]

**DIFFICULTY**: [Undergraduate | Graduate | Research-level | Millennium-level]

**KEYWORDS**: [5-8 comma-separated mathematical keywords]
```

### Response Parser (`parseResp`)

The client-side parser uses regex section extraction:

```javascript
// Section extraction pattern:
// \*\*SECTION TITLE\*\*:\s*([\s\S]*?)(?=\n\*\*[A-Z]|\n$|$)

const parsed = {
  title:      extractSection(raw, 'CONJECTURE TITLE'),
  statement:  extractSection(raw, 'STATEMENT'),
  motivation: extractSection(raw, 'MOTIVATION'),
  related:    extractSection(raw, 'RELATED RESULTS'),
  approaches: extractSection(raw, 'PROOF APPROACHES'),
  difficulty: extractSection(raw, 'DIFFICULTY'),
  keywords:   extractSection(raw, 'KEYWORDS')
              .split(',').map(k => k.trim()).filter(Boolean)
}
```

### History Entry Schema

Each generated conjecture is stored as a serialised object:

```typescript
interface HistoryEntry {
  id:         string;     // Date.now().toString() — unique key
  ts:         string;     // ISO 8601 timestamp
  domain:     string;
  type:       string;
  cx:         string;     // complexity label
  title:      string;
  statement:  string;     // includes $LaTeX$ markers
  motivation: string;
  related:    string;
  approaches: string;
  difficulty: string;
  keywords:   string[];
  raw:        string;     // original AI response for re-parsing
  liked:      boolean;    // favourited flag
}
```

---

## ∑ Supported Models

| Model ID | Provider | Parameters | Best For |
|----------|----------|-----------|----------|
| `llama-3.3-70b-versatile` | Meta (via Groq) | 70B | **Default.** Best balance of depth and speed |
| `llama-3.1-8b-instant` | Meta (via Groq) | 8B | Fast iteration, high-volume batch generation |
| `openai/gpt-oss-120b` | OpenAI OSS (via Groq) | 120B | Maximum depth, Millennium-level conjectures |
| `openai/gpt-oss-20b` | OpenAI OSS (via Groq) | 20B | Balanced quality for research-level work |
| `meta-llama/llama-4-scout-17b-16e-instruct` | Meta LLaMA 4 (via Groq) | 17B-16E MoE | Novel approach; efficient mixture-of-experts |
| `qwen/qwen3-32b` | Alibaba Qwen (via Groq) | 32B | Strong mathematical reasoning performance |

> **Model Selection Rationale:** All models are served via Groq's ultra-low-latency inference infrastructure. The `llama-3.3-70b-versatile` default provides an exceptional quality-to-latency ratio for graduate-level conjectures. For Millennium-level generation, switch to `gpt-oss-120b`.

---

## ∑ Mathematical Domains & Conjecture Types

### Domains (8)

| Symbol | Domain | Example Open Problem |
|--------|--------|---------------------|
| ℕ | **Number Theory** | Goldbach's Conjecture, Twin Prime Conjecture |
| ∮ | **Topology** | Smooth 4D Poincaré Conjecture |
| ∘ | **Abstract Algebra** | Inverse Galois Problem |
| ∫ | **Real Analysis** | Existence of smooth Navier–Stokes solutions |
| ₂ | **Combinatorics** | Hadwiger's Conjecture |
| ∇ | **Differential Geometry** | Yau's Calabi conjecture (proved 1977) |
| P | **Probability Theory** | Ergodic theory open questions |
| ∈ | **Set Theory** | Continuum Hypothesis independence results |

### Conjecture Types (7)

| Type | Logical Form | Example |
|------|-------------|---------|
| **Existence** | `∃x : P(x)` | There exists a prime with property X |
| **Inequality** | `f(n) ≤ g(n)` | Bound on gap between consecutive primes |
| **Equivalence** | `A ⟺ B` | Two number-theoretic conditions are equivalent |
| **Asymptotic** | `f(n) ~ g(n)` | Prime counting function asymptotics |
| **Classification** | Enumerate all X | Classify all finite simple groups variant |
| **Structural** | `X has structure Y` | Every manifold satisfying X is Y |
| **Open-ended** | Exploratory | Unconstrained; AI selects logical form |

### Complexity Scale

```
Level 1 — UNDERGRADUATE    ⎯ Provable with standard tools; accessible to a math undergrad
Level 2 — GRADUATE         ⎯ Requires advanced coursework; PhD-level techniques needed
Level 3 — RESEARCH-LEVEL   ⎯ Requires cutting-edge mathematical machinery; publishable territory
Level 4 — MILLENNIUM-LEVEL ⎯ Comparable in difficulty to a Clay Millennium Prize Problem ($1M)
```

---

## ∑ Frontend State Machine

The entire application state is managed in a single plain object `S`, making all transitions predictable and debuggable from the browser console:

```javascript
const S = {
  // Configuration
  model:      'llama-3.3-70b-versatile',   // selected model ID
  domain:     'Number Theory',              // selected mathematical domain
  type:       'Existence',                  // selected conjecture type
  cx:         2,                            // complexity index (1–4)
  temp:       0.7,                          // generation temperature

  // Runtime flags
  generating: false,                        // prevents concurrent requests

  // Data
  hist:       [],                           // HistoryEntry[] — all conjectures
  charts:     {},                           // Chart.js instance registry (for destroy/re-create)

  // History view state
  hFilter:    'all',                        // active domain filter
  hSearch:    ''                            // search query string
};
```

### Tab Navigation

Tabs are managed via CSS class toggling with a forced reflow animation replay:

```javascript
function switchTab(tab, btn) {
  // 1. Remove 'active' from all panels and buttons
  // 2. Add 'active' to target panel
  // 3. Force reflow: void p.offsetWidth
  // 4. Re-add 'anim' class to replay fadeInUp
  // 5. Lazy-render: Analytics re-renders charts on switch
  //                 History re-renders list on switch
}
```

---

## ∑ Backend API Reference

> The frontend communicates exclusively with your own backend proxy. **The Groq API key is never exposed to the browser.**

### `GET /api/health`

Health check — verifies server is live and API key is configured.

**Response:**
```json
{ "keyConfigured": true }
```

**Frontend behaviour on response:**
- `keyConfigured: true`  → status dot turns **green** (`.sdot.on`)
- `keyConfigured: false` → status dot turns **red** (`.sdot.er`), toast error
- Network error          → status dot turns **red**, toast error

---

### `POST /api/generate`

Generate a single conjecture.

**Request Body:**
```json
{
  "domain":       "Number Theory",
  "type":         "Existence",
  "complexity":   "Graduate",
  "temperature":  0.7,
  "maxTokens":    1200,
  "context":      "Focus on prime gaps and Cramér's model",
  "model":        "llama-3.3-70b-versatile",
  "systemPrompt": "You are a world-class mathematician..."
}
```

**Response:**
```json
{ "content": "**CONJECTURE TITLE**: ...\n\n**STATEMENT**: ..." }
```

**Error response:**
```json
{ "error": "Human-readable error message" }
```

---

### `POST /api/batch`

Generate multiple conjectures in a single server-side loop.

**Request Body:**
```json
{
  "domain":       "Mixed",
  "count":        3,
  "complexity":   "Research-level",
  "temperature":  0.7,
  "maxTokens":    1000,
  "context":      "Algebraic structures",
  "model":        "llama-3.3-70b-versatile",
  "systemPrompt": "..."
}
```

**Response:**
```json
{
  "results": [
    { "ok": true,  "content": "**CONJECTURE TITLE**...", "domain": "Topology", "type": "Structural" },
    { "ok": false, "error": "Rate limit exceeded", "domain": "Algebra", "type": "Existence" }
  ]
}
```

---

### Recommended Backend: Node.js / Express

```javascript
// server.js — minimal reference implementation
import express from 'express';
import Groq    from 'groq-sdk';

const app  = express();
const groq = new Groq({ apiKey: process.env.GROQ_API_KEY });

app.use(express.json());

const VALID_MODELS = [
  'llama-3.3-70b-versatile',
  'llama-3.1-8b-instant',
  'openai/gpt-oss-120b',
  'openai/gpt-oss-20b',
  'meta-llama/llama-4-scout-17b-16e-instruct',
  'qwen/qwen3-32b'
];

app.get('/api/health', (_, res) => {
  res.json({ keyConfigured: !!process.env.GROQ_API_KEY });
});

app.post('/api/generate', async (req, res) => {
  const { domain, type, complexity, temperature, maxTokens,
          context, model, systemPrompt } = req.body;

  if (!VALID_MODELS.includes(model))
    return res.status(400).json({ error: 'Invalid model' });

  const userMsg = `Generate a ${complexity} ${type} conjecture in ${domain}.${
    context ? ` Context: ${context}` : ''}`;

  try {
    const chat = await groq.chat.completions.create({
      model,
      temperature,
      max_tokens: maxTokens,
      messages: [
        { role: 'system', content: systemPrompt },
        { role: 'user',   content: userMsg }
      ]
    });
    res.json({ content: chat.choices[0].message.content });
  } catch (e) {
    res.status(500).json({ error: e.message });
  }
});

app.listen(3001, () => console.log('NCP backend on :3001'));
```

---

## ∑ LocalStorage Schema

NCP uses two `localStorage` keys, both serialised as JSON:

### `ncp_h` — History Array

```
Key:   "ncp_h"
Type:  JSON array of HistoryEntry objects
Limit: No enforced limit — grows unbounded; export/clear recommended periodically
```

```json
[
  {
    "id":         "1720000000000",
    "ts":         "2025-01-15T14:32:00.000Z",
    "domain":     "Number Theory",
    "type":       "Existence",
    "cx":         "Graduate",
    "title":      "On the Density of Primes in Quadratic Residues",
    "statement":  "Let $p$ be a prime and $\\mathbb{Q}_p$ be...",
    "motivation": "Motivated by Dirichlet's theorem on primes...",
    "related":    "Closely related to the Chebotarev density theorem...",
    "approaches": "1. Sieve methods — apply a weighted Brun sieve...",
    "difficulty": "Research-level",
    "keywords":   ["prime density", "quadratic residues", "L-functions"],
    "raw":        "**CONJECTURE TITLE**: On the Density...",
    "liked":      true
  }
]
```

### `ncp_s` — Settings Object

```
Key:   "ncp_s"
Type:  JSON object
```

```json
{
  "model":    "llama-3.3-70b-versatile",
  "sysPmt":   "You are a world-class mathematician...",
  "defDom":   "Number Theory",
  "defCx":    "2"
}
```

> **Note:** If a stored `model` value is not in the `VALID_MODELS` whitelist (e.g., a model was deprecated), it is automatically reset to `DEFAULT_MODEL` and the corrected value is persisted back to localStorage.

---

## ∑ Analytics Engine

The Analytics tab renders three Chart.js 4 visualisations computed live from `S.hist`:

### Stat Cards

| Card | Formula |
|------|---------|
| **Total Generated** | `S.hist.length` |
| **Favourited** | `S.hist.filter(x => x.liked).length` |
| **Domains Explored** | `new Set(S.hist.map(x => x.domain)).size` |
| **Avg Complexity** | `mean(hist.map(x => complexityToInt(x.difficulty)))` — scale 1–4 |

### Chart 1 — Domain Distribution (Doughnut)

```
Data:   { [domain]: count } for all 8 domains (zero-count domains omitted)
Colors: hsla(38 + i×28, 65%, 50 + i%2×8, 0.85) — golden-warm harmonic palette
Type:   Chart.js "doughnut"
```

### Chart 2 — Complexity Distribution (Bar)

```
Labels: ["Undergraduate", "Graduate", "Research-level", "Millennium-level"]
Colors: [blue, gold, red, brown] — difficulty severity gradient
Type:   Chart.js "bar" with borderRadius: 5
```

### Chart 3 — Activity Timeline (Line)

```
Window: Rolling 7-day lookback from today
Labels: Day-of-week abbreviations for the past 7 days
Data:   Count of conjectures generated each day
Style:  Gold line, fill: gold@8% opacity, tension: 0.35 (slight curve)
Type:   Chart.js "line"
```

> All charts are destroyed and re-created on each Analytics tab switch to prevent canvas context leaks.

---

## ∑ Typography System

Three typeface families form a deliberate hierarchy:

| Role | Family | Variable | Usage |
|------|---------|---------|-------|
| **Display / Serif** | Cormorant Garamond | `--fd` | Hero title, section headers, conjecture titles, footer quote |
| **Monospace / Code** | JetBrains Mono | `--fm` | LaTeX source, model names, status text, ticker, canvas symbols |
| **Body / UI** | DM Sans → Inter | `--fs` | All UI copy, labels, badges, navigation, descriptions |

### Type Scale (hero)

```
.htl-1   clamp(2.2rem, 5.5vw, 4.5rem)   weight: 300   colour: --tx
.htl-2   clamp(2.8rem, 7.0vw, 5.8rem)   weight: 700   colour: shimmerGold gradient
```

### Shimmer Gold Animation

The hero title gradient animates via `background-position`:

```css
@keyframes shimmerGold {
  0%, 100% { background-position: 0% 50%; }
  50%       { background-position: 100% 50%; }
}
/* background-size: 200% 200% — enables position-based shimmer travel */
```

---

## ∑ Responsive Breakpoints

Full mobile-first responsive system across six breakpoints:

| Breakpoint | Width | Key Changes |
|------------|-------|-------------|
| **XS** | ≤ 399.98px | Stacked hero stats, reduced font sizes, single-column grids |
| **Mobile** | ≤ 767.98px | Orbital hidden, formula tags hidden, CTA buttons full-width, `100svh` hero |
| **Tablet** | ≤ 991.98px | Orbital reduced opacity (0.4), 2-col batch grid |
| **Navbar Break** | ≤ 1199.98px | Hamburger menu, nav collapses to full-width panel |
| **Large** | ≥ 1400px | Hero content max-width 760px, orbital 460px |
| **XL** | ≥ 1800px | Hero content 820px with extra left padding, orbital 500px |

### Mobile Hero Specifics

```css
/* Mobile: use svh for better address-bar handling */
min-height: 100svh;

/* Symbol field: first 9 symbols only (performance) */
.hero-sym-field .hsym:nth-child(n+10) { display: none; }

/* Grid plane: smaller cells on mobile */
background-size: 50px 50px;  /* vs 80px 80px on desktop */
```

---

## ∑ Security Architecture

NCP follows a strict **backend-proxy security model**. No API credentials ever reach the browser.

```
┌───────────────┐         ┌───────────────────┐         ┌─────────────┐
│    Browser    │──POST──▶│  Your Backend     │──HTTPS─▶│  Groq API   │
│               │         │  /api/generate    │         │             │
│  (no API key) │◀──JSON──│  GROQ_API_KEY     │◀──JSON──│             │
│               │         │  (env var only)   │         │             │
└───────────────┘         └───────────────────┘         └─────────────┘
```

### Client-Side XSS Protection

All user-influenced text is sanitised before DOM insertion via two helpers:

```javascript
// esc() — HTML entity encoding for text nodes
function esc(s) {
  return String(s)
    .replace(/&/g, '&amp;')
    .replace(/</g, '&lt;')
    .replace(/>/g, '&gt;');
}

// san() — strips inline event handlers and <script> tags from AI-generated HTML
function san(s) {
  return s
    .replace(/<script\b[^<]*(?:(?!<\/script>)<[^<]*)*<\/script>/gi, '')
    .replace(/on\w+\s*=\s*"[^"]*"/gi, '');
}
```

### Model Whitelist

Before any request reaches Groq, the backend validates the model string against a hardcoded whitelist. Any unlisted model ID returns `HTTP 400`.

```javascript
const VALID_MODELS = [
  'llama-3.3-70b-versatile',
  'llama-3.1-8b-instant',
  'openai/gpt-oss-120b',
  'openai/gpt-oss-20b',
  'meta-llama/llama-4-scout-17b-16e-instruct',
  'qwen/qwen3-32b'
];
```

---

## ∑ Keyboard Shortcuts

| Shortcut | Context | Action |
|----------|---------|--------|
| `Ctrl` / `⌘` + `Enter` | Generate tab active | Trigger `generateConjecture()` |
| `Escape` | Modal open | Close conjecture modal (`closeMod()`) |

---

## ∑ Getting Started

### Prerequisites

```
Node.js   ≥ 18.0.0  (backend server)
npm       ≥ 9.0.0
GROQ_API_KEY  (obtain from console.groq.com)
```

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/neural-conjecture-proposer.git
cd neural-conjecture-proposer

# 2. Install backend dependencies
cd server
npm install

# 3. Set your Groq API key
cp .env.example .env
# Edit .env → GROQ_API_KEY=your_key_here

# 4. Start the backend proxy
npm start
# → Backend running on http://localhost:3001

# 5. Serve the frontend
# Option A: VS Code Live Server (port 5500)
# Option B: npx serve . (from project root)
# Option C: any static file server

# 6. Open index.html in browser and click Settings → Test Connection
```

### Environment Variables

| Variable | Required | Description |
|----------|----------|-------------|
| `GROQ_API_KEY` | ✅ Yes | Your Groq API key — never exposed to client |
| `PORT` | No | Backend port (default: `3001`) |
| `ALLOWED_ORIGIN` | No | CORS origin for production (default: `*`) |

---

## ∑ Project Structure

```
neural-conjecture-proposer/
│
├── index.html                  # ← Single-file frontend (3553 lines)
│   ├── <head>                  #   Fonts, Bootstrap CSS, MathJax, GSAP, Chart.js
│   ├── <style> (CSS)           #   20 sections, ~2000 lines of design tokens + components
│   └── <body>                  #   Canvas, Navbar, Hero, Ticker, App Section, Scripts
│       ├── #bgCanvas           #     Particle system canvas
│       ├── nav.nb              #     Bootstrap responsive navbar (6 tabs + status)
│       ├── section.hero        #     7-layer animated hero
│       ├── div.ticker          #     Formula marquee
│       └── section.app         #     6 tab panels
│           ├── #tp-gen         #       Generate tab
│           ├── #tp-batch       #       Batch tab
│           ├── #tp-analytics   #       Analytics tab (3 Chart.js)
│           ├── #tp-hist        #       History tab (CRUD)
│           ├── #tp-learn       #       Learn accordion (6 conjectures)
│           └── #tp-settings    #       Settings (model picker, system prompt)
│
├── server/
│   ├── server.js               # Express proxy server (recommended)
│   ├── package.json
│   └── .env.example            # GROQ_API_KEY=
│
└── README.md                   # ← You are here
```

---

## ∑ Performance Profile

### Bundle Composition (CDN, no build step)

| Resource | Size (gzip approx.) | Priority |
|----------|--------------------|----|
| Bootstrap 5.3.2 CSS | ~30KB | High |
| Bootstrap 5.3.2 JS | ~19KB | Low (deferred) |
| GSAP 3.12.5 | ~30KB | Medium |
| GSAP ScrollTrigger | ~16KB | Medium |
| Chart.js 4.4.0 | ~60KB | Low (lazy loaded by tab) |
| MathJax 3 (tex-chtml) | ~300KB | Async (non-blocking) |
| Google Fonts (4 families) | ~60KB | Preconnected |
| **index.html (inline)** | ~110KB raw | Critical path |

### Rendering Strategy

- **MathJax** is loaded `async` — never blocks first paint
- **Chart.js** charts are created only when the Analytics tab is first switched to
- **Canvas** starts only after `DOMContentLoaded`
- **GSAP ScrollTrigger** animations use `will-change: transform` on animated elements
- **Tab switches** use CSS `display` toggle + forced reflow for animation replay (zero reflow in static state)
- **History rendering** is deferred to tab switch — large history arrays don't block initial render

### Optimisation Notes

```javascript
// Canvas: symbols outside viewport wrap (no DOM cost)
if (p.x < -60) p.x = W + 60;
if (p.y < -60) p.y = H + 60;

// Chart.js: destroy before re-create prevents canvas context accumulation
['domChart','cxChart','actChart'].forEach(id => {
  if (S.charts[id]) { try { S.charts[id].destroy(); } catch {} }
});

// MathJax: called only on visible containers, not whole document
MathJax.typesetPromise([container]).catch(() => {});
```

---

## ∑ Browser Compatibility

| Browser | Version | Notes |
|---------|---------|-------|
| Chrome / Edge | ≥ 105 | Full support including `@property` Houdini |
| Firefox | ≥ 110 | Full support; `@property` fallback acceptable |
| Safari | ≥ 16 | `backdrop-filter` and `-webkit-background-clip` supported |
| Mobile Chrome | ≥ 105 | `100svh` unit used for correct mobile viewport |
| Mobile Safari | ≥ 16 | Full support |

> **`@property`**: Used for `--glow-angle` CSS Houdini. Browsers without Houdini support receive a graceful static fallback — no layout breakage.

> **`navigator.share`**: Used for the Share button. Falls back to `navigator.clipboard.writeText` on unsupported browsers (e.g. desktop Firefox).

---

## ∑ Roadmap

### Version 2.0 — Near Term

- [ ] **Streaming responses** — `EventSource` / Server-Sent Events for character-by-character conjecture rendering
- [ ] **Export to LaTeX** — Download full conjecture as a `.tex` document with `\begin{theorem}` environment
- [ ] **PDF Export** — Client-side `window.print()` styled for academic paper format
- [ ] **Conjecture tagging** — User-defined tags beyond domain (e.g., `#prime-gaps`, `#open`, `#verified`)
- [ ] **Cross-domain comparison** — Side-by-side diff of two generated conjectures

### Version 3.0 — Medium Term

- [ ] **Collaborative mode** — Shareable conjecture URLs with encoded state
- [ ] **Proof attempt logger** — Attach personal proof notes to each conjecture
- [ ] **Citation parser** — Auto-detect and link mathematician names to Wikipedia / arXiv
- [ ] **Semantic similarity search** — Embed conjectures and retrieve nearest neighbours
- [ ] **Multi-modal** — Upload a paper/diagram; generate conjectures inspired by it

### Long-Term Vision

- [ ] **Integration with arXiv API** — Detect if a generated conjecture resembles a known paper
- [ ] **Formal verification assistant** — Hook into Lean 4 / Isabelle for automated proof checking
- [ ] **Community gallery** — Opt-in public feed of the most interesting community-generated conjectures

---

## ∑ Contributing

Contributions are deeply welcome — whether you are a mathematician, frontend engineer, or AI researcher.

### Development Workflow

```bash
# Fork → clone → branch
git checkout -b feature/your-feature-name

# Make changes to index.html or server/
# Test across Chrome, Firefox, Safari, and mobile viewport

# Commit with conventional commit format
git commit -m "feat(analytics): add keyword frequency word cloud chart"
git commit -m "fix(parser): handle multi-line STATEMENT sections correctly"
git commit -m "perf(canvas): reduce particle count on mobile to 25"
git commit -m "docs(readme): add backend Deno deployment guide"

# Push and open a Pull Request
```

### Areas Where Help Is Especially Welcome

- **Mathematics review** — Validating that the system prompt elicits genuinely novel, non-trivially-false conjectures
- **Backend implementations** — Deno Deploy, Cloudflare Workers, Python/FastAPI, Bun variants
- **Accessibility** — ARIA labels, keyboard navigation completeness, screen reader testing
- **Performance** — Canvas worker thread, lazy-loading Chart.js, MathJax bundle reduction
- **New domains** — Algebraic Geometry, Mathematical Logic, Mathematical Physics

### Code Style

- **No build step** — this is intentional. The project must remain a single `index.html` + thin server.
- Use `const` and `let`; no `var`
- All DOM helpers follow the `if (!el) return;` guard pattern
- CSS: add new design tokens to `:root` before hardcoding values

---

## ∑ Acknowledgements

This project stands on the shoulders of giants — both mathematical and technological:

| Contribution | Credit |
|-------------|--------|
| **Ultra-fast LLM inference** | [Groq](https://groq.com) — Language Processing Units make real-time generation feasible |
| **LLaMA 3 models** | [Meta AI](https://ai.meta.com) — Open-weight foundation models |
| **MathJax** | [MathJax Consortium](https://www.mathjax.org) — The gold standard for web mathematics rendering |
| **GSAP** | [GreenSock](https://greensock.com) — Industry-standard animation toolkit |
| **Bootstrap** | [Bootstrap Team](https://getbootstrap.com) — Responsive grid and component foundation |
| **Chart.js** | [Chart.js Contributors](https://www.chartjs.org) — Beautiful declarative charts |
| **JetBrains Mono** | [JetBrains](https://www.jetbrains.com/lp/mono) — The monospace typeface that makes math beautiful |
| **Cormorant Garamond** | [Christian Thalmann](https://github.com/CatharsisFonts/Cormorant) — The serif of mathematical manuscripts |
| **Mathematical Heritage** | Riemann, Goldbach, Euler, Perelman, Wiles, Birch, Swinnerton-Dyer, and every mathematician whose open problems inspired this platform |

---

## ∑ Learn Section — Conjecture Reference

The built-in Learn tab covers these six landmark problems:

| Conjecture | Year | Domain | Status | Prize |
|------------|------|--------|--------|-------|
| **Riemann Hypothesis** | 1859 | Analytic Number Theory | 🔴 Open | $1M (Clay) |
| **Goldbach's Conjecture** | 1742 | Number Theory | 🔴 Open | — |
| **Twin Prime Conjecture** | ~300 BC | Number Theory | 🔴 Open | — |
| **P vs NP** | 1971 | Computational Complexity | 🔴 Open | $1M (Clay) |
| **Poincaré Conjecture** | 1904 | Topology | ✅ Proved (Perelman 2003) | Declined |
| **Birch & Swinnerton-Dyer** | 1965 | Algebraic Geometry | 🔴 Open | $1M (Clay) |

---

## ∑ License

```
MIT License

Copyright (c) 2025 Neural Conjecture Proposer Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

---

<div align="center">

```
∑  e^{iπ} + 1 = 0  ·  ∀ε>0 ∃δ>0  ·  ζ(s) = ∏ 1/(1−p^{−s})  ·  P ≟ NP  ∑
```

**Built for mathematicians, by people who believe AI should expand the frontier of human knowledge.**

*"Mathematics is the art of giving the same name to different things."*
— Henri Poincaré

---

[![Star on GitHub](https://img.shields.io/github/stars/your-username/neural-conjecture-proposer?style=social)](https://github.com/your-username/neural-conjecture-proposer)
[![Follow](https://img.shields.io/github/followers/your-username?style=social)](https://github.com/your-username)

</div>
