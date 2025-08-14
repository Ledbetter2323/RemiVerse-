# RemiVerse Technical Architecture (MVP)

## Canisters
1. **Identity & Access** — II linkage, roles (viewer/creator/admin), KYC flags.
2. **REMI Token/Ledger** — balances, transfers, staking hooks.
3. **Creator Registry** — channel metadata, payout splits, proof-of-rights refs.
4. **EPG/Metadata** — program guide, playout schedules, content policies.
5. **Payout Router** — settlement cycles, on-chain splits, vesting.
6. **Analytics & Events** — watch-time, impressions, tips; rollup summaries.

## Key Interfaces (sketch)
- `register_creator(principal, payout_split[])`
- `submit_asset(hash, license_uri, policy)`
- `report_event(session_id, type, value)`
- `settle(period_id)`

## Storage/Delivery
- Media in object storage (S3/GCS/R2). Hash anchored on-chain.
- HLS/DASH via CDN; signed URLs; optional DRM (Widevine/FairPlay) later.

## Ads
- Adapter service posts impression/click/complete events.
- On-chain rollup of verified events for revenue share.

## Security/Abuse
- Rate limiting, moderation queues, fingerprinting for re-uploads.
- Audit logs hashed and time-stamped.

## Diagrams
(Place sequence and component diagrams here.)