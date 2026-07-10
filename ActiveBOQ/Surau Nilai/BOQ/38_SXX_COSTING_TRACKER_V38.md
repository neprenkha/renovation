# Surau Nilai — SXX Costing Tracker V38

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/37_SXX_COSTING_TRACKER_V37.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V38 note — S19 13G strict 100 / no-missing-component recheck

Owner clarified the `100% / 99.9% gate` again:

```text
100% means current BOQ cost basis is complete: no missing known component, no missing rate, no wrong explicit drawing size/spec/quantity.
99.9% is fail if even one required item/component/rate is missing or wrong.
Logical/provisional estimate can pass when drawing data is incomplete, provided the estimate is complete, buildable, premium-sensible where appropriate, and all normal required components are included.
```

Latest owner uploaded header checked:

```text
GPTRenovationHeader.txt
Generated MYT: 2026-07-10 19:25
Section 13G: 100% completeness / logical estimate / no-missing-component rule
```

GitHub amendment checked:

```text
GPTEditable/GPT_Header_Amendment_100Percent_Completeness_NoMissingComponent_20260710.md
Commit: 5350950fd7c2e37b87b3181c56fffb52c2093fb5
```

## S19 V2 active files

```text
13G strict recheck audit:
ActiveBOQ/Surau Nilai/BOQ/S19_FinalCurrentCostBOQ_13G_Strict100_Recheck_Audit_V2.txt

Summary/paste-ready control file:
ActiveBOQ/Surau Nilai/BOQ/S19_BOQXLSM_PASTE_READY_OR_SUMMARY_V2.txt
```

## S19 V2 decision

```text
S19 13G STRICT 100% RECHECK V2: PASS FOR CURRENT BOQ COST BASIS
S19 NEW TRADE COST IMPACT: RM0.00
S20 START ALLOWED: YES - MARKUP / FINAL CUSTOMER OUTPUT PATH ONLY WHEN OWNER ASKS
```

## Why S19 remains PASS under 13G

S19 is not a new construction trade package. S19 is a final current-cost BOQ consolidation / paste-chain / no-missing-component recheck after S18 confirmed all 24 current drawing/source files are covered.

The S19 13G recheck confirms:

```text
S18 24/24 drawing/source coverage: PASS
No unassigned drawing/source scope after S18: PASS
No new S19 material/labour/service BOQ line required: PASS
Active S01-S18 paste chain present: PASS
S03 V2 correction retained: PASS
S13 premium-sensible provisional M&E component completeness: PASS
No known missing component/rate/line count in current BOQ basis: PASS
```

## S13 13G recheck note

S13 remains accepted as temporary complete current BOQ working-cost basis because the V2 estimate includes the normal required electrical/M&E components for a building of this size and quality:

```text
36 general light points
8 feature/external light points
6 emergency/exit points
10 fan points
28 socket points
18 switch/control points
10 AC power/isolator points
6 ventilation points
PA/audio wiring lot
8 CCTV/WiFi/data points
3-phase DB/protection/SPD/spare capacity allowance
earthing/bonding allowance
conduit/cable/trunking/fixing sundries allowance
10 AC condensate drain/sleeve points
electrical/low-voltage installation labour
AC point labour
PA/data labour
DB/earthing/testing labour
helper/skilled labour
testing/commissioning
ceiling access/making-good
tools/equipment
as-built/circuit labelling
```

Therefore S13 has no missing obvious current component under the owner-accepted provisional path. Future exact M&E drawing or supplier quote is a replacement/update only and not a current SXX blocker.

## S19 V2 current-cost total

```text
S01-S16 corrected base working cost: RM748,244.00
Optional 10% contingency: RM74,824.40
Working cost with optional 10% contingency: RM823,068.40
S17 new cost impact: RM0.00
S18 new cost impact: RM0.00
S19 V2 new cost impact: RM0.00
Customer selling price: NOT READY - markup/gross margin excluded by owner decision until owner asks
```

## Active BOQ.xlsm paste chain after S19 V2

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
```

## S19 V2 13G strict checklist

```text
Latest 13G owner header checked: PASS
GitHub 13G amendment checked: PASS
100% / 99.9% owner meaning checked: PASS
Explicit drawing data followed where current SXX had explicit data: PASS
Unclear/missing drawing data closed by logical/authorised allowance where needed: PASS
All active S01-S18 paste files present: PASS
S01-S16 active cost chain reconciled: PASS
S17/S18 no-cost reconciliation files present: PASS
S13 provisional M&E component completeness checked: PASS
No known visible/required component missing from active current BOQ basis: PASS
No required material/product/labour/service/rental/plant rate missing without accepted provisional/logical rate: PASS
No known explicit size/spec/quantity copied incorrectly in S19 consolidation: PASS
No line-count mismatch found in S19 consolidation: PASS
Duplicate prevention across all SXX: PASS
Markup/customer selling price excluded by owner decision: PASS
S19 final current-cost BOQ consolidation under 13G: PASS
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
S19 13G STRICT 100% RECHECK V2: PASS FOR CURRENT BOQ COST BASIS
S01-S16 CORRECTED BASE WORKING COST: RM748,244.00
S01-S16 CORRECTED WORKING COST WITH OPTIONAL 10% CONTINGENCY: RM823,068.40
CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN EXCLUDED BY OWNER DECISION
S20 START ALLOWED: YES - MARKUP / FINAL CUSTOMER OUTPUT PATH ONLY WHEN OWNER ASKS
```

## Header update decision

No new header update is required in this S19 recheck because the latest uploaded `GPTRenovationHeader.txt` already includes Section 13G. This tracker applies 13G to S19 execution.

## Next action

Proceed to S20 only if owner wants markup / gross margin / final customer quotation or another owner-requested final output path:

```text
S20_FinalCustomerPrice_Markup_GrossMargin_or_FinalQuotationOutput_Takeoff_Audit_V1.txt
S20_BOQXLSM_PASTE_READY_OR_SUMMARY_V1.txt
39_SXX_COSTING_TRACKER_V39.md
```
