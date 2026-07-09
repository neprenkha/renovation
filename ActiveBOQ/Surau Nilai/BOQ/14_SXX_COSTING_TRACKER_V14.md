# Surau Nilai — SXX Costing Tracker V14

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/13_SXX_COSTING_TRACKER_V13.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V14 note

S05 has been completed on the owner-confirmed path:

```text
WORKING-COST DRAWING/SPEC BASIS
Margin/profit/customer selling price later
Undercost / overprice / double-count check recorded
```

## Current gate

```text
CURRENT ACTIVE SXX: S06
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
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S06 START ALLOWED: YES - WORKING-COST DRAWING/SPEC PATH
```

## S05 final files

```text
Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S05_BuildingSubstructure_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S05_BOQXLSM_PASTE_READY_V1.txt
```

Only `S05_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm` for S05.

## S05 cost summary

```text
Block 1 material: RM19,869.07
Block 2 labour:   RM8,520.00
Block 3 service:  RM2,700.00
Base working cost: RM31,089.07
Optional 10% contingency: RM3,108.91
Working cost with contingency: RM34,197.98
Customer selling price: NOT READY - markup/gross margin not applied
```

## S05 undercost / overprice / double-count check

```text
Drawing/spec scope included: YES - rendered foundation/ground beam drawings used
Missing required line check: PASS - G25, G15, rebar, formwork, labour, backhoe and concrete placing access included
Undercost check: PASS - pad footings, stump/column starter, ground beam, lean concrete and rebar/formwork basis included
Overprice check: PASS WITH NOTE - S07 slab/hardcore/DPM/BRC excluded; if trench-cast ground beams are later confirmed without formwork, reduce formwork in correction version
Double-count check: PASS - excludes S03 general earthwork/platform, S04 bridge, S07 slab/apron, S08 columns/roof beams, S22/S24 external works
Markup check: PASS - no customer markup included
Supplier/site verification items: rebar BBS, concrete pump/access quote and formwork method may refine later
```

## SXX tracker

| SXX | Proposed scope | Working-cost status | BOQ.xlsm paste file | Drawing/spec status | Required source check | Notes |
|---|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | COMPLETE | `S01_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `Hoarding and Signboard 1.pdf`, site plan, survey | Existing base working cost RM8,750.00; optional 10% contingency RM875.00; with contingency RM9,625.00. No customer markup. |
| S02 | ESCP and temporary erosion/sediment control | COMPLETE | `S02_BOQXLSM_PASTE_READY_V2.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01ESCP-LP-01-S0-00.pdf` | Existing base working cost RM1,944.00; optional 10% contingency RM194.40; with contingency RM2,138.40. No customer markup. |
| S03 | Site clearing, earthwork, cut/fill and platform formation | COMPLETE | `S03_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01EW-CS-01-S0-00.pdf`, `SJ_01EW-DT-01-S0-00.pdf`, `SJ_01EW-LP-01-S0-00.pdf`, site plan/survey | Existing base working cost RM2,090.00; optional 10% contingency RM209.00; with contingency RM2,299.00. No customer markup. |
| S04 | Crossing bridge and permanent site entrance | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S04_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `CROSSING BRIDGE.pdf` rendered and visually inspected | Base working cost RM36,004.11; optional 10% contingency RM3,600.41; with contingency RM39,604.52. No customer markup. V1 undercost superseded. |
| S05 | Building substructure: footing, stump and ground beam | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S05_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `04-SURAU JERUSSALAM GROUND BEAM DETAIL 01.pdf`, `05-SURAU JERUSSALAM GROUND BEAM DETAIL 02.pdf` rendered and visually inspected | Base working cost RM31,089.07; optional 10% contingency RM3,108.91; with contingency RM34,197.98. No customer markup. |
| S06 | Under-slab plumbing, sewerage and drainage rough-in | START ALLOWED | - | NOT STARTED | Plumbing/sewerage drawings and foundation/slab interface drawings | Must avoid duplicate with S12/S21 and S07 slab works. |

## Next action

Proceed to S06 on working-cost drawing/spec path:

```text
S06_UnderSlabPlumbing_DrainageRoughIn_Takeoff_Audit_V1.txt
S06_BOQXLSM_PASTE_READY_V1.txt
15_SXX_COSTING_TRACKER_V15.md
```
