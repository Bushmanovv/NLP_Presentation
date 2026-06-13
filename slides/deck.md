---
marp: true
theme: deepseek
paginate: true
size: 16:9
header: 'DeepSeek-R1 · NLP Presentation'
footer: 'arXiv:2501.12948'
---

<!-- _class: title -->
<!-- _paginate: false -->

# DeepSeek-R1

### Incentivizing Reasoning Capability in LLMs via Reinforcement Learning

DeepSeek-AI (2025) · [arXiv:2501.12948](https://arxiv.org/abs/2501.12948)

Presented by **<your name>** · NLP Course

<!--
Speaker notes: one-line hook — "Can a model learn to reason without being shown
how? This paper says yes, with reinforcement learning alone."
-->

---

## Agenda

1. Motivation — reasoning, chain-of-thought, and the limits of SFT
2. Key idea & contributions
3. DeepSeek-R1-Zero — pure RL
4. DeepSeek-R1 — the multi-stage pipeline
5. Experiments & results
6. Distillation to smaller models
7. Limitations & open challenges
8. Conclusion & takeaways

---

<!-- _class: divider -->

# 1 · Motivation

---

## Why reasoning is hard

<!-- TODO: reasoning as the cornerstone of intelligence; CoT prompting;
why SFT on human traces is limiting (scalability, human bias, capped quality). -->

> TODO

---

<!-- _class: divider -->

# 2 · Key Idea & Contributions

---

## The core hypothesis

<!-- TODO: reasoning can be incentivized via pure RL, no SFT on reasoning traces.
List the paper's main contributions (R1-Zero, R1 pipeline, distillation). -->

> TODO

---

<!-- _class: divider -->

# 3 · DeepSeek-R1-Zero

---

## GRPO in one slide

<!-- TODO: Group Relative Policy Optimization — drops the critic, advantage from
group mean/std. Contrast with PPO (Fig. 3). Add the objective if useful. -->

> TODO

---

## Reward design

<!-- TODO: rule-based rewards only — accuracy + format. Why no neural reward
model (reward hacking). -->

> TODO

---

## Emergent behavior & the "aha moment"

<!-- TODO: AIME 15.6% → 77.9% (86.7% w/ self-consistency); response length grows;
the "aha moment" (Table 2). -->

> TODO

---

<!-- _class: divider -->

# 4 · DeepSeek-R1

---

## The multi-stage pipeline

<!-- TODO: cold-start long-CoT SFT → reasoning RL (+ language consistency) →
rejection sampling + SFT → final RL for helpfulness/harmlessness (Fig. 2). -->

> TODO

---

<!-- _class: divider -->

# 5 · Experiments & Results

---

## Headline results

<!-- TODO: Table 3 highlights — MMLU, AIME, MATH-500, Codeforces, GPQA.
Progression across Dev1 → Dev3. -->

> TODO

---

<!-- _class: divider -->

# 6 · Distillation

---

## Transferring reasoning to smaller models

<!-- TODO: distilled smaller models beat their instruction-tuned counterparts;
the accessibility argument. -->

> TODO

---

<!-- _class: divider -->

# 7 · Limitations & Open Challenges

---

## What R1 still can't do

<!-- TODO: structured output / tool use, token efficiency (overthinking),
language mixing, software-engineering tasks, prompt sensitivity, reward hacking. -->

> TODO

---

<!-- _class: divider -->

# 8 · Conclusion

---

## Takeaways

<!-- TODO: 3–4 crisp takeaways. End with the "pure RL unlocks reasoning" message
and what it means for future work. -->

> TODO

---

<!-- _class: title -->
<!-- _paginate: false -->

# Thank you

### Questions?

[arXiv:2501.12948](https://arxiv.org/abs/2501.12948) · [huggingface.co/deepseek-ai](https://huggingface.co/deepseek-ai)
