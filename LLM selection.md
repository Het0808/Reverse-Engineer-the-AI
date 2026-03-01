# LLM Selection Guide: Based on YouTube Recsys Comparison

**Primary Recommendation: Claude**  
- **Use When**: Frontier ML systems, causal inference, feedback loops, paper-deep teardowns.  
- **Why**: Highest fidelity to 2016-2026 research (interleaving A/B, RL policy gradients, counterfactual logging).  
- **Score**: 9.5/10 for accuracy/depth.

**Secondary: Gemini**  
- **Use When**: Production deployment, 2025/26 scaling (tail latency, LLM cold-start distillation).  
- **Why**: Practical engineer insights, timely updates.  
- **Score**: 8.5/10.

**Tertiary: ChatGPT**  
- **Use When**: Pedagogical intros, balanced overviews, non-experts.  
- **Why**: Clear structure, safe framing.  
- **Score**: 8/10.

## Decision Matrix
| Query Type              | Top Pick  | Rationale                              |
|-------------------------|-----------|----------------------------------------|
| **Recsys Architecture** | Claude   | RL + interleaving precision            |
| **MLOps/Infra**         | Gemini   | TPU funnels, P99 latency               |
| **Teaching/Overview**   | ChatGPT  | 6-layer scaffolding                    |
| **LLM Integration**     | Gemini   | Distillation for scale                 |
| **Scale Challenges**    | Claude   | Cross-surface + global shards          |

**Hybrid Tip**: Start with Claude for core, layer Gemini production scars. Avoid single-LLM dependency—cross-verify as done here.
**Updated Feb 2026**: Claude holds edge post-Gemini video recs talks.
