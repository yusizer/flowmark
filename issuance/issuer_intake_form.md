# HACD Incubator Cohort 2 — Issuer Intake Form

## 1. Project basics

- Project name: FlowMark
- Ticker / asset symbol: FLOW
- Category: utility
- One-sentence description: FlowMark anchors money-streaming commitments to HACD Stack formation records — immutable, PoW-backed proof that a payment stream started.
- Founder / team: Yusif (issuer, X @Yusifab7) — identity to be confirmed to HACD Labs privately
- Website: https://yusizer.github.io/flowmark/ (live GitHub Pages demo)
- X / community links: @Yusifab7
- Contact: yusifabdullayev48@gmail.com

## 2. Why HACD

- Why should this asset be issued on HACD instead of a normal token contract? A "stream started" claim is only as credible as the record behind it. A normal contract or database timestamp can be edited, backdated, or reconfigured by the operator. HACD formation is mined and Stacked, so its formation time cannot be backdated and the receipt cannot be silently altered. That non-repudiable formation time is the entire product.
- What does PoW-backed formation add to this project? It makes every StreamMark receipt costly-to-fake and neutrally verifiable. A receipt anchored to a PoW-mined HACD carries real formation energy, not a platform-rendered row. External parties (employers, auditors, revenue-share partners) can verify proof without trusting the streaming platform.
- Why does the asset need HACD containers? Each StreamMark receipt identity is tied to one unique 6-letter HACD name. The finite 16-letter name space makes receipt IDs scarce and non-duplicable. The HACD container is the durable anchor that links a stream to a formation moment.
- What should users remember after seeing this launch? FlowMark receipts are formed, not logged. Each receipt exists because a real HACD was committed and a real HAC cost was paid — and that formation is permanent on-chain.

## 3. Asset design

- Asset type: HYBRID (FT FLOW balance + NFT HACD-name as StreamMark receipt ID)
- Total supply: 2,560,000 FLOW
- Number of HACD lots: 256
- Units per HACD lot: 10,000
- Are all lots equal? Yes, all 256 lots are identical. No tiers.
- Does removing the stack burn / disable / unlock anything? Removing the stack burns the 10,000 FLOW tied to that HACD lot and retires that HACD name as a StreamMark receipt ID.

## 4. Stack cost

- Proposed stack cost per HACD in HAC: 50 HAC
- Who receives or controls the stack cost? Stack cost goes to the Hacash network protocol as required by the Stack mechanism.
- Is any HAC burned, locked, paid, or reserved? HAC is paid as the formation cost per the Stack protocol. No additional locking or reservation by the issuer.
- Estimated network fee: standard Hacash network transaction fee per lot

## 5. Launch rules

- Launch date target: 2026-07-01
- Public sale / allowlist / designated address / phased launch: designated_first — first 32 lots Stacked by issuer/designated address, then 224 lots public
- Minimum HACD per participant: 1
- Maximum HACD per participant: 10
- Is there a first phase reserved for issuer or designated address? Yes — first 32 lots reserved as genesis StreamMark receipts, designated address 15j5fHZzL8Qkzi7YBtChf2GDfM6RJvUht7
- When does public participation begin? After the 32 genesis lots are formed by the designated address

## 6. Utility

- What can holders do at launch? Anchor a money-streaming commitment (stream ID, recipient, token, rate) to a HACD formation record and receive a StreamMark receipt with a public proof page showing the HACD name, formation timestamp, and stream reference.
- What may holders do later? Auto-anchor GrowStreams streams, participate in FLOW revenue-share distributions, list receipts on a receipt marketplace (all planned).
- What is already built? Stack formation logic, this issuance spec, and a demo app exposing the formation moment (start stream → anchor → receipt → public proof).
- What depends on future development? GrowStreams API auto-anchoring, revenue-share distribution contract, receipt marketplace.
- What should not be promised publicly? Price appreciation, liquidity, listing on exchanges, yield, or any financial return.

## 7. Community and communication

- Target audience: streaming-protocol users (GrowStreams/Vara), freelancers and bounty platforms needing payment proof, revenue-share and payroll operators, HACD collectors.
- Main narrative: Streaming proof formed through PoW. Not a dashboard claim — a HACD-anchored receipt.
- Tone: serious / technical / educational
- Key announcement message: FlowMark is a money-streaming receipt asset formed through HACD Stack, built for the GrowStreams ecosystem (HACD Incubator Cohort 2 sprint).
- Three things you want users to understand:
  1. FLOW supply is hard-capped at 2,560,000 units across 256 HACD lots.
  2. Each lot requires 1 HACD and 50 HAC formation cost and forms one StreamMark receipt ID.
  3. This is a utility asset for payment proof, not an investment product.

## 8. Risk disclosure

- Main risks users should understand: HACD and HAC market volatility, no guaranteed liquidity, future utility depends on development, formation cost is non-refundable, GrowStreams integration is planned and not guaranteed.
- Dependencies: Hacash network availability, HACD Launchpad operation, GrowStreams protocol and Vara network for the streaming side.
- Legal or regulatory sensitivities: Not a security. No profit promise. No redemption guarantee. No claim that stack cost sets a price.
- Anything HACD Labs should avoid saying: Do not say FLOW has a price floor. Do not describe stack cost as backing. Do not promise GrowStreams auto-anchoring as a launched feature.

## 9. Issuer confirmation

- I confirm that the information above is accurate to the best of my knowledge.
- I understand that HACD Labs review does not guarantee approval, listing, price, liquidity, or investment outcome.
