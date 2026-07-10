# Surau Nilai — SXX Costing Tracker V32

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/31_SXX_COSTING_TRACKER_V31.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V32 note — S16 external utility / rainwater / garden tap strict recheck

Owner requested S16 to be repeatedly checked so that it can be taken off at 100% current BOQ cost basis and proceed to S17 only if it passes.

Latest owner uploaded header checked:

```text
GPTRenovationHeader.txt
Generated MYT: 2026-07-10 07:00
```

Owner repeated the strict gate:

```text
Take off to next SXX is only allowed at 100%.
99.9% is not a pass.
```

For S16, the active 100% target is:

```text
Current BOQ cost basis complete using customer site plan/survey drawings and customer/drawing accepted full allowance basis.
Customer selling price/margin is separate and not part of the current 100% target unless owner explicitly asks for selling price.
```

## S16 source checked

```text
Surau Site Plan Tender_Constn.pdf
Survey Tapak Surau Juassewh Sentosa.pdf
Surau Plan Roof Plan Bldg Tender_Constn.pdf
S06 under-slab plumbing / sanitary rough-in boundary
S09 roof rainwater goods boundary
S13 electrical/M&E boundary
S14 road and drainage boundary
S15 fencing/gate/meter enclosure boundary
```

## S16 drawing/spec facts

```text
Site plan title: SITE PLAN
Scale: 1:100
Project: Cadangan Membina 1 Unit Surau 1 Tingkat Diatas Lot 20093, Taman Juasseh Sentosa
Lot 20093 area shown: 1,759 m2 / 18,934 SF
Garden tap labels are visible at multiple external locations around the site.
Rainwater harvesting tank note is shown on site plan.
1 day supply suction tank to engineer's detail is shown on site plan.
Conc paving to detail is shown near main entrance / external walk interface.
Stormwater discharge outlet and perimeter drain are S14 drainage boundary and not double counted as drain body.
Electrical meter / water meter / rubbish compartment positions are S15 gatepost/enclosure boundary; S16 carries only water utility function/interface where relevant.
```

## S16 active files

```text
Rate reference:
ActiveBOQ/Surau Nilai/BOQ/S16_ExternalUtility_Rainwater_GardenTap_RateReference_V1.txt

Repeated recheck file:
ActiveBOQ/Surau Nilai/BOQ/S16_ExternalUtility_Rainwater_GardenTap_Recheck_Audit_V1.md

Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S16_ExternalUtility_Rainwater_GardenTap_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S16_BOQXLSM_PASTE_READY_V1.txt
```

Only `S16_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm` for S16.

## S16 quantity basis

| Item | Quantity basis | S16 current BOQ quantity |
|---|---|---:|
| Rainwater harvesting tank | Site plan note: rainwater harvesting tank to engineer's detail | 1 set |
| 1 day supply suction tank | Site plan note: 1 day supply suction tank to engineer's detail | 1 set |
| Garden tap points | Visible site plan garden tap labels at perimeter/external locations | 4 points |
| External water supply pipework | Drawing-derived route allowance from meter/tank to taps around building/perimeter | 95 m |
| Rainwater harvesting overflow/transfer pipework | Drawing-derived interface from roof water/tank to drain/tank route | 45 m |
| External concrete paving | Site plan conc paving to detail, excluding S07/S14 | 55 m2 |
| Garden tap marker/protection apron | One at each garden tap point | 4 points |
| Testing/flushing | Full lot for S16 external utility | 1 lot |
| Small plant/tools | Full lot for S16 external utility/paving | 1 lot |
| Making good/cleaning | Full lot for S16 external utility/paving | 1 lot |

## S16 cost summary

```text
Block 1 material: RM23,680.00
Block 2 labour:   RM6,170.00
Block 3 service:  RM3,550.00
Base working cost: RM33,400.00
Optional 10% contingency: RM3,340.00
Working cost with contingency: RM36,740.00
Customer selling price: NOT READY - markup/gross margin not applied
```

## S16 strict gate checklist

```text
Source drawing rendered/visually checked: PASS
Rainwater harvesting tank included: PASS
1 day supply suction tank included: PASS
Garden taps included: PASS
External water pipework included: PASS
Rainwater overflow/transfer included: PASS
Concrete paving included: PASS
S06 duplicate prevention: PASS
S09 duplicate prevention: PASS
S13 duplicate prevention: PASS
S14 duplicate prevention: PASS
S15 duplicate prevention: PASS
Block 1 complete: PASS
Block 2 complete: PASS
Block 3 complete: PASS
Markup check: PASS
100% / 99.9% gate: PASS
```

## Current gate

```text
CURRENT ACTIVE SXX: S17
S01 WORKING-COST BASIS: COMPLETE - KEEP FOR INTERNAL COST PLANNING
S01 BOQ.XLSM PASTE FILE: READY - WORKING-COST ONLY
S01 DRAWING/SPEC RESCAN: STILL REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ
S02 WORKING-COST BASIS: COMPLETE - KEEP FOR INTERNAL COST PLANNING
S02 BOQ.XLSM PASTE FILE: READY - WORKING-COST ONLY
S02 DRAWING/SPEC RESCAN: STILL REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ
S03 WORKING-COST BASIS: COMPLETE - KEEP FOR INTERNAL COST PLANNING
S03 BOQ.XLSM PASTE FILE: READY - WORKING-COST ONLY
S03 DRAWING/SPEC RESCAN: STILL REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ
S04 WORKING-COST DRAWING/SPEC BASIS: COMPLETE
S04 BOQ.XLSM PASTE FILE: READY - USE V2
S05 WORKING-COST DRAWING/SPEC BASIS: COMPLETE
S05 BOQ.XLSM PASTE FILE: READY - USE V1
S06 WORKING-COST DRAWING/SPEC BASIS: COMPLETE AFTER RECHECK - USE V2
S06 BOQ.XLSM PASTE FILE: READY - USE V2
S07 WORKING-COST DRAWING/SPEC BASIS: COMPLETE AFTER RECHECK - USE V1
S07 BOQ.XLSM PASTE FILE: READY - USE V1
S08 COMPLETE FOR NEXT SXX - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS
S08 BOQ.XLSM PASTE FILE: READY - USE V2
S09 COMPLETE FOR NEXT SXX - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS
S09 BOQ.XLSM PASTE FILE: READY - USE V1
S10 COMPLETE FOR NEXT SXX - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS
S10 BOQ.XLSM PASTE FILE: READY - USE V1
S11 STRICT 100% CURRENT BOQ COST BASIS: PASS
S11 ACTIVE ALUMINIUM/GLASS SCHEDULE: USE V2
S11 ACTIVE AUDIT FILE: USE V3
S11 ACTIVE BOQ.XLSM PASTE FILE: USE V2
S12 STRICT 100% CURRENT BOQ COST BASIS: PASS
S12 ACTIVE AUDIT FILE: USE V1
S12 ACTIVE BOQ.XLSM PASTE FILE: USE V1
S13 WORKING-COST ESTIMATE COMPLETE - OWNER ACCEPTED PREMIUM-SENSIBLE SIZE-BASED PROVISIONAL PATH
S13 ACTIVE AUDIT FILE: USE V2
S13 ACTIVE BOQ.XLSM PASTE FILE: USE V2
S13 DRAWING-SPEC EXACT ELECTRICAL DESIGN: HOLD UNTIL DEDICATED ELECTRICAL DRAWING / OWNER CONFIRMED ELECTRICAL SCHEDULE
S14 STRICT 100% CURRENT BOQ COST BASIS: PASS
S14 ACTIVE AUDIT FILE: USE V1
S14 ACTIVE BOQ.XLSM PASTE FILE: USE V1
S15 STRICT 100% CURRENT BOQ COST BASIS: PASS
S15 ACTIVE AUDIT FILE: USE V1
S15 ACTIVE BOQ.XLSM PASTE FILE: USE V1
S16 STRICT 100% CURRENT BOQ COST BASIS: PASS
S16 ACTIVE AUDIT FILE: USE V1
S16 ACTIVE BOQ.XLSM PASTE FILE: USE V1
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S06 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S07 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S08 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S09 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S10 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S11 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S12 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S13 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S14 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S15 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S16 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S17 START ALLOWED: YES - OVERALL RECONCILIATION / FINAL BOQ REVIEW PATH
```

## Header update decision

No new header update is required because the latest uploaded `GPTRenovationHeader.txt` already contains:

```text
13B Drawing/spec and auditable takeoff rule
13C BOQ.xlsm paste-ready output rule
13D Drawing-spec SXX completion gate
13E Authorised allowance / 100% current BOQ cost basis rule
```

## Next action

Proceed to S17 on overall reconciliation / final BOQ review path:

```text
S17_OverallReconciliation_FinalBOQReview_Takeoff_Audit_V1.txt
S17_BOQXLSM_PASTE_READY_OR_SUMMARY_V1.txt
33_SXX_COSTING_TRACKER_V33.md
```
