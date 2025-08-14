# RemiVerse

**Status:** Grant resubmission-ready • Updated August 14, 2025  
**Owner:** Ledbetter2323

RemiVerse is a Web3-native media ecosystem built on the Internet Computer Protocol (ICP). It combines free AVOD channels to acquire audience, live creator streaming, and tokenized revenue sharing so creators and backers are paid automatically.

## Core Modules

- **RemiWatch (AVOD)** — 24/7 themed free channels (licensed + public-domain + creator content). Traffic engine to the rest of the ecosystem.
- **RemiLive** — Creator live-streaming with on-chain payouts and programmable splits.
- **RemiRights / RemiVestment** — (Phase 2) Buy/sell fractional rights in viral videos with revenue sharing.
- **RemiBets** — (Phase 3) Optional sports/event betting integrations, region-gated.
- **REMI Token** — Native utility token for payouts, staking, ad-revenue shares, and incentives.

> **GMVerse is a separate project** (mobile sports management game). Optional future integrations (streams, tournaments, token rewards) remain decoupled by design.

## Why RemiVerse

- **Aligned incentives:** AVOD monetization with transparent on-chain splits to creators and channel partners.  
- **Distribution first:** Always-on free channels + basic live streaming to seed supply and demand before advanced rights trading.  
- **ICP fit:** Low-latency canisters, Internet Identity (II) login, and canister-based storage for metadata; integrates with media CDNs for video delivery.

## Business Model

1) **Advertising (AVOD):** Programmatic + direct. Tokenized revenue shares to creators/channels.  
2) **Tips/Microtransactions:** Viewers tip in REMI; creators receive instant splits.  
3) **Sponsorships & Branded Channels:** Flat-fee + rev-share.  
4) **(Phase 2) Rights Trading Fees:** % fee on RemiRights/RemiVestment transactions.  
5) **(Phase 3) Betting Affiliate/Take:** Where compliant and licensed.

## Technical Overview (MVP)

- **Identity:** Internet Identity (II).  
- **Wallet/Token:** REMI token canister; ledger integration for balances & payouts.  
- **Creator Registry:** Canister with channel metadata, payout addresses, KYC flags (off-chain provider).  
- **AVOD Catalog + EPG:** Canister stores EPG, content metadata, policy IDs, entitlements.  
- **Payments:** Programmable split contracts (canister methods) to route ad/tip revenue.  
- **Video Delivery:** Object storage + CDN (off-chain) with content hashes anchored on-chain; signed URL policy; DRM optional.  
- **Analytics:** Ingest events (impressions, watch time, tips) → summarized usage on-chain (rollups) for transparency.

## MVP (3–6 months)

- **P0:** RemiWatch (2–3 free channels), REMI wallet, creator onboarding, basic live streaming, revenue split payouts, analytics dashboard.  
- **P1:** Programmatic ads integration, creator tipping, basic moderation.  
- **P2:** Rights marketplace alpha.

## Compliance & Content

- AVOD catalog = licensed + public-domain + CC-BY content with proof-of-rights registry.  
- Geo & age gating for betting or sensitive content.  
- DMCA + notice-and-takedown workflow.

## Repo Map