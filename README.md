# FlowMark — streaming proof, formed through HACD

> Bitcoin proved PoW for money. **HACD brings PoW to assets.** FlowMark anchors every money-streaming commitment to a PoW-mined HACD formation record — so an external party (employer, auditor, revenue-share partner) can verify a stream started *without trusting the streaming platform*.

**Live demo:** https://yusizer.github.io/flowmark/

**Bounty:** B8 «Build on HACD» on [Wizz](https://wizzhq.xyz/bounties/build_on_hacd_), sponsored by GrowStreams.
**Ticker:** FLOW · **Category:** utility · **Accent:** `#6FB3AB`

---

## The formation moment (under one minute)

1. A user enters a stream (recipient, token, rate per second) on the **Anchor** page.
2. Clicks **Anchor to HACD** → a HACD Stack record is formed: a unique 6-letter HACD name, a formation timestamp, a content hash, and the stream reference.
3. A **StreamMark receipt** appears instantly. The user copies the public proof link.
4. Opens it in a fresh tab (the reviewer's point of view) → the **same unfakeable formation time, content hash and stream reference** render for anyone, not just the sender.

That non-repudiable formation time is the entire product. A streaming dashboard can render a "stream started" row, but the operator can edit, backdate, or reconfigure it — so it proves nothing to someone outside the platform. A HACD formation record is **mined and Stacked**: its formation time cannot be backdated and the receipt cannot be silently altered. Without HACD, FlowMark is just another streaming dashboard.

## Pages

- **Anchor** — start a stream + single "Anchor to HACD" action.
- **Receipts** — the user's StreamMark receipts, each with its HACD name and formation time.
- **Proof (public)** — the canonical receipt a reviewer opens: HACD name, formation timestamp, content hash, stream reference, copyable proof link.

The app is a single self-contained `index.html` (hash router + `localStorage`), so it runs anywhere static hosting is available.

## HACD Stack Asset design (FLOW)

| Field | Value |
|---|---|
| Asset type | **HYBRID** (FT FLOW balance + NFT HACD name as StreamMark receipt ID) |
| Total HACD lots | 256 |
| Units per HACD lot | 10,000 |
| Total supply | 2,560,000 FLOW |
| Stack cost | 50 HAC per HACD lot |
| Formation cost reference | 12,800 HAC + network fees |
| Phase model | `designated_first` — 32 designated lots + 224 public |
| Per participant | min 1 / max 10 HACD |
| Removal effect | `burn` (receipt annulled; formation history permanent) |

Full validated spec: [`issuance/launch_spec.json`](issuance/launch_spec.json) — passes `validate_launch_spec.py` with 0 ERRORs (2 expected draft warnings; `--strict` pending issuer + HACD Labs sign-off).

## Why this is honest

- The demo **mocks** the Hacash mainnet Stack step and labels it **"formation: mocked for demo"** in the UI. Real Vara stream creation, wallet signing, and mainnet Stack are explicitly out of scope for the sprint.
- FLOW is a **utility Stack Asset, not an investment product**. No price, liquidity, listing, or return is guaranteed. Formation cost is non-refundable. Not financial advice.
- Future utility (GrowStreams auto-anchoring, revenue-share distributions, receipt marketplace) is **planned only** and is not promised in public copy.
- HACD is a **PoW-native asset container**, HAC pays the stack cost, Stack is the **formation action**. HACD is never called "just an NFT"; stack cost never "guarantees a price".

## Issuance package (`issuance/`)

Generated with the [HACD Incubator AI Issuance Skill](https://github.com/Satyam-10124/hacd-incubator-ai-issuance-skill):

- `issuer_intake_form.md` · `incubator_fit_review.md` · `project_profile.md` · `stack_design.md`
- `launch_spec.json` (validator: `OK: launch spec passed validation`)
- `launchpad_copy.md` · `issuer_faq.md` · `x_announcement.md` · `review_checklist.md`
- `validator_output.txt`

## Submission

Built for **B8 «Build on HACD»** (Wizz, sponsored by GrowStreams). Submit target: hacd.it/incubator Google Form + Wizz «Submit Your Entry». Quest: growstreams.xyz/app/projects/HACD (Vara / SubWallet) — to be completed before final submission.

---

*Draft structure pending HACD Labs review. Final Launchpad parameters must be confirmed by the issuer and HACD Labs before publication.*
