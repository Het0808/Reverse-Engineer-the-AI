# Best Parts Map: YouTube Recsys Teardown Extraction (2026)

**Hybrid synthesis from comparison. Claude = 60% weight; Gemini = 25%; ChatGPT = 15%.**

## Layer-by-Layer Best Elements

### Layer 1 — Data Foundation
| Source   | Best Part                                      | Why Best                          |
|----------|------------------------------------------------|-----------------------------------|
| **Claude** | Counterfactual logging (position/skips bias)  | Fixes selection bias at source [web:11] |
| **ChatGPT** | ETL freshness (petabytes/day pipeline)       | Rebuild priority #1              |
| **Gemini** | Fixed-size vector from variable history      | NN-ready feature engineering     |

**Winner**: Claude's logging infra.

### Layer 2 — Statistics & Analysis
| Source   | Best Part                                      | Why Best                          |
|----------|------------------------------------------------|-----------------------------------|
| **Claude** | Interleaving A/B + importance sampling       | Unbiased ranking eval [web:20]   |
| **Gemini** | Clickbait correction (weighted regression)   | Practical bias fix               |
| **ChatGPT** | Bayesian multi-metric alignment              | Solid baseline                   |

**Winner**: Claude's interleaving (Google-specific).

### Layer 3 — Machine Learning Models (CORE)
| Source   | Best Part                                      | Why Best                          |
|----------|------------------------------------------------|-----------------------------------|
| **Claude** | Sampled softmax + RL policy gradient         | Handles feedback loops [web:25]  |
| **Gemini** | MMoE + extreme multiclass sampling           | Production ranking detail        |
| **ChatGPT** | Two-tower exploration/personalization balance| Clear conceptual framing         |

**Winner**: Claude's RL (hardest problem solved).

### Layer 4 — LLM / Generative AI
| Source   | Best Part                                      | Why Best                          |
|----------|------------------------------------------------|-----------------------------------|
| **Gemini** | Distilled LLMs for cold-start semantic IDs   | 2025/26 economically viable [web:18] |
| **Claude** | Gemini multimodal → content tower alignment  | Technical integration depth      |
| **ChatGPT** | Secondary role honesty check                 | Prevents overhyping              |

**Winner**: Gemini/Claude tie (practical + precise).

### Layer 5 — Deployment & Infrastructure
| Source   | Best Part                                      | Why Best                          |
|----------|------------------------------------------------|-----------------------------------|
| **Gemini** | Tail latency P99 + TPU funnel timeouts       | Real engineer pain point [web:14] |
| **Claude** | Tiered features (<100ms budget breakdown)    | Latency math verified            |
| **ChatGPT** | Shadow deployment monitoring                 | Standard but essential           |

**Winner**: Gemini's tail latency focus.

### Layer 6 — System Design & Scale
| Source   | Best Part                                      | Why Best                          |
|----------|------------------------------------------------|-----------------------------------|
| **Claude** | Cross-surface embedding sharing + ScaNN shards| Multi-feed complexity [web:26]   |
| **Gemini** | Global consistency vs. local latency (CAP)   | Distributed systems theory       |
| **ChatGPT** | Hierarchical ranking pipelines               | Scale visualization              |

**Winner**: Claude's surface separation.

## Overall Rankings Integration
