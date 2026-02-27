# Best-Parts Map

| Layer | Best LLM for This Layer | What to Extract (copy the key paragraph/section) |
|-------|------------------------|--------------------------------------------------|
| Layer 1: Data Foundation        |  Claude | Training-serving skew framing — clock skew, deduplication, late-arriving data causing silent model degradation            |
| Layer 2: Statistics & Analysis  |ChatGPT  | Point-in-time consistency: joins must recreate the exact feature state at the millisecond a historical request was made            |
| Layer 3: ML Models              | Gemini  | Only one to name MMoE (Multi-gate Mixture-of-Experts) — an actually documented Google architecture for multi-objective ranking            |
| Layer 4: LLM / Generative AI   |Claude    | Cold-start consequence of offline pre-computation: new videos lack semantic features immediately after upload            |
| Layer 5: Deployment & Infra     |   Claude| Actual millisecond breakdown per stage + org-structure insight: each team consumes latency budget without shared accountability            |
| Layer 6: System Design & Scale  |  Gemini | Scatter-gather fan-out pattern + Memcached for pre-computed homepage candidates — most architecturally precise            |
| Overall Analysis / Hardest Problem |Claude| Closed feedback loop framing: system converges toward narrow content, degrading long-term retention without deliberate intervention            |
| Writing Style / Structure       |  Claude |  Most consistent uncertainty flagging, named model families with training approach on every ML claim, zero filler          |
