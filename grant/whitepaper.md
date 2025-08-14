# RemiVerse Whitepaper (Grant Edition) — Updated August 14, 2025

## Abstract
RemiVerse is a Web3-native media platform on ICP. It uses AVOD channels to acquire audience, live streaming to grow creators, and on-chain revenue splits to pay contributors automatically. A native token (REMI) coordinates incentives and enables transparent reporting.

## Problem
Creators and small channels can't see or trust the monetization flow. Rights and rev-shares are opaque; payouts are slow; middlemen tax the system.

## Solution
- Transparent, programmable revenue splits on-chain.
- Free 24/7 channels to aggregate audience quickly.
- Simple live streaming to monetize immediately.
- Later: fractional rights trading when liquidity exists.

## Architecture (MVP)
- Internet Identity for auth.
- Canisters: Identity, Wallet/Token, Creator Registry, EPG/Metadata, Payout Router, Analytics.
- Storage & Delivery: off-chain object storage and CDN, content hashes anchored on-chain.
- Ads: programmatic adapters; event ingestion; settlement rollups on-chain.

## Token (REMI)
Utility for payouts, tipping, staking creator channels, and rewarding watch-time engagement. Tokenomics designed so founder allocation is **locked** (5–10%) with on-chain vesting to avoid negotiation drift during future acquisition discussions.

## Roadmap
- P0 (Months 1–2): AVOD (2–3 channels), wallet, creator onboarding, payouts, dashboard.
- P1 (Months 3–4): Ad adapters, tipping, moderation, KYC hooks.
- P2 (Months 5–6): Rights marketplace alpha.

## Compliance
- Content proofs-of-rights; DMCA; regional gating.
- Betting features are modular and jurisdiction-gated; excluded from MVP.

## Go-To-Market
- Seed with themed channels using licensed + public-domain libraries.
- Recruit 25–50 pilot creators; tip matching funded from grant.
- Partnerships with small OTT networks for overflow inventory.

## Budget & Use of Proceeds (MVP)
- Engineering (2–3 devs): Core canisters, dashboard, wallets.
- Licensing/Legal: initial catalog rights + counsel.
- Infra: storage/CDN credits, monitoring.
- Creator fund: tip matching to catalyze usage.

## Risks & Mitigations
- **Licensing:** start with public-domain + CC + low-cost libraries; rights registry on-chain.
- **Latency:** use CDN edges; keep canister interactions lightweight during playback.
- **Ad Fill:** start with one adapter; add direct deals; default to house ads initially.