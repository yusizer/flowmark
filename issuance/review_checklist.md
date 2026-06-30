# Review Checklist: FlowMark (FLOW)

## Formation logic

- [x] Supply matches HACD lots: 256 × 10,000 = 2,560,000 ✓
- [x] Phase-lot sum: 32 (first) + 224 (public) = 256 = total_hacd_lots ✓
- [x] Stack cost is clear: 50 HAC per HACD, stated consistently across all documents
- [x] Participant flow is clear: step-by-step in stack_design.md and launchpad_copy.md
- [x] hacd_per_lot is 1 (standard, no unusual structure)
- [x] Removal / burn logic is defined and consistent (burn FLOW + retire receipt ID)
- [ ] Maximum per participant (10 HACD) enforcement confirmed at Launchpad level — **Needs issuer confirmation**
- [ ] Stack cost (50 HAC) confirmed as final — **Needs issuer confirmation**
- [x] Designated address for first 32 lots confirmed as issuer's Hacash address (15j5fHZzL8Qkzi7YBtChf2GDfM6RJvUht7)

## Copy safety

- [x] No profit promise in any document
- [x] No misleading backing claim: formation cost described as "formation cost reference" not "floor price"
- [x] No legal guarantee: risk disclosure present in launchpad_copy.md and issuer_faq.md
- [x] "Not financial advice" included in launchpad_copy.md and issuer_faq.md
- [x] "Not an investment" included in issuer_faq.md
- [x] GrowStreams auto-anchoring marked as planned / not guaranteed in all relevant documents
- [x] Revenue-share distributions marked as planned / not guaranteed in all relevant documents
- [x] Receipt marketplace marked as planned / not guaranteed in all relevant documents
- [x] No mention of exchange listing guarantee
- [x] No un-negated use of "yield", "profit", "floor", "guaranteed", "moon", "ROI", or "backed value"

## Launch readiness

- [ ] Launchpad URL — **Missing, to be confirmed by HACD Labs**
- [ ] Issuer identity confirmed to HACD Labs privately — **Pending**
- [x] Issuer X handle (@Yusifab7) and contact (yusifabdullayev48@gmail.com) replaced with real values
- [ ] Website replaced with live Lovable demo URL — **Pending demo build**
- [x] Issuer has confirmed numbers in intake form
- [ ] issuer_confirmed flag set to true in launch_spec.json — **Pending issuer sign-off**
- [ ] hacd_labs_reviewed flag set to true in launch_spec.json — **Pending HACD Labs review**
- [ ] Legal review completed — **Required before publication**

## Validator

- [x] launch_spec.json passes validate_launch_spec.py with no ERRORs
- [x] Supply math validated: 256 × 10,000 = 2,560,000
- [x] Phase-lot sum validated: 32 + 224 = 256
- [x] Formation cost reference: 12,800 HAC + network fees
- [ ] Final validated spec signed off by HACD Labs — **Pending**

## Outstanding items before Launchpad publication

1. Issuer confirms 50 HAC stack cost is final.
2. Issuer confirms 10 HACD max per participant is Launchpad-enforced.
3. Issuer provides verified designated Hacash address for the first 32 lots.
4. Issuer provides verified team / operator identity and real X handle / contact to HACD Labs.
5. HACD Labs assigns Launchpad URL and sets hacd_labs_reviewed to true.
6. Legal review completed and any required disclosures added.
7. issuer_confirmed and hacd_labs_reviewed flags updated to true in launch_spec.json.
8. Final re-run of validate_launch_spec.py on the approved spec.

---

*This checklist is part of a draft issuance package. Final parameters must be confirmed by the issuer and reviewed by HACD Labs before Launchpad publication.*
