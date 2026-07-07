# Show HN Post

**Title:** Show HN: I built an ML oracle that predicts world events from 100+ live data streams

**Body:**

Hi HN,

I've been building GOD — a prediction market platform that doesn't rely on crowd wisdom. Instead, it continuously monitors 100+ live data streams (news, financial markets, social signals, weather, seismic activity, satellite data, and more) and uses an ML ensemble to forecast geopolitical, economic, and climate events with calibrated probabilities.

Every prediction comes with:
- A confidence score (calibrated, not just raw model output)
- A reasoning trail explaining *why* the prediction was made
- A causal chain showing the chain of events that led to the forecast
- Supporting evidence from the underlying data streams
- Accuracy tracking — every prediction is scored against outcomes over time

The idea: Polymarket uses crowd wisdom (market prices) to predict events. GOD uses an actual ML engine that does the research for you — watching the world 24/7, connecting dots across domains, and producing forecasts you can verify.

**What's live:**
- Landing page with early access waitlist: https://vishnu-MVP.github.io/god-landing/
- Prediction markets across Politics, Geopolitics, Economy, Crypto, Technology, and Climate
- Interactive globe view showing predictions geolocated worldwide
- Accuracy dashboard tracking model performance over time

**Tech stack:** React/TypeScript frontend, Python/FastAPI backend, graph database for the knowledge graph, vector search for semantic retrieval, and an LLM for event extraction.

The project is MIT licensed and open source.

I'd love feedback on:
1. The prediction market approach — does ML-driven forecasting interest you more than crowd wisdom?
2. The accuracy tracking — is Brier-style scoring enough, or would you want to see more calibration metrics?
3. The API tier — I'm planning a Prophet tier ($99/mo) with full API access for developers/funds. Would you use this?

Happy to answer any questions about the architecture, the ML approach, or the product direction.

---
**Posting instructions:** Post to https://news.ycombinator.com/submit with the title above. Best time: Tuesday-Thursday, 8-10am PT. Engage with every comment within the first 2 hours — this is critical for HN ranking.