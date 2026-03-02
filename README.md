# 🧠 NeuroNav — AI Cognitive Co-Pilot for Neurodivergent Professionals

[![MIT License](https://img.shields.io/badge/License-MIT-teal.svg)](LICENSE)
[![Built with Claude](https://img.shields.io/badge/Powered%20by-Claude%20AI-orange)](https://anthropic.com)
[![Status: Active Development](https://img.shields.io/badge/Status-Active%20Development-brightgreen)]()
[![Neurodivergent-Led](https://img.shields.io/badge/Neurodivergent-Led%20Project-%23a78bfa)]()
[![Building in Public](https://img.shields.io/badge/Building-in%20Public-%2300e5c8)]()

> **Reducing cognitive friction. Supporting authentic communication. Built by and for neurodivergent minds.**

---

## 📌 What Is NeuroNav?

NeuroNav is an open-source, AI-powered support system designed for neurodivergent professionals navigating ADHD, Autism Spectrum Disorder, dyslexia, and related cognitive profiles. Unlike traditional "assistive technology" that tries to fix how neurodivergent people think, **NeuroNav meets you where you are** — providing scaffolding that reduces friction without forcing masking.

The tool is built on a core belief: **neurodivergent brains are not broken. Environments are.**

---

## ✨ Features

### Module 1 — Executive Function Scaffolding 🧩

| Feature | Description |
|---|---|
| **Task Decomposition** | LLM breaks overwhelming tasks into granular micro-steps (<5 min each) |
| **Adaptive Modes** | Standard / ADHD Mode (gamified, dopamine hooks) / Burnout Mode (ultra-gentle) |
| **Time Estimation** | Each step includes a realistic time estimate to combat time blindness |
| **Progress Tracking** | Interactive checklist with completion state — visual momentum feedback |
| **Body Doubling** *(roadmap)* | Virtual accountability companion for focus sessions |
| **Distraction Detection** *(roadmap)* | On-device behavioral cue monitoring for adaptive nudges |

### Module 2 — Social Communication Assistant 💬

| Feature | Description |
|---|---|
| **Tone Analysis** | Scores drafts across Directness, Perceived Warmth, Assertiveness, Formality |
| **Neurotypical Bridge** | Explains how a colleague is likely to interpret your message |
| **Intent-Preserving Rewrite** | Suggests a softer version without losing your authentic voice |
| **Context Modes** | Professional email / Slack / Peer feedback / Help requests |
| **Real-Time Drafting** *(roadmap)* | Live tone feedback as you type |
| **Facial Expression Reading** *(roadmap)* | On-device camera analysis for virtual meetings |

---

## 🏗️ Architecture

```
neuronav/
├── src/
│   ├── modules/
│   │   ├── exec-function/      # Task breakdown engine
│   │   └── social-comm/        # Tone analysis & rewriter
│   ├── components/             # Shared UI components
│   ├── hooks/                  # Custom React hooks
│   └── lib/
│       ├── claude.ts           # Anthropic API client
│       └── prompts.ts          # System prompt templates
├── on-device/                  # Future: local ML models (privacy-first)
│   ├── attention-monitor/      # Tab/focus behavioral inference
│   └── emotion-recognition/    # Facial expression classifier
├── docs/                       # Architecture decisions
└── README.md
```

**Current Stack:**
- **Frontend:** React + Tailwind CSS
- **AI:** Anthropic Claude API (`claude-sonnet-4`)
- **Future On-Device:** TensorFlow.js / ONNX Runtime (for privacy-preserving local inference)

---

## 🔒 Privacy Philosophy

> *"Sensitive social interactions and personal emotional data should never touch external servers."*

NeuroNav is designed with a **local-first, privacy-by-default** architecture:

- ✅ Task decomposition: stateless, no history stored
- ✅ Tone analysis: conversation content never logged
- 🔄 Roadmap: emotion recognition runs entirely on-device via WebAssembly
- 🔄 Roadmap: attention monitoring via local behavioral inference only

---

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/neuronav.git
cd neuronav

# Install dependencies
npm install

# Add your Anthropic API key
cp .env.example .env
# Edit .env: VITE_ANTHROPIC_API_KEY=your_key_here

# Start development server
npm run dev
```

> **Note:** A hosted demo (no API key required) is coming soon.

---

## 🗺️ Roadmap

See [ROADMAP.md](ROADMAP.md) for the full phased plan. At a glance:

- [x] **MVP** — Task breakdown + Tone analyzer (web prototype)
- [ ] **Phase 2** — Real-time drafting assistant, browser extension
- [ ] **Phase 3** — Attention monitoring, body doubling sessions
- [ ] **Phase 4** — On-device emotion recognition, wearable integration
- [ ] **Phase 5** — Mobile app (iOS / Android)

---

## 🤝 Contributing

This is a **solo developer project building in public**. Contributions, feedback, and lived-experience perspectives are warmly welcomed.

**Ways to contribute:**
- 🐛 File issues — bugs, UX friction, confusing prompts
- 💬 Share your neurodivergent experience — what tools do you wish existed?
- 🔧 Submit PRs — especially for accessibility improvements
- 📖 Improve documentation

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a PR.

---

## 🌍 Why This Exists

Studies indicate that **85% of neurodivergent millennials use AI in everyday tasks** to manage cognitive load — more than any other demographic. Yet most AI tools are built for neurotypical workflows.

Neurodivergent professionals often possess exceptional pattern recognition, creative systems thinking, and resilience. The barrier isn't capability — it's **cognitive friction** created by environments that weren't designed for how we process the world.

NeuroNav aims to be infrastructure, not a crutch. A scaffold that helps neurodivergent people operate authentically in neurotypical-designed spaces, without forcing them to mask.

---

## 📓 Building in Public

I'm documenting the full journey — technical decisions, failures, pivots, and lessons — on:

- **GitHub Discussions** — architecture decisions and research
- **LinkedIn** — weekly build logs and reflections
- **README changelog** — honest progress tracking

---

## 📄 License

MIT — free to use, fork, and build upon. If NeuroNav helps you, consider starring ⭐ the repo or sharing it with someone who needs it.

---

<div align="center">
  <sub>Built with 🧠 by a neurodivergent developer, for the community.</sub><br/>
  <sub>If this resonates, connect on <a href="#">LinkedIn</a>.</sub>
</div>
