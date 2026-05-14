# Membra Demo Data

Membra Demo Data is the seed scenario pack for showing MEMBRA as a live physical media network.

It contains demo owners, advertisers, campaigns, assets, media kits, QR scans, proof events, reward states, and reports that make the dashboard, API, admin console, KPI layer, and investor demo feel alive.

## One-line thesis

Demo data turns MEMBRA from abstract architecture into a clickable proof-of-placement story.

## Demo story

A local coffee brand funds a campaign.

Three owners register surfaces:

- a vehicle rear-window placement
- a wearable QR shirt placement
- a storefront window placement

Membra generates media kits, assigns QR identities, records proof events, tracks scans, and marks reward eligibility after review.

## Files

- `data/demo_bundle.json` — complete demo state bundle.
- `data/owners.json` — demo owners.
- `data/advertisers.json` — demo advertisers.
- `data/campaigns.json` — demo campaigns.
- `data/assets.json` — demo physical surfaces.
- `data/media_kits.json` — QR/NFC media kits.
- `data/proof_events.json` — install and receipt proof records.
- `data/tracking_events.json` — QR/NFC scan and tap events.
- `data/reward_states.json` — reward eligibility states.
- `scripts/load_demo_data.py` — loader for SQLite-style demo APIs.

## Integration targets

- `Membra_api`
- `Membra_ads`
- `membra-qr-gateway`
- `Membra_admin-`
- `Membra_kpi`
- `Membra_proofbook`

## Current stage

Demo seed package for dashboard, API, and investor walkthroughs.
