# Surau Nilai — SXX Costing Tracker V28

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/27_SXX_COSTING_TRACKER_V27.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V28 note — S13 owner accepted size-based estimate path

Owner clarified that S13 may proceed as an estimate based on surau size, full-area electrical need and aircond demand so that the workflow can continue to S14.

This does not convert S13 into exact electrical drawing/spec measured completion.

## S13 status

```text
S13 WORKING-COST ESTIMATE COMPLETE - OWNER ACCEPTED SIZE-BASED PROVISIONAL PATH
S13 DRAWING-SPEC EXACT ELECTRICAL DESIGN: HOLD UNTIL DEDICATED ELECTRICAL DRAWING / OWNER CONFIRMED ELECTRICAL SCHEDULE
S13 BOQ.XLSM PASTE FILE: READY - USE V1
S14 START ALLOWED: YES - WORKING-COST ESTIMATE PATH
```

## S13 active files

```text
Assumption file:
ActiveBOQ/Surau Nilai/BOQ/S13_Electrical_Aircond_SizeBased_Estimate_Assumption_V1.md

Rate reference:
ActiveBOQ/Surau Nilai/BOQ/S13_Electrical_Aircond_RateReference_V1.txt

Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S13_Electrical_Lighting_Power_Mechanical_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S13_BOQXLSM_PASTE_READY_V1.txt
```

Only `S13_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm` for S13.

## Area and aircond basis

| Basis | Quantity | Use |
|---|---:|---|
| Covered internal / ceiling finish area | 232.63 m2 / 2,504 ft2 | Full internal electrical coverage estimate area |
| Main prayer / carpet substrate area | 98.50 m2 / 1,060 ft2 | Main hall aircond/fan comfort estimate |
| Full-building aircond allowance | 8 AC points | About 18HP to 20HP class, about 166,000 to 184,000 BTU/h |
| Main hall practical AC allowance | 4 units x 3.0HP class | About 112,000 BTU/h for main worship zone |
| Estimated working electrical demand | 25kW to 30kW | Preliminary 3-phase DB/submain allowance only |

## Point quantity basis

| Item | Quantity | Basis |
|---|---:|---|
| General lighting points | 30 points | 232.63m2 at about one point per 7.5-8.5m2 |
| Emergency / exit light points | 4 points | Limited EL labels visible/extracted |
| Ceiling fan / air movement points | 8 points | 4 visible KS labels + 4 size/high-roof comfort allowance |
| General power socket outlets | 22 points | Full-building allowance for surau/office/cleaning/PA/support |
| Switch / control points | 14 points | Lighting/fan/control zones |
| Aircond power isolator points | 8 points | Full-building 18HP-20HP class aircond allowance |
| Exhaust fan / ventilation points | 4 points | Toilets/wet/internal ventilation allowance |
| Distribution board / protection | 1 lot | 25kW-30kW working demand allowance |
| Earthing / bonding | 1 lot | Small public building allowance |

## S13 cost summary

```text
Block 1 material: RM30,290.00
Block 2 labour:   RM11,740.00
Block 3 service:  RM3,550.00
Base working cost: RM45,580.00
Optional 10% contingency: RM4,558.00
Working cost with contingency: RM50,138.00
Customer selling price: NOT READY - markup/gross margin not applied
```

## S13 strict status note

```text
This S13 is NOT exact electrical drawing/spec measured.
This S13 is owner-approved size-based working-cost estimate.
Dedicated electrical drawing/spec can replace this later by V2 correction.
S14 may start only because owner accepted the provisional estimate path.
```

## Current gate

```text
CURRENT ACTIVE SXX: S14
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
S13 WORKING-COST ESTIMATE COMPLETE - OWNER ACCEPTED SIZE-BASED PROVISIONAL PATH
S13 ACTIVE AUDIT FILE: USE V1
S13 ACTIVE BOQ.XLSM PASTE FILE: USE V1
S13 DRAWING-SPEC EXACT ELECTRICAL DESIGN: HOLD UNTIL DEDICATED ELECTRICAL DRAWING / OWNER CONFIRMED ELECTRICAL SCHEDULE
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
S14 START ALLOWED: YES - WORKING-COST ESTIMATE PATH
```

## Header update decision

No new header update is required because the current uploaded header already allows a working-cost sequencing path when the owner accepts it, as long as it is not mislabelled as drawing-spec measured completion.

## Next action

Proceed to S14 on working-cost estimate path:

```text
S14_ExternalWorks_Rainwater_Drainage_or_next_scope_Takeoff_Audit_V1.txt
S14_BOQXLSM_PASTE_READY_V1.txt
29_SXX_COSTING_TRACKER_V29.md
```
