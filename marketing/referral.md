# Referral Program Design

## Mechanism
In-app viral loop: users share a prediction → both referrer and referee get free Oracle tier months.

## Structure

### How it works:
1. Each user gets a unique referral link: `https://vishnu-MVP.github.io/god-landing/?ref=USER_CODE`
2. When someone signs up via a referral link, both the referrer and the new user get 1 free month of Oracle tier
3. After 3 successful referrals, the referrer gets 3 months free
4. After 10 successful referrals, the referrer gets Prophet tier free for 3 months

### Why this works for prediction markets:
- Prediction markets have a natural viral loop — users share their forecasts to prove they're right
- "GOD says there's a 78% chance X will happen — check it out" is a natural shareable moment
- The incentive (free Oracle months) aligns with the product — users want the advanced features

### Implementation:
- Add referral link generation to the landing page
- Track referrals via URL parameter (?ref=USER_CODE)
- Store referral data in localStorage (for now, until backend is available)
- Display referral count and earned rewards on a referral dashboard

### Landing page integration:
Add a referral section to the landing page with:
- "Share GOD, earn free Oracle months" headline
- Referral link generator (uses a hash of the user's email as their code)
- Share buttons for Twitter/X, Reddit, Discord, copy link
- Progress tracker showing referrals count and earned rewards

### Copy:
"Think GOD is cool? Share it.
For every friend who signs up, you both get a free month of Oracle tier.
Share 3 friends → 3 months free.
Share 10 friends → 3 months of Prophet tier (API access) free.

Your referral link: [GENERATED LINK]
[Share on Twitter] [Share on Reddit] [Copy Link]"