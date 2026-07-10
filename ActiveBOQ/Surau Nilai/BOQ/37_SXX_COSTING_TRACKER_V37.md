# Surau Nilai — SXX Costing Tracker V37

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/36_SXX_COSTING_TRACKER_V36.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V37 note — S19 final current-cost BOQ consolidation

Owner requested S19 to be repeatedly checked so that S19 can be confirmed at 100% according to current customer drawing/spec cost basis and proceed to S20 only if it passes.

Latest owner uploaded header checked:

```text
GPTRenovationHeader.txt
Generated MYT: 2026-07-10 07:00
```

Owner strict gate repeated:

```text
Take off to next SXX is only allowed at 100%.
99.9% is not a pass.
```

## S19 active files

```text
Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S19_FinalCurrentCostBOQ_Consolidation_Takeoff_Audit_V1.txt

Summary/paste-ready control file:
ActiveBOQ/Surau Nilai/BOQ/S19_BOQXLSM_PASTE_READY_OR_SUMMARY_V1.txt
```

## S19 decision

```text
S19 FINAL CURRENT-COST BOQ CONSOLIDATION: PASS FOR CURRENT BOQ COST BASIS
S19 NEW TRADE COST IMPACT: RM0.00
S20 START ALLOWED: YES - MARKUP / FINAL CUSTOMER OUTPUT PATH ONLY WHEN OWNER ASKS
```

## S19 scope clarification

S19 is not a new construction trade package. S19 is a final current-cost BOQ consolidation and paste-chain audit after S18 confirmed 24/24 current drawing/source coverage.

S19 does not add new material, labour or service cost lines.

## Drawing/source coverage carried forward

S18 confirmed:

```text
S18 FINAL RESERVED SCOPE / PROJECT CLOSEOUT REVIEW: PASS FOR CURRENT BOQ COST BASIS
S18 NEW TRADE COST IMPACT: RM0.00
S18 DRAWING/SOURCE COVERAGE CHECK: 24/24 CURRENT DRAWINGS COVERED
```

S19 rechecked that no new unassigned drawing/source scope is introduced after S18.

## Active BOQ.xlsm paste chain after S19

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
S19_BOQXLSM_PASTE_READY_OR_SUMMARY_V1.txt
```

## S19 current-cost total

```text
S01-S16 corrected base working cost: RM748,244.00
Optional 10% contingency: RM74,824.40
Working cost with optional 10% contingency: RM823,068.40
S17 new cost impact: RM0.00
S18 new cost impact: RM0.00
S19 new cost impact: RM0.00
Customer selling price: NOT READY - markup/gross margin excluded by owner decision until owner asks
```

## S19 strict checklist

```text
Latest owner header checked: PASS
100% / 99.9% gate checked: PASS
V36/S18 drawing-source coverage checked: PASS
No unassigned drawing scope found after S18: PASS
Active BOQ.xlsm paste chain checked: PASS
S01 rescan status checked: PASS
S02 rescan status checked: PASS
S03 V2 correction checked: PASS
S04-S16 active file chain checked: PASS
S13 owner-accepted provisional M&E basis not treated as current blocker: PASS
Markup/customer selling price excluded by owner decision: PASS
No new S19 material/labour/service BOQ line required: PASS
S19 final current-cost BOQ consolidation: PASS
S20 start gate: PASS
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
S19 FINAL CURRENT-COST BOQ CONSOLIDATION: PASS FOR CURRENT BOQ COST BASIS
S01-S16 CORRECTED BASE WORKING COST: RM748,244.00
S01-S16 CORRECTED WORKING COST WITH OPTIONAL 10% CONTINGENCY: RM823,068.40
CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN EXCLUDED BY OWNER DECISION
S20 START ALLOWED: YES - MARKUP / FINAL CUSTOMER OUTPUT PATH ONLY WHEN OWNER ASKS
```

## Header update decision

No new header update is required. The latest uploaded `GPTRenovationHeader.txt` already covers:

```text
13B Drawing/spec and auditable takeoff rule
13C BOQ.xlsm paste-ready output rule
13D Drawing-spec SXX completion gate
13E Authorised allowance / 100% current BOQ cost basis rule
Price/cost rule separating working cost from customer selling price
```

S19 is an execution/tracker consolidation step, not a new permanent governance rule.

## Next action

Proceed to S20 only if owner wants markup / gross margin / final customer quotation or another owner-requested final output path:

```text
S20_FinalCustomerPrice_Markup_GrossMargin_or_FinalQuotationOutput_Takeoff_Audit_V1.txt
S20_BOQXLSM_PASTE_READY_OR_SUMMARY_V1.txt
38_SXX_COSTING_TRACKER_V38.md
```
