# Reddit — r/datascience

**Title:** I built a prediction market powered by an ML ensemble — forecasts world events from 100+ data streams with calibrated probabilities

**Body:**

Hey r/datascience,

I've been building GOD — a prediction market platform that uses an ML ensemble to forecast real-world events. Instead of crowd wisdom (like Polymarket), it monitors 100+ live data streams and produces calibrated probability forecasts.

**What makes it interesting from a DS perspective:**
- Multi-domain data fusion: news, financial markets, social signals, weather, seismic activity, satellite data, geopolitical events
- Causal inference to discover non-obvious connections across domains
- Ensemble forecasting with multiple model types
- Calibration: predictions are calibrated so confidence scores reflect actual likelihood
- Accuracy tracking: every prediction is scored against outcomes, and the system adapts

**The pipeline (high level):**
1. Stream processing — real-time ingestion, dedup, enrichment from 100+ sources
2. Event extraction — structured events from unstructured data
3. Knowledge graph — temporal graph of entities, events, and causal relationships
4. Correlation discovery — finding cause→effect chains across domains
5. Ensemble prediction — multiple models produce calibrated probabilities
6. Scoring — predictions tracked against outcomes, weights adapted

**What's live:**
- Landing page with early access: https://vishnu-MVP.github.io/god-landing/
- Open source (MIT)
- API access for developers ($99/mo Prophet tier)

I'd love feedback from this community:
1. How do you handle calibration in production systems?
2. What's your experience with causal inference at scale?
3. Would you use an API like this for your own forecasting work?

---
**Posting instructions:** Post to r/datascience. Frame as sharing a project for technical feedback. Engage with all comments.