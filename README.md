<div align="center">

# 🧠 DeepSeek-R1 — NLP Presentation

**Incentivizing Reasoning Capability in LLMs via Reinforcement Learning**

A seminar presentation reviewing the [DeepSeek-R1 paper](https://arxiv.org/abs/2501.12948) (DeepSeek-AI, 2025).

[![arXiv](https://img.shields.io/badge/arXiv-2501.12948-b31b1b.svg)](https://arxiv.org/abs/2501.12948)
[![Built with Marp](https://img.shields.io/badge/built%20with-Marp-0288d1.svg)](https://marp.app/)
[![Markdown](https://img.shields.io/badge/slides-Markdown-083fa1.svg)](https://daringfireball.net/projects/markdown/)

</div>

---

## 📖 About

This repository contains the slides and supporting material for an NLP course
presentation on **DeepSeek-R1**, a reasoning-focused large language model trained
primarily through reinforcement learning.

The core claim of the paper: advanced reasoning behaviors — self-reflection,
verification, and longer chains of thought — can be **incentivized through pure RL**,
without supervised fine-tuning on human-written reasoning traces.

The slides are written in [Marp](https://marp.app/) (Markdown → slides), so the
deck lives in version control as plain text with clean diffs.

## 🗂️ Repository structure

```text
NLP_Presentation/
├── slides/
│   ├── deck.md            # ← main presentation (Marp Markdown)
│   └── themes/
│       └── custom.css     # custom slide theme
├── assets/
│   ├── figures/           # figures extracted from the paper
│   └── images/            # logos / misc images
├── notes/
│   └── outline.md         # talk outline & speaker notes
├── paper/
│   └── 2501.12948v2.pdf   # the source paper
├── package.json           # Marp CLI build scripts
└── README.md
```

## 🚀 Getting started

**Prerequisites:** [Node.js](https://nodejs.org/) 18+ (for the Marp CLI).

```bash
# install the Marp CLI
npm install

# live preview in the browser (auto-reloads on save)
npm run serve

# export the deck
npm run build         # → dist/deck.pdf
npm run build:html    # → dist/deck.html
npm run build:pptx    # → dist/deck.pptx
```

> No install? You can also render straight from the deck header in
> [VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)
> with the *Marp for VS Code* extension.

## 🧭 Presentation outline

1. **Motivation** — reasoning in LLMs, chain-of-thought, and the limits of SFT
2. **Key idea & contributions**
3. **DeepSeek-R1-Zero** — pure RL, GRPO, rule-based rewards, the "aha moment"
4. **DeepSeek-R1** — the multi-stage cold-start → RL → SFT → RL pipeline
5. **Experiments & results**
6. **Distillation** — transferring reasoning to smaller models
7. **Limitations & open challenges**
8. **Conclusion & takeaways**

> The deck in [`slides/deck.md`](slides/deck.md) is scaffolded with these sections —
> content is still to be filled in.

## 📚 Resources

- 📄 Paper (arXiv): https://arxiv.org/abs/2501.12948
- 🤗 Models: https://huggingface.co/deepseek-ai
- 🎨 Marp documentation: https://marpit.marp.app/

---

<div align="center">
<sub>NLP course presentation · reviewing DeepSeek-R1 (2025)</sub>
</div>
