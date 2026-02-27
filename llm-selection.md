# LLM Selection Decision

| Decision Factor                 | My Choice | Reason (1 sentence) |
|---------------------------------|-----------|---------------------|
| Which LLM followed my prompt structure most faithfully? |Claude| Enforced every strict rule consistently — uncertainty flags, model family + training approach on every ML claim, no category-level technology names|
| Which LLM was most technically accurate (least hallucination)? |ChatGPT | Most conservative with claims, explicitly flagged uncertainty rather than stating unconfirmed tools as fact|
| Which LLM's output was most readable and well-organized? |ChatGPT | Cleanest prose flow and strongest narrative structure, easiest to read top to bottom|
| Which LLM handled the "honesty check" best (admitting when a layer doesn't apply)? | Claude| Only response that explained why a layer doesn't apply and gave the downstream consequence (e.g., cold-start impact)|

**Selected LLM for final tool:** Claude
**Why:**It most faithfully enforced the prompt's strict rules while producing the deepest layer-level insights,
particularly on failure modes and tradeoffs.
The one gap — Gemini's MMoE catch — is a single factual addition, not a structural advantage.
