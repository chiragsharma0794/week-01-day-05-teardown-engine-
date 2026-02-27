## Reflection Questions

---

**1. Which of the 6 layers surprised you most in terms of complexity?**

**Layer 6 — System Design & Scale** was the most surprising — specifically the **payment-booking atomicity problem** in IRCTC and the **cross-surface interference problem** in YouTube. Most people assume scale complexity means "handle more requests," but the real surprise is that the hardest problems aren't throughput problems at all — they're **consistency problems across systems you don't fully control**. For IRCTC, the PRS backend is owned by CRIS, not IRCTC, meaning no shared transaction coordinator exists between a UPI payment confirmation and a seat booking — reconciliation is purely eventual. For YouTube, optimizing one surface (homepage) can silently cannibalize another (Up Next) in ways that only appear in system-level holdback experiments months later, not in any individual A/B test.

---

**2. What was the single biggest difference between the LLMs?**

The sharpest difference wasn't accuracy or writing quality — it was **epistemic behavior under uncertainty**. ChatGPT and Gemini both stated unconfirmed technologies as facts without flagging them (Gemini confidently named MMoE and TPUs as if confirmed; ChatGPT stated Pub/Sub and Memcached without hedging). Claude consistently separated "confirmed via published research" from "likely but unconfirmed" within the same sentence. The practical consequence is significant: if you're a junior engineer reading Gemini's output, you might cite MMoE as a confirmed YouTube architecture in a design doc — it's probably correct, but it's sourced from a Google research paper on recommendation systems generally, not a YouTube-specific disclosure. Only Claude's output trained the reader to distinguish between those two levels of confidence, which is the difference between a useful technical reference and a plausible-sounding hallucination risk.
