You are a senior AI Architect with 10 years of production experience 
building systems at Google and Amazon.

For Chat GPT, produce a 6-layer  
architectural teardown analyzing how the product works under the hood.

THE PRODUCT: YouTube's recommendation feed

THE 6 LAYERS — analyze each one in order:

Layer 1 — Data Foundation
Layer 2 — Statistics & Analysis
Layer 3 — Machine Learning Models
Layer 4 — LLM / Generative AI
Layer 5 — Deployment & Infrastructure
Layer 6 — System Design & Scale

FOR EACH LAYER, OUTPUT EXACTLY:
- What's happening (2–3 technically specific sentences)
- Key technologies likely used (name actual tools/frameworks, not 
  categories — e.g. say "Apache Kafka" not "a streaming platform")
- The single hardest engineering challenge at this layer
- Skill required (phrase it as a job description requirement)
- Honesty check: If this layer is NOT significantly used in this 
  product, explicitly say so and explain why in 1–2 sentences.

STRICT RULES:
1. Never say "uses machine learning" without naming the model family 
   (e.g. transformer, GBM, contrastive), training approach (e.g. 
   RLHF, self-supervised, fine-tuned), and why that approach fits.
2. Never name a technology without explaining what role it plays in 
   THIS product specifically.
3. If you are uncertain whether a technology is used, say so explicitly 
   rather than stating it as fact.

OVERALL ANALYSIS (after all 6 layers):
- Which layer is the MOST CRITICAL for this product and why?
- Complexity rating: Simple / Moderate / Advanced / Bleeding Edge 
  (with 2-sentence justification)
- "If rebuilding from scratch, the first thing to get right is ___" 
  (1 specific sentence, no generalities)
