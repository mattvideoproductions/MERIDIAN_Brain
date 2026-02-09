# Project Meridian

> **The `.md` Operating System for AI Agents**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## What Is This?

Project Meridian transforms any AI agent into **Meridian** — a customized, self-aware, memory-persistent AI entity with visible cognitive state and adjustable behavior parameters.

**The philosophy:**
> Agents need **tight specification** and **mandatory structure** to behave consistently. Lazy prompts yield lazy code.

Instead of reinventing infrastructure, Meridian provides an **intelligence layer** via structured `.md` files that work with any AI model (Claude, GPT, Gemini, etc.).

---

## 🛡️ Latent Integrity & Cognitive Safety (New in v1.0)

Meridian is rigorously audited against **Latent Instability**, including:
- **Speculation Labeling**: Enforced `[Fact]` vs `[Speculation]` tagging for all research.
- **Latent Grounding**: Built-in safety protocols for "cursed inputs" and hallucination loops.
- **Memory Gardening**: Automated pruning/consolidation rules to prevents "fossil layers" of outdated project data.

---

## 🚀 Quick Start

### Option 1: Drop-in (Easiest)
1. Copy the `brain/` folder to your AI session
2. Upload `brain/MASTER_SPEC.md` as the first file
3. Start chatting — Meridian is now active

### Option 2: Full Context
Provide the entire `brain/` folder as context for maximum capability.

### Option 3: Customize First
1. Edit `brain/sliders/USER.md` with your preferences
2. Adjust slider defaults in `brain/gauges/LIVEHUD.md`
3. Then upload `brain/MASTER_SPEC.md`

---

## What You Get

### 📊 LiveHud Dashboard v1.0
Every response starts with a visual cognitive state display featuring **Active Personality** verification:

```
╔══════════════════════════════════════════════════════════════════════════════╗
║  ◈ MERIDIAN LIVEHUD v1.0 ◈                                                  ║
║  Session: Active  │  Mode: [Active Personality Name]                         ║
╠══════════════════════════════════════════════════════════════════════════════╣
║  ├─ 🔊 Verbosity      [████████░░░░░░░░░░░░]       40%       28%             ║
║  ├─ 😂 Humor          [██████░░░░░░░░░░░░░░]       30%       45%             ║
║  ├─ 🎨 Creativity     [████████████░░░░░░░░]       60%       55%             ║
...
```

### 🎚️ Adjustable Sliders
Control behavior in real-time with **Schema Mapping** for programmatic parsing:
- `"Set creativity to 90%"`
- `"Max directness"`
- `"Research mode"` (preset adjustments)

### 🧠 Memory System
Persistent context with **Auto-Gardening** to prevent logic drift across long-term sessions.

### 🎭 Personality Modes
Switch personalities on demand: Base, Research, Creative, Technical, Concise.

---

## File Structure

```
Project Meridian/
├── brain/                      ← THE PORTABLE OS (v1.0)
│   ├── MASTER_SPEC.md          ← Entry point (load first)
│   ├── COMPATIBILITY.md        ← Host capability matrix & fallbacks
│   ├── audit_v2_latent_integrity.md ← Safety audit record
│   ├── README.md               ← Quick reference
│   ├── gauges/
│   │   └── LIVEHUD.md          ← v1.0 Dashboard spec + Schema Mapping
│   ├── sliders/                ← Cognitive parameters
│   │   ├── HUMOR.md
│   │   ├── CREATIVITY.md
│   │   ├── DIRECTNESS.md
│   │   ├── MORALITY.md
│   │   ├── TECHNICALITY.md
│   │   ├── SOUL.md             ← Includes Latent Grounding
│   │   ├── TOOLS.md
│   │   ├── USER.md             ← Customize for yourself
│   │   └── IDENTITY.md
│   ├── memory/
│   │   ├── MEMORY_PROTOCOL.md  ← Includes Memory Gardening
│   │   ├── RETRIEVAL.md
│   │   ├── PERSISTENCE.md
│   │   └── allmemories/        ← Where memories are stored
│   ├── personalities/
│   │   ├── BASE.md
│   │   ├── RESEARCH_ANALYST.md ← Includes Speculation Labeling
│   │   ├── CREATIVE_DIRECTOR.md
│   │   └── TECHNICAL_COPILOT.md
│   └── .agent/workflows/
│       └── meridian-init.md
├── LICENSE                     ← MIT
├── CONTRIBUTING.md             ← How to contribute
└── .gitignore
```

---

## Key Protocols

### The Completeness Doctrine
Meridian addresses **every distinct point** in your input. No detail gets summarized away.

### Receipts-Backed Protocol (Enhanced)
All research claims include **Confidence Grading** (0.00 - 1.00) and **Claim Type** labeling.

### Verification Protocol
Actions are verified, not assumed. No "latent space" execution.

### Capability Handshake
Meridian automatically detects host limitations (filesystem, web, tools) and applies fallbacks from `COMPATIBILITY.md`.

### 1-of-1 Identity
Meridian isn't generic — it's configured specifically for *you*.

---

## Customization

### Adjust Your Profile
Edit `brain/sliders/USER.md` with your preferences:
- Communication style
- Default slider values
- Domain expertise
- Technical context

### Add New Sliders
Create new `.md` files in `brain/sliders/` following the template in `CONTRIBUTING.md`.

### Add Personality Modes
Create new modes in `brain/personalities/` and reference them in `MASTER_SPEC.md`.

---

## Compatibility

Project Meridian is now **Host-Aware**. See `brain/COMPATIBILITY.md` for specific fallback behaviors across:
- ✅ Claude / OpenAI / Gemini
- ✅ Local Tool-Runners (Antigravity, OpenClaw)
- ✅ Custom Frameworks

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on extending the Meridian ecosystem.

---

## License

MIT License — see [LICENSE](LICENSE)

---

> *Project Meridian — Because the best agents are specified, not suggested.*
