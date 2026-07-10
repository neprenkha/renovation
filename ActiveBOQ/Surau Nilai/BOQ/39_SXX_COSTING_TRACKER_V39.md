# Surau Nilai — SXX Costing Tracker V39

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/38_SXX_COSTING_TRACKER_V38.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V39 note — S20 13G strict recheck HOLD

Owner requested S20 to be repeatedly checked so that S20 can be confirmed at 100% according to customer drawing/spec and proceed to S21 only if it passes.

Latest owner uploaded header checked:

```text
GPTRenovationHeader.txt
Generated MYT: 2026-07-10 19:25
Section 13G: 100% completeness / logical estimate / no-missing-component rule
```

Owner strict gate repeated:

```text
Take off to next SXX is only allowed at 100%.
99.9% is not a pass.
```

## S20 active files

```text
Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S20_FinalCustomerPrice_Markup_GrossMargin_FinalOutput_Recheck_HOLD_V1.txt

Summary/HOLD file:
ActiveBOQ/Surau Nilai/BOQ/S20_BOQXLSM_PASTE_READY_OR_SUMMARY_HOLD_V1.txt
```

## S20 decision

```text
S20 FINAL CUSTOMER PRICE / MARKUP / GROSS MARGIN PATH: HOLD
S20 CONSTRUCTION DRAWING-COST TAKEOFF: NO NEW TRADE SCOPE AFTER S19
S20 CURRENT BOQ COST BASIS CARRY-FORWARD: S01-S19 PASS
S21 START ALLOWED: NO
```

## Why S20 cannot pass 100% now

S18 and S19 already closed the current construction drawing-cost basis:

```text
S18 drawing/source coverage: 24/24 covered
S19 13G current-cost BOQ consolidation: PASS
No new S20 construction trade cost line required
```

However, V38 opened S20 only for:

```text
Markup / final customer output path
```

A final customer price/gross margin output cannot be 100% because owner has not supplied or approved the markup percentage, target gross margin, selling-rate policy, or instruction to output a working-cost-only final customer summary.

Under 13G, creating a markup or final customer price without owner-approved commercial basis would be an invented rate/policy, not 100%.

## Current cost basis retained

```text
S01-S16 corrected base working cost: RM748,244.00
Optional 10% contingency: RM74,824.40
Working cost with optional 10% contingency: RM823,068.40
S17 new cost impact: RM0.00
S18 new cost impact: RM0.00
S19 V2 new cost impact: RM0.00
S20 new construction-cost impact: RM0.00
Customer selling price: NOT READY - markup/gross margin excluded until owner approves pricing method
```

## S20 13G strict checklist

```text
Latest 13G owner header checked: PASS
GitHub 13G amendment checked: PASS
V38/S19 current-cost consolidation checked: PASS
S18 24/24 drawing-source coverage checked: PASS
S01-S19 current BOQ cost basis carried forward: PASS
No new construction trade line required for S20: PASS
Markup/gross-margin/final customer pricing basis supplied by owner: FAIL / NOT PROVIDED
Inventing markup or customer price without owner instruction blocked: PASS
S20 final customer output 100% gate: HOLD
S21 start gate: FAIL / NO
```

## Current gate

```text
CURRENT ACTIVE SXX: S20
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
S20 FINAL CUSTOMER PRICE / MARKUP / GROSS MARGIN PATH: HOLD
S01-S16 CORRECTED BASE WORKING COST: RM748,244.00
S01-S16 CORRECTED WORKING COST WITH OPTIONAL 10% CONTINGENCY: RM823,068.40
CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT PROVIDED/APPROVED
S21 START ALLOWED: NO
```

## Header update decision

No new header update is required. The latest uploaded `GPTRenovationHeader.txt` already includes Section 13G and correctly requires S20 to HOLD when the active S20 path is missing an owner-approved commercial pricing basis.

## Required owner decision to complete S20 later

S20 can pass later only after owner provides or confirms one of these:

```text
1. markup percentage; or
2. target gross margin percentage; or
3. instruction to output working-cost-only final summary with no customer selling price; or
4. another explicit final output path.
```
