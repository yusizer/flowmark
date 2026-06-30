# Incubator Fit Review: FlowMark

## Verdict

Strong fit

## Why it fits HACD

- The product's core value is a non-repudiable "stream started" proof. A plain token contract or database timestamp can be edited or backdated by the operator; a HACD formation time is mined and cannot be backdated. HACD is load-bearing here, not decorative.
- Receipt identity maps naturally to HACD's per-unit name model: one unique 6-letter HACD name = one StreamMark receipt ID. The finite 16-letter name space makes receipt IDs scarce and non-duplicable, which a generic contract cannot replicate.
- Formation cost in HAC creates a real, visible cost basis reference on-chain, distinguishing FlowMark from a costless log entry on a streaming dashboard.
- Removing a Stack lot burns the FLOW tied to that lot and retires the receipt ID, keeping receipt supply permanently linked to active HACD containers.

## What HACD adds

- **PoW container**: Each of the 256 HACD lots is a PoW-mined container. A StreamMark receipt is not a platform-rendered row — it is tied to a real mined asset whose formation time is immutable.
- **Formation cost**: 50 HAC per HACD lot. Total formation cost reference is 12,800 HAC. This makes anchoring a stream non-trivial and visibly committal.
- **Asset history**: Every formation event is inscribed on-chain. An external verifier (employer, auditor, revenue-share partner) can confirm exactly which HACD anchored which stream and when, without trusting the streaming platform.
- **Community formation**: The 1–10 HACD per participant cap and the designated-first genesis phase distribute receipt formation across the community rather than concentrating it.

## Main concerns

- GrowStreams auto-anchoring, revenue-share distributions, and the receipt marketplace are planned, not built. Public copy must mark these as planned and must not promise them as launch features.
- The streaming side depends on the GrowStreams protocol and Vara network, which are external to Hacash. FlowMark's HACD anchoring is independent of that, but the full product vision assumes GrowStreams availability.
- Issuer identity is not yet verified. HACD Labs should confirm team / operator identity privately before approval.
- The designated first phase (32 lots) gives the issuer genesis receipts; HACD Labs should confirm this is acceptable and that the designated address is the issuer's verified Hacash address.

## Required issuer confirmations

- Confirm 50 HAC per HACD is the final stack cost and not a placeholder.
- Confirm the designated address for the first 32 lots is the issuer's verified Hacash address.
- Confirm the maximum of 10 HACD per participant is enforced at the Launchpad level.
- Confirm GrowStreams auto-anchoring, revenue-share, and marketplace are marked as planned rather than promised in all public copy.
- Confirm team / operator identity to HACD Labs privately before approval.

## Recommended next step

Proceed to stack design and launch spec generation. Mark GrowStreams integration and revenue-share utility as roadmap dependencies in all public copy. HACD Labs internal review required before Launchpad publication.
