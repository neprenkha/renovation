# Surau Nilai — SXX Costing Tracker V13

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/12_SXX_COSTING_TRACKER_V12.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V13 correction note

Owner clarified that working cost is acceptable and customer margin/profit will be calculated later. The required gate is not customer selling price. The required gate is:

```text
WORKING-COST DRAWING/SPEC BASIS
with undercost / overprice / double-count check recorded
```

S04 has now been corrected from V1 allowance basis to V2 measured drawing/spec working-cost basis.

## Current gate

```text
CURRENT ACTIVE SXX: S05
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
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 START ALLOWED: YES - WORKING-COST DRAWING/SPEC PATH
```

## S04 V2 final files

```text
Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S04_CrossingBridge_Entrance_Takeoff_Audit_V2.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S04_BOQXLSM_PASTE_READY_V2.txt
```

Only `S04_BOQXLSM_PASTE_READY_V2.txt` should be copied into `*BOQ.xlsm` for S04. Do not use S04 V1 unless comparing old undercost.

## S04 cost summary

```text
Block 1 material: RM28,374.11
Block 2 labour:   RM5,680.00
Block 3 service:  RM1,950.00
Base working cost: RM36,004.11
Optional 10% contingency: RM3,600.41
Working cost with contingency: RM39,604.52
Customer selling price: NOT READY - markup/gross margin not applied
```

## S04 undercost / overprice / double-count check

```text
Drawing/spec scope included: YES - rendered CROSSING BRIDGE.pdf used
Missing required line check: PASS - G30, G15, rebar, formwork, labour, backhoe and concrete placing access included
Undercost check: PASS - V1 undercost corrected by adding full bridge structural elements and G30/G15 grades
Overprice check: PASS WITH NOTE - beam concrete measured net below slab to avoid double counting slab/beam overlap
Double-count check: PASS - excludes S03 general earthwork, S05 building substructure, S22 drainage and S24 road/premix
Markup check: PASS - no customer markup included
Supplier/site verification items: rebar BBS and concrete pump/access quote may refine later
```

## SXX tracker

| SXX | Proposed scope | Working-cost status | BOQ.xlsm paste file | Drawing/spec status | Required source check | Notes |
|---|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | COMPLETE | `S01_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `Hoarding and Signboard 1.pdf`, site plan, survey | Existing base working cost RM8,750.00; optional 10% contingency RM875.00; with contingency RM9,625.00. No customer markup. |
| S02 | ESCP and temporary erosion/sediment control | COMPLETE | `S02_BOQXLSM_PASTE_READY_V2.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01ESCP-LP-01-S0-00.pdf` | Existing base working cost RM1,944.00; optional 10% contingency RM194.40; with contingency RM2,138.40. No customer markup. |
| S03 | Site clearing, earthwork, cut/fill and platform formation | COMPLETE | `S03_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01EW-CS-01-S0-00.pdf`, `SJ_01EW-DT-01-S0-00.pdf`, `SJ_01EW-LP-01-S0-00.pdf`, site plan/survey | Existing base working cost RM2,090.00; optional 10% contingency RM209.00; with contingency RM2,299.00. No customer markup. |
| S04 | Crossing bridge and permanent site entrance | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S04_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `CROSSING BRIDGE.pdf` rendered and visually inspected | Base working cost RM36,004.11; optional 10% contingency RM3,600.41; with contingency RM39,604.52. No customer markup. V1 undercost superseded. |
| S05 | Building substructure: footing, stump and ground beam | START ALLOWED | - | NOT STARTED | `04-SURAU JERUSSALAM GROUND BEAM DETAIL 01.pdf`, `05-SURAU JERUSSALAM GROUND BEAM DETAIL 02.pdf`, slab/section/source drawings as needed | Must produce both audit/reference and BOQ.xlsm paste-ready output. Work on drawing/spec working-cost path; margin later. |

## Next action

Proceed to S05 on working-cost drawing/spec path:

```text
S05_BuildingSubstructure_Takeoff_Audit_V1.txt
S05_BOQXLSM_PASTE_READY_V1.txt
14_SXX_COSTING_TRACKER_V14.md
```
