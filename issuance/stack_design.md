# Stack Design: FlowMark

## Asset type

Hybrid FT + NFT

- **FT:** FLOW (fungible receipt-pool balance)
- **NFT:** HACD name as StreamMark receipt ID (unique per lot)

## Supply

- Total supply: 2,560,000 FLOW
- HACD lots: 256
- Units per HACD: 10,000 FLOW
- StreamMark receipt IDs: up to 256 (one unique HACD name per lot)
- All lots are equal: Yes

Supply formula check:

```
total_supply = total_hacd_lots × units_per_hacd_lot
2,560,000 = 256 × 10,000 ✓
```

Phase-lot sum check:

```
first_phase_hacd_lots + public_phase_hacd_lots = total_hacd_lots
32 + 224 = 256 ✓
```

## Stack cost

- Cost per HACD: 50 HAC
- Estimated total formation cost reference: 12,800 HAC (256 × 50 HAC)
- Network fee: standard Hacash transaction fee per lot (paid by participant)
- Formation cost reference is an on-chain cost input, not a guaranteed price floor.

Per-lot formation inputs: 1 HACD + 50 HAC + network fee (formation cost reference — not a price floor and not backing).

## Formation rules

1. Each participant must hold at least 1 HACD and enough HAC to cover 50 HAC stack cost plus network fee.
2. Each participant may Stack between 1 and 10 HACD lots per the launch rules.
3. Each Stack transaction on 1 HACD lot produces exactly 10,000 FLOW and registers that HACD name as one StreamMark receipt ID.
4. The first 32 lots are reserved for the issuer / designated address (genesis StreamMark receipts). The remaining 224 lots are public. All 256 lots follow identical per-lot rules.
5. Once all 256 lots are Stacked, no more FLOW can be formed and no more StreamMark receipt IDs can be created. Supply is permanently fixed.

## Participant flow

1. Prepare 1–10 HACD units. (Their names will become your StreamMark receipt IDs.)
2. Prepare enough HAC: (number of HACD) × 50 HAC + estimated network fee.
3. Go to the HACD Launchpad and find FlowMark (FLOW).
4. Enter your HACD name(s) and confirm the Stack transaction. (Up to 200 HACD names can be entered per Launchpad transaction.)
5. Verify your formed FLOW balance and registered StreamMark receipt ID(s) on the Launchpad or Hacash explorer.
6. Anchor a money-streaming commitment to a receipt ID and share the public proof page with any external verifier.

## Removal / burn logic

If a participant removes the Stack from a HACD lot, the 10,000 FLOW tied to that lot are burned and that HACD name is retired as a StreamMark receipt ID. The HACD is released back to the holder's free HACD. Stack cost HAC is not refunded. This mechanism keeps HACD containers, StreamMark receipt IDs, and FLOW supply linked as long as the Stack is active.

## Hybrid clarification

- The **FLOW balance** is fungible — 10,000 FLOW from lot A is identical to 10,000 FLOW from lot B.
- The **StreamMark receipt ID** is the unique HACD name and is not fungible — it identifies which HACD anchored which stream.
- Both are produced by the same single Stack action; participants do not pay or transact twice.

---

*Draft design. Issuer confirmation required on stack cost, supply, designated address, and transferability of the StreamMark receipt ID. Not financial advice. Final Launchpad parameters must be verified by HACD Labs.*
