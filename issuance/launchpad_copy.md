# FlowMark on HACD

## Hero

**Streaming proof, formed through HACD.**

FlowMark issues FLOW — a hybrid Stack Asset that anchors money-streaming commitments to PoW-backed formation records no platform can rewrite.

## What is FlowMark?

FlowMark is a utility asset issued through the HACD Stack protocol that turns "a stream started" into a verifiable, on-chain fact. Unlike a streaming dashboard whose status row the operator can reconfigure, every StreamMark receipt is formed through a real HACD container and a real HAC formation cost. The result is a receipt with a traceable, permanent on-chain origin that an external party can verify without trusting the streaming platform.

There are exactly 256 Stack lots. Each lot uses 1 HACD and 50 HAC to form 10,000 FLOW and register one unique HACD name as a StreamMark receipt ID. Once all 256 lots are filled, no more FLOW can ever be created.

## Why HACD?

A money-streaming platform can show "stream started" on its own dashboard. But a dashboard claim shown to an external party — an employer, an auditor, a revenue-share partner — is just a row the platform renders. It can be edited, backdated, or reconfigured. It proves nothing to someone outside the platform.

FlowMark is different.

- Each StreamMark receipt exists because a PoW-mined HACD was committed as its anchor.
- Each receipt's formation time is mined and cannot be backdated.
- Each receipt ID is a unique 6-letter HACD name from a finite 16-letter name space — scarce and non-duplicable.
- The formation history is permanent and visible on the Hacash explorer, so a verifier who was not the sender can confirm the proof independently.

Bitcoin proved PoW for money. HACD brings PoW to assets. FlowMark brings PoW to streaming proof.

## How Stack works

1. You bring 1–10 HACD units.
2. You bring enough HAC: (number of HACD) × 50 HAC + a small network fee.
3. You confirm a Stack transaction on the Launchpad.
4. Your HACD containers form FLOW and register their names as StreamMark receipt IDs. You receive 10,000 FLOW per HACD lot.
5. You anchor a money-streaming commitment (stream ID, recipient, token, rate) to a receipt ID and receive a public proof page.
6. Your formation is recorded on-chain permanently.

Your HACD is not consumed — it is used as the formation container. If you later remove the Stack, the HACD is released but the FLOW for that lot is burned and the receipt ID is retired.

## Formation rules

- Total HACD lots: 256
- Units per lot: 10,000 FLOW
- Stack cost: 50 HAC per HACD
- Total supply cap: 2,560,000 FLOW (hard cap, no exceptions)
- Minimum per participant: 1 HACD
- Maximum per participant: 10 HACD
- Phase model: designated_first — first 32 lots Stacked by the issuer as genesis StreamMark receipts, then 224 lots public
- All lots are equal — no tiers

## Launch details

- Target date: 2026-07-01
- Platform: HACD Launchpad
- Phase: designated_first (32 genesis lots, then 224 public lots)
- Status: draft (pending HACD Labs review)

## Utility

At launch, FLOW holders can anchor a money-streaming commitment to a HACD formation record and receive a StreamMark receipt with a public proof page showing the HACD name, formation timestamp, and stream reference. Anyone with the proof link can verify the receipt without trusting the streaming platform.

Planned future utility (not guaranteed, depends on development):
- Auto-anchoring of GrowStreams streams to HACD receipts
- FLOW-based revenue-share distributions
- A receipt marketplace for StreamMark receipts

These features depend on future development and are not available at launch.

## FAQ

**Do I need HACD to participate?**
Yes. Each Stack lot requires 1 HACD. You must hold HACD before you can form FLOW.

**Do I need HAC?**
Yes. Each HACD lot requires 50 HAC as the formation cost plus a small network fee.

**How many FLOW do I get per HACD?**
10,000 FLOW per HACD lot, plus one StreamMark receipt ID from the HACD name.

**What is a StreamMark receipt ID?**
The unique 6-letter HACD name tied to your lot. It is the non-fungible identity of one stream-anchor receipt, separate from your fungible FLOW balance.

**Can I participate with more than 10 HACD?**
No. The maximum per participant is 10 HACD lots.

**What happens if I remove my Stack?**
Removing a Stack releases your HACD but permanently burns the 10,000 FLOW tied to that lot and retires the StreamMark receipt ID. The HAC formation cost is not refunded.

**Is FLOW an investment?**
No. FLOW is a utility Stack Asset for streaming proof. No price, return, or liquidity is guaranteed.

## Risk disclosure

FLOW is a utility Stack Asset issued through the HACD Stack protocol. It is not an investment product. No price appreciation, liquidity, listing on exchanges, or financial return is guaranteed.

Future utility features (GrowStreams auto-anchoring, revenue-share distributions, receipt marketplace) depend on development that has not yet been completed. They should not be treated as committed product features.

Formation cost (HAC) is non-refundable. HACD and HAC values fluctuate with market conditions. The streaming side of FlowMark depends on external protocols (GrowStreams, Vara) that are outside Hacash. Participation requires understanding the Hacash network, HACD Stack mechanics, and the streaming protocol you anchor.

This Launchpad page describes a draft issuance structure. Final parameters must be confirmed by the issuer and reviewed by HACD Labs before publication.

Not financial advice. Not legal advice.
