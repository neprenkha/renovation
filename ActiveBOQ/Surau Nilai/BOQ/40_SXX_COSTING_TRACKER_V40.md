# Surau Nilai — SXX Costing Tracker V40

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/39_SXX_COSTING_TRACKER_V39.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V40 note — correction of S20/S21 markup classification

Owner corrected the workflow classification:

```text
S01-SXX in this BOQ workflow is for cost takeoff only.
Markup/gross margin/customer selling price is outside the SXX cost chain.
S20 should not be used as a markup SXX.
S21 should not open unless there is a real new cost/takeoff scope.
```

## Header/governance correction

New governance amendment created:

```text
GPTEditable/GPT_Header_Amendment_SXXCostOnly_NoMarkupInsideSXX_20260710.md
Commit: f6c61145d4c85efa6d20047a7cb1c5d80a7954dd
```

Active rule:

```text
SXX COST-ONLY CHAIN / NO MARKUP INSIDE SXX
```

## S20 corrected active files

```text
Correction audit:
ActiveBOQ/Surau Nilai/BOQ/S20_SXXCostOnly_NoMarkupCorrection_Recheck_V2.txt

Summary file:
ActiveBOQ/Surau Nilai/BOQ/S20_BOQXLSM_PASTE_READY_OR_SUMMARY_V2.txt
```

## S20 corrected decision

```text
S20 PREVIOUS MARKUP CLASSIFICATION: ERROR - SUPERSEDED
S20 COST TAKEOFF SCOPE: NO NEW CONSTRUCTION COST SCOPE AFTER S19
S20 SXX COST-ONLY CORRECTION / CLOSURE CHECKPOINT: PASS
S21 START ALLOWED: NO - NO CURRENT COST SCOPE
```

## What S21 is currently

```text
S21 has no defined BOQ cost/takeoff scope.
S21 is not markup.
S21 is not final customer price.
S21 is not open.
S21 may be created later only if owner adds a new cost scope, drawing/spec update, correction package, or reserved cost package.
```

## Current cost-chain basis retained

```text
S18 drawing/source coverage: 24/24 covered
S19 13G current-cost BOQ consolidation: PASS
No new S20 construction trade cost line required
No current S21 cost scope identified
```

## Current cost total retained

```text
S01-S16 corrected base working cost: RM748,244.00
Optional 10% contingency: RM74,824.40
Working cost with optional 10% contingency: RM823,068.40
S17 new cost impact: RM0.00
S18 new cost impact: RM0.00
S19 V2 new cost impact: RM0.00
S20 V2 new construction-cost impact: RM0.00
Customer selling price: OUTSIDE SXX - NOT PART OF BOQ COST TAKEOFF CHAIN
```

## Correct active paste/summary chain

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
S17_BOQXLSM_PASTE_READY_OR_SUMMARY_V3.txt
S18_BOQXLSM_PASTE_READY_OR_SUMMARY_V1.txt
S19_BOQXLSM_PASTE_READY_OR_SUMMARY_V2.txt
S20_BOQXLSM_PASTE_READY_OR_SUMMARY_V2.txt
```

## V40 strict checklist

```text
Owner correction checked: PASS
SXX cost-only rule captured: PASS
Markup removed from SXX active gate: PASS
S20 previous markup classification superseded: PASS
S20 no new construction cost scope confirmed: PASS
S21 not opened without cost scope: PASS
S18 24/24 drawing/source coverage retained: PASS
S19 13G cost consolidation retained: PASS
Current cost total retained: PASS
Header amendment created: PASS
```

## Current gate

```text
CURRENT ACTIVE SXX: COST CHAIN CLOSED AT S19 / S20 CORRECTION CHECKPOINT
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
S17 STRICT 100% RECHECK V3: PASS FOR CURRENT BOQ COST BASIS
S18 FINAL RESERVED SCOPE / PROJECT CLOSEOUT REVIEW: PASS FOR CURRENT BOQ COST BASIS
S19 13G STRICT 100% RECHECK V2: PASS FOR CURRENT BOQ COST BASIS
S20 SXX COST-ONLY CORRECTION / CLOSURE CHECKPOINT: PASS
S21 START ALLOWED: NO - NO CURRENT COST SCOPE
S01-S16 CORRECTED BASE WORKING COST: RM748,244.00
S01-S16 CORRECTED WORKING COST WITH OPTIONAL 10% CONTINGENCY: RM823,068.40
CUSTOMER SELLING PRICE / MARKUP: OUTSIDE SXX
```

## Next action

```text
Do not start S21 unless owner provides a new construction cost scope, drawing/spec update, correction package, or reserved cost package.
If owner wants selling price, create a separate commercial/pricing file outside the SXX cost takeoff chain.
```
