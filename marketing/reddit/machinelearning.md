# Reddit — r/MachineLearning

**Title:** [Project] I built an ML ensemble that forecasts world events from 100+ live data streams — prediction markets powered by causal inference

**Body:**

Hey r/MachineLearning,

I've been working on GOD — a prediction market platform where an ML ensemble engine forecasts geopolitical, economic, and climate events. I wanted to share the approach and get feedback from this community.

**The problem:**
Traditional prediction markets (Polymarket, PredictIt) rely on crowd wisdom — market prices as probabilities. This works but has limitations: crowd bias, liquidity issues, and no explainability. I wanted to see if an autonomous ML system could do better.

**The approach:**
- Ingest 100+ live data streams across 6 event categories (news, markets, social, weather, seismic, geopolitical)
- Extract structured events using LLM-based semantic understanding
- Build a temporal knowledge graph connecting entities, events, and causal edges
- Use causal inference methods to discover non-obvious cause→effect chains
- Ensemble multiple model types to produce calibrated probability forecasts
- Score every prediction against actual outcomes and adapt

**Key design decisions:**
- Calibration over raw accuracy — predictions are calibrated so a "70% likely" event actually happens ~70% of the time
- Explainability — every prediction includes a reasoning trail, causal chain, and supporting evidence
- Self-improving — the system tracks its own accuracy and adjusts model weights based on historical performance

**What's live:**
- Landing page: https://vishnu-MVP.github.io/god-landing/
- Open source (MIT)
- API tier for developers/funds ($99/mo)

I'd really value feedback from this community on:
1. The calibration approach — what methods have you found effective?
2. Causal inference at scale — any recommendations for handling confounders across domains?
3. Ensemble design — how would you weight models that have different strengths (temporal patterns vs causal reasoning vs semantic understanding)?

Happy to go deeper on any aspect of the architecture.

---
**Posting instructions:** Post to r/MachineLearning. Use [Project] tag. This community values technical depth — be ready to discuss methodology in detail in comments. Best time: weekday morning US time.