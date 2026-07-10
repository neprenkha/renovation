# Surau Nilai — SXX Costing Tracker V34

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/33_SXX_COSTING_TRACKER_V33.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V34 note — S17 correction after owner clarification

Owner corrected S17 V1 logic:

```text
Markup/customer price must be ignored for now because owner already said markup will be discussed after all scope is complete.
S13 premium-sensible provisional electrical/M&E estimate is accepted as temporary 100% working-cost basis for SXX continuity.
S13 must not block later SXX unless final electrical/M&E design is specifically required.
S01-S03 should be rescanned and corrected rather than left as blockers.
```

## Correction actions completed

```text
S01 rescan completed:
ActiveBOQ/Surau Nilai/BOQ/S01_Preliminaries_DrawingSpec_Rescan_Audit_V1.md

S02 rescan completed:
ActiveBOQ/Surau Nilai/BOQ/S02_ESCP_DrawingSpec_Rescan_Audit_V1.md

S03 rescan completed and revised:
ActiveBOQ/Surau Nilai/BOQ/S03_Earthwork_DrawingSpec_Revised_Takeoff_Audit_V2.txt
ActiveBOQ/Surau Nilai/BOQ/S03_BOQXLSM_PASTE_READY_V2.txt

S17 corrected reconciliation:
ActiveBOQ/Surau Nilai/BOQ/S17_OverallReconciliation_FinalBOQReview_Takeoff_Audit_V2.txt
ActiveBOQ/Surau Nilai/BOQ/S17_BOQXLSM_PASTE_READY_OR_SUMMARY_V2.txt
```

## S01-S03 corrected status

```text
S01 DRAWING/SPEC RESCAN: PASS FOR CURRENT BOQ COST BASIS - USE V1
S02 DRAWING/SPEC RESCAN: PASS FOR CURRENT BOQ COST BASIS - USE V2
S03 DRAWING/SPEC RESCAN: PASS AND COST REVISED - USE V2
```

S03 correction reason:

```text
Earthwork drawing quantity table shows:
FILL 255m3
CUT 222m3
Net import/fill balance 33m3
Export 0m3

Old S03 V1 base working cost RM2,090.00 was too low against the drawing quantity table.
S03 V2 base working cost is RM18,743.50.
```

## S17 V2 decision

```text
S17 OVERALL RECONCILIATION: PASS FOR CURRENT BOQ COST BASIS
S17 FINAL CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED BY OWNER DECISION
S17 DRAWING-SPEC FINAL ELECTRICAL DESIGN: S13 PROVISIONAL PREMIUM-SENSIBLE ESTIMATE ACCEPTED FOR TEMPORARY WORKING-COST BASIS
S18 START ALLOWED: YES - CURRENT BOQ COST BASIS PATH
```

## Corrected S01-S16 total after S03 V2

```text
Previous S17 V1 total S01-S16 base working cost: RM731,590.50
Less old S03 V1 base: RM2,090.00
Add revised S03 V2 base: RM18,743.50
Corrected S01-S16 base working cost: RM748,244.00

Corrected optional 10% contingency: RM74,824.40
Corrected working cost with contingency: RM823,068.40

Customer selling price: NOT READY - deliberately ignored until owner asks for markup/gross margin stage
```

## Active BOQ.xlsm paste files after correction

```text
S01_BOQXLSM_PASTE_READY_V1.txt
S02_BOQXLSM_PASTE_READY_V2.txt
S03_BOQXLSM_PASTE_READY_V2.txt
S04_BOQXLSM_PASTE_READY_V2.txt
S05_BOQXLSM_PASTE_READY_V1.txt
S06_BOQXLSM_PASTE_READY_V2.txt
S07_BOQXLSM_PASTE_READY_V1.txt
S08_BOQXLSM_PASTE_READY_V2.txt
S09_BOQXLSM_PASTE_READY_V1.txt
S10_BOQXLSM_PASTE_READY_V1.txt
S11_BOQXLSM_PASTE_READY_V2.txt
S12_BOQXLSM_PASTE_READY_V1.txt
S13_BOQXLSM_PASTE_READY_V2.txt
S14_BOQXLSM_PASTE_READY_V1.txt
S15_BOQXLSM_PASTE_READY_V1.txt
S16_BOQXLSM_PASTE_READY_V1.txt
```

## S17 V2 gate checklist

```text
S01 drawing/spec rescan: PASS
S02 drawing/spec rescan: PASS
S03 drawing/spec rescan and cost correction: PASS - USE V2
S04 current BOQ cost basis: PASS
S05 current BOQ cost basis: PASS
S06 current BOQ cost basis: PASS
S07 current BOQ cost basis: PASS
S08 authorised full allowance basis: PASS
S09 authorised full allowance basis: PASS
S10 authorised full allowance basis: PASS
S11 aluminium/glass schedule and cost basis: PASS
S12 current BOQ cost basis: PASS
S13 owner-accepted premium-sensible provisional M&E basis: PASS FOR TEMPORARY WORKING-COST SEQUENCING
S14 current BOQ cost basis: PASS
S15 current BOQ cost basis: PASS
S16 current BOQ cost basis: PASS
Markup/customer selling price excluded by owner decision: PASS
100% / 99.9% gate for current BOQ cost basis: PASS
```

## Current gate

```text
CURRENT ACTIVE SXX: S18
S01 DRAWING/SPEC RESCAN: PASS FOR CURRENT BOQ COST BASIS - USE V1
S02 DRAWING/SPEC RESCAN: PASS FOR CURRENT BOQ COST BASIS - USE V2
S03 DRAWING/SPEC RESCAN: PASS AND COST REVISED - USE V2
S04 WORKING-COST DRAWING/SPEC BASIS: COMPLETE - USE V2
S05 WORKING-COST DRAWING/SPEC BASIS: COMPLETE - USE V1
S06 WORKING-COST DRAWING/SPEC BASIS: COMPLETE AFTER RECHECK - USE V2
S07 WORKING-COST DRAWING/SPEC BASIS: COMPLETE AFTER RECHECK - USE V1
S08 COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS - USE V2
S09 COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS - USE V1
S10 COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS - USE V1
S11 STRICT 100% CURRENT BOQ COST BASIS: PASS - USE AUDIT V3 / PASTE V2
S12 STRICT 100% CURRENT BOQ COST BASIS: PASS - USE V1
S13 WORKING-COST ESTIMATE COMPLETE - OWNER ACCEPTED PREMIUM-SENSIBLE SIZE-BASED PROVISIONAL PATH - USE V2
S13 DRAWING-SPEC EXACT ELECTRICAL DESIGN: HOLD FOR FUTURE M&E UPDATE ONLY, NOT A BLOCKER FOR SXX CONTINUITY
S14 STRICT 100% CURRENT BOQ COST BASIS: PASS - USE V1
S15 STRICT 100% CURRENT BOQ COST BASIS: PASS - USE V1
S16 STRICT 100% CURRENT BOQ COST BASIS: PASS - USE V1
S17 OVERALL RECONCILIATION: PASS FOR CURRENT BOQ COST BASIS - USE V2
S01-S16 CORRECTED BASE WORKING COST: RM748,244.00
S01-S16 CORRECTED WORKING COST WITH OPTIONAL 10% CONTINGENCY: RM823,068.40
CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED BY OWNER DECISION
S18 START ALLOWED: YES - CURRENT BOQ COST BASIS PATH
```

## Header update decision

No new header update is required because the latest uploaded `GPTRenovationHeader.txt` already says customer selling price/margin is separate from current SXX completion unless owner asks, and already allows a working-cost-only path when owner accepts it. This V34 corrects execution/tracker logic rather than adding a new permanent governance rule.

## Next action

Proceed to S18 on current BOQ cost basis path:

```text
S18_FinalReservedScope_or_ProjectCloseoutReview_Takeoff_Audit_V1.txt
S18_BOQXLSM_PASTE_READY_OR_SUMMARY_V1.txt
35_SXX_COSTING_TRACKER_V35.md
```