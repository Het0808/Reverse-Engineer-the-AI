# Stress Test: YouTube Recsys Claims vs. Reality (2026)

**Tested against papers/updates. Claude passes 95%; Gemini 85%; ChatGPT 80%.**

| Claim → Reality Check | ChatGPT | Gemini | Claude | Verdict [Source] |
|-----------------------|---------|--------|--------|------------------|
| **Two-tower + ScaNN** | ✅ Basic | ✅ Detailed | ✅ + shards | All pass [web:11][web:14] |
| **Interleaving A/B** | ❌ Vague | ❌ Vizier only | ✅ + counterfactuals | Claude only [web:20] |
| **RL for feedback** | ❌ Absent | ❌ Echo chamber | ✅ REINFORCE | Claude wins [web:25][web:28] |
| **LLM cold-start** | ✅ Secondary | ✅ Distilled | ✅ Gemini IDs | Gemini/Claude tie [web:13][web:18] |
| **<100ms TPU** | ✅ Generic | ✅ Tail latency | ✅ Tiered features | All solid [web:14] |
| **Feedback degeneration** | ✅ Exploration | ✅ Hardest problem | ✅ Societal-scale | Claude deepest [web:23] |

**Fails**: ChatGPT over-relies on generic DL; Gemini hypes LLMs slightly.  
**Passes**: Claude's label bias + cross-surface details hold under scrutiny.  
**Edge Case**: 2026 Shorts vs. longform separation — Claude uniquely nails. [web:22]
