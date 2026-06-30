# Project Profile: FlowMark

## One-liner

FlowMark anchors money-streaming commitments to HACD Stack formation records, giving every payment stream an immutable, PoW-backed proof that it started.

## Category

Utility

## Problem

Money-streaming platforms can show a "stream started" status on a dashboard, but that record is a platform-rendered row the operator can reconfigure. When an external party — an employer verifying payment, an auditor checking revenue share, a bounty platform confirming payout — needs proof a stream actually began, a dashboard claim proves nothing. FlowMark uses HACD to make stream-start proof neutral, non-repudiable, and costly-to-fake.

## Asset concept

FLOW is a hybrid asset (FT + NFT) issued across 256 HACD lots. Each lot forms exactly 10,000 FLOW and registers the unique 6-letter HACD name as one StreamMark receipt ID. Total supply is fixed at 2,560,000 FLOW. Supply cannot increase because no additional HACD lots are available beyond the 256 defined at launch. Removing a Stack burns the FLOW tied to that lot and retires the receipt ID, permanently reducing supply.

## Why HACD

- HACD provides a PoW container whose formation time cannot be backdated — the exact property a "stream started" proof requires.
- Stack cost (50 HAC per HACD) creates a visible formation cost reference that a plain token contract or log entry cannot provide.
- The finite 16-letter HACD name space makes each StreamMark receipt ID unique and non-duplicable.
- Formation history is on-chain and permanent, so an external verifier can confirm a receipt without trusting the streaming platform.

## Target users

- Streaming-protocol users (GrowStreams / Vara) who want verifiable stream-start proof.
- Freelancers and bounty platforms that need payment-proof to resolve disputes.
- Revenue-share and payroll operators who need auditable stream commitments.
- HACD collectors who want to put their HACD units to productive use as receipt anchors.

## Launch readiness

- Issuance structure: defined (HYBRID, 256 lots, 10,000 FLOW per lot)
- Stack cost: defined (50 HAC / HACD)
- Supply: defined (2,560,000 FLOW across 256 lots)
- Launch utility: defined (anchor stream → StreamMark receipt → public proof page)
- GrowStreams auto-anchoring, revenue-share, receipt marketplace: planned, not built
- Launchpad listing: pending HACD Labs review
- Legal review: required before publication
