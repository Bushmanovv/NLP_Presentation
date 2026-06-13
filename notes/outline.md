# Talk outline & speaker notes

Working notes for the DeepSeek-R1 presentation. Each section maps to a divider in
[`slides/deck.md`](../slides/deck.md). Fill in talking points, then transfer the
polished version to the slides.

> **Target length:** ~__ minutes · **Audience:** NLP course

---

## 1 · Motivation
- _Hook:_ can a model learn to reason without being shown how?
- Reasoning as the cornerstone of intelligence; chain-of-thought (CoT) prompting.
- The problem with SFT on human reasoning traces: scalability, human bias, quality cap.

## 2 · Key idea & contributions
- Hypothesis: reasoning can be **incentivized via pure RL** — no SFT on reasoning traces.
- Contributions: R1-Zero (pure RL), R1 (multi-stage pipeline), distillation to small models.

## 3 · DeepSeek-R1-Zero
- **GRPO** — group-relative advantage, no critic model; contrast with PPO.
- **Rewards** — rule-based only (accuracy + format); why no neural reward model.
- **Emergence** — AIME 15.6% → 77.9%; growing response length; the "aha moment".

## 4 · DeepSeek-R1
- Multi-stage pipeline: cold-start long CoT → reasoning RL → rejection sampling + SFT → final RL.
- Why each stage exists (readability, language mixing, alignment).

## 5 · Experiments & results
- Table 3 highlights; Dev1 → Dev3 progression and trade-offs.

## 6 · Distillation
- Small distilled models beat their instruction-tuned counterparts.
- The accessibility / cost argument.

## 7 · Limitations & open challenges
- Structured output / tool use, token efficiency (overthinking), language mixing,
  software-engineering tasks, prompt sensitivity, reward hacking.

## 8 · Conclusion
- 3–4 crisp takeaways; the "pure RL unlocks reasoning" message; future work.

---

## Figures to extract from the paper
- [ ] Fig. 1 — AIME accuracy & response length during R1-Zero training
- [ ] Table 2 — the "aha moment"
- [ ] Fig. 2 — the multi-stage R1 pipeline
- [ ] Fig. 3 — PPO vs GRPO
- [ ] Table 3 — results across stages

> Save extracted images to [`../assets/figures/`](../assets/figures/).
