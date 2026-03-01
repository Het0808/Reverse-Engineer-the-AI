# YouTube Recommendations: Final 6-Layer Teardown (2026)

**Claude's hybrid best-of: Precision from research + scale insights from Gemini/ChatGPT.**

**Layer 1 — Data Foundation**  
✅ Ingests position-aware signals (skips, context, watch %). Counterfactual logging debias via Pub/Sub → Bigtable/Dataflow ETL.  
🛠 Bigtable, Beam, Feature Store. Challenge: Label freshness vs. spam. [web:11]  
🎯 Rebuild first: Counterfactual logs.

**Layer 2 — Statistics & Analysis**  
✅ Interleaving A/B + counterfactuals track watch time vs. satisfaction.  
🛠 Gondola/Vizier, importance sampling. Challenge: Metric conflicts. [web:20]  
🎯 Causal inference mastery.

**Layer 3 — Machine Learning Models (CORE)**  
✅ Two-tower retrieval (sampled softmax → ~500 candidates via ScaNN) + multi-task ranking (RL policy gradient).  
🛠 TensorFlow, REINFORCE, MMoE. Challenge: Feedback degeneration. [web:25][web:28]  
🎯 Bleeding edge: RL at 2B users.

**Layer 4 — LLM / Generative AI**  
✅ Gemini-distilled semantic IDs for cold-start + multimodal embeddings.  
🛠 Vertex AI, ViT/CLIP. Challenge: Embedding alignment. [web:13][web:18]  
🎯 Secondary but growing.

**Layer 5 — Deployment & Infrastructure**  
✅ <100ms TPU funnel (tiered features, tail latency fallbacks). Shadow deploys + policy gates.  
🛠 TPU v5, TF Serving, Borg/K8s. Challenge: P99 latency. [web:14]  
🎯 MLOps at planetary QPS.

**Layer 6 — System Design & Scale**  
✅ Sharded ScaNN + cross-surface embeddings (Shorts ≠ Homepage). Global CDN/Spanner.  
🛠 Colossus, regional shards. Challenge: Consistency vs. locality. [web:26]  
🎯 Few systems match this physics.

**Overall**  
⭐ Critical: Layer 3 (RL feedback fix). 🔥 Hardest: Degenerate loops. 🏗 First: Logging infra.  
**Complexity: Bleeding Edge** [web:22]
