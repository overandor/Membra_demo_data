# Membra Demo Data

**Membra Demo Data is the seed scenario pack for MEMBRA Labs and the MEMBRA Proof Network.**

It makes the company demo feel alive by supplying sample owners, advertisers, campaigns, assets, media kits, QR/NFC scan events, proof events, reward states, and reports.

## Company Context

- Company: **MEMBRA Labs**
- Flagship product: **MEMBRA Proof Network**
- Module: **Membra Demo Data**
- Category: seed scenarios, demo data bundle, dashboard walkthrough data, investor demo support

## One-Line Thesis

Demo data turns MEMBRA from abstract architecture into a clickable proof-of-placement story.

## Product Role

This repo should support demos for:

- `Membra_ads`
- `membra-qr-gateway`
- `Membra_admin-`
- `Membra_kpi`
- `Membra_proofbook`
- `Membra_wallet`
- `Membra_mobile`
- `Membra_investor_room-`

## Canonical Demo Story

A local coffee brand funds a physical media campaign.

Three owners register surfaces:

- vehicle rear-window placement
- wearable QR shirt placement
- storefront window placement

MEMBRA generates media kits, assigns QR/NFC identities, records receipt and install proof, tracks scans/taps, reviews proof, and marks reward eligibility after review.

## Suggested Files

```text
data/
  demo_bundle.json
  owners.json
  advertisers.json
  campaigns.json
  assets.json
  media_kits.json
  proof_events.json
  tracking_events.json
  reward_states.json
  reports.json
scripts/
  load_demo_data.py
  reset_demo_data.py
  export_demo_bundle.py
```

## Required Demo Entities

Owners:

- vehicle owner
- wearable campaign participant
- storefront/window owner

Advertiser:

- local coffee brand

Campaign:

- QR/NFC proof media campaign

Assets:

- vehicle rear window
- campaign shirt
- storefront window

Media kits:

- QR sticker
- wearable QR print
- window decal

Proof events:

- kit receipt confirmed
- installation photo submitted
- proof approved
- proof disputed example

Tracking events:

- QR scan
- NFC tap
- redirect click
- repeat scan

Reward states:

- pending
- eligible
- held
- released
- failed example

## Integration Targets

| Repo | Demo Data Usage |
|---|---|
| `overandor/Membra_ads` | seed owners, advertisers, campaigns, assets, kits, proof, scans |
| `overandor/membra-qr-gateway` | render dashboard cards, scan charts, proof timelines |
| `overandor/Membra_admin-` | populate proof review and claims queues |
| `overandor/Membra_kpi` | generate KPI reports and exports |
| `overandor/Membra_proofbook` | generate canonical proof hashes and audit records |
| `overandor/Membra_wallet` | demonstrate reward eligibility and payout states |
| `overandor/Membra_investor_room-` | support buyer demo script and screenshots |

## Demo Data Rules

- mark all demo records as demo records
- no real personal data
- no real private addresses
- no private keys
- no real payment credentials
- no unsupported revenue claims
- no fabricated customer traction presented as real

## Productization Priority

This repo is a high-leverage resale upgrade because a buyer-facing demo needs believable data.

Next steps:

1. create canonical `demo_bundle.json`
2. create seed data split by resource type
3. write SQLite loader for `Membra_ads`
4. write dashboard mock data adapter for `membra-qr-gateway`
5. create sample KPI export files
6. create screenshot-ready demo script

## Current Stage

Demo seed package and scenario charter. Some demo files may exist, but the next company-grade step is a complete canonical bundle plus loaders for the backend and dashboard.