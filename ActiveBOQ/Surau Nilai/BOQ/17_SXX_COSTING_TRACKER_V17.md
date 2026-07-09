# Surau Nilai — SXX Costing Tracker V17

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/16_SXX_COSTING_TRACKER_V16.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V17 note

Owner requested repeated careful review of S07 before continuing to S08.

S07 was checked against rendered:

```text
01-SURAU JERUSSALAM LP-R02 Layout1.pdf
02-SURAU JERUSSALAM SLAB SECTION 01.pdf
03-SURAU JERUSSALAM SLAB SECTION 02.pdf
```

Repeated check confirmed:

```text
Non-suspended slab detail: 150mm concrete, BRC A8 bottom, polythene sheet/DPM, crusher run/hardcore, 50mm lean concrete where shown.
Slab cut sections: 150mm slab, BRC A8 bottom and BRC B5 top strip zones.
Typical apron detail: 100mm concrete apron, wire mesh A6 and 150mm hardcore.
Perimeter drain shown near apron detail is excluded to S22 drainage.
Ground beams are excluded to S05 and under-slab pipe rough-ins are excluded to S06.
```

## Current gate

```text
CURRENT ACTIVE SXX: S08
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
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S06 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S07 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S08 START ALLOWED: YES - WORKING-COST DRAWING/SPEC PATH
```

## S07 files

```text
Repeated recheck file:
ActiveBOQ/Surau Nilai/BOQ/S07_GroundFloorSlab_Apron_StepsRamps_Recheck_Audit_V1.txt

Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S07_GroundFloorSlab_Apron_StepsRamps_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S07_BOQXLSM_PASTE_READY_V1.txt
```

Only `S07_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm` for S07.

## S07 cost summary

```text
Block 1 material: RM35,105.56
Block 2 labour:   RM6,650.00
Block 3 service:  RM2,050.00
Base working cost: RM43,805.56
Optional 10% contingency: RM4,380.56
Working cost with contingency: RM48,186.12
Customer selling price: NOT READY - markup/gross margin not applied
```

## S07 undercost / overprice / double-count check

```text
Drawing/spec scope included: YES - rendered layout/slab section drawings used and rechecked
Missing required line check: PASS - G25 slab/apron concrete, G15 lean concrete, crusher run/hardcore, BRC A8, BRC B5 top strip, BRC A6 apron mesh, DPM, edge/step formwork, slab sundries, labour, concrete placing and equipment included
Undercost check: PASS - slab is not priced as concrete-only; BRC/DPM/hardcore/lean/sundries/labour/equipment included
Overprice check: PASS WITH NOTE - ground beams/footings/stumps excluded to S05; plumbing rough-ins excluded to S06; perimeter drain excluded to S22; BRC B5 measured as strip allowance, not full double mesh
Double-count check: PASS - excludes S05 substructure, S06 pipe rough-ins, S08 columns/roof beams, S12 finishes/final fixtures, S21 sewer external, S22 drainage and S24 road/premix
Markup check: PASS - no customer markup included
Supplier/site verification items: exact mesh supplier sizing/lapping, final slab edge set-out and actual pour/access method may refine later
```

## SXX tracker

| SXX | Proposed scope | Working-cost status | BOQ.xlsm paste file | Drawing/spec status | Required source check | Notes |
|---|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | COMPLETE | `S01_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `Hoarding and Signboard 1.pdf`, site plan, survey | Existing base working cost RM8,750.00; optional 10% contingency RM875.00; with contingency RM9,625.00. No customer markup. |
| S02 | ESCP and temporary erosion/sediment control | COMPLETE | `S02_BOQXLSM_PASTE_READY_V2.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01ESCP-LP-01-S0-00.pdf` | Existing base working cost RM1,944.00; optional 10% contingency RM194.40; with contingency RM2,138.40. No customer markup. |
| S03 | Site clearing, earthwork, cut/fill and platform formation | COMPLETE | `S03_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01EW-CS-01-S0-00.pdf`, `SJ_01EW-DT-01-S0-00.pdf`, `SJ_01EW-LP-01-S0-00.pdf`, site plan/survey | Existing base working cost RM2,090.00; optional 10% contingency RM209.00; with contingency RM2,299.00. No customer markup. |
| S04 | Crossing bridge and permanent site entrance | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S04_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `CROSSING BRIDGE.pdf` rendered and visually inspected | Base working cost RM36,004.11; optional 10% contingency RM3,600.41; with contingency RM39,604.52. No customer markup. V1 undercost superseded. |
| S05 | Building substructure: footing, stump and ground beam | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S05_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `04-SURAU JERUSSALAM GROUND BEAM DETAIL 01.pdf`, `05-SURAU JERUSSALAM GROUND BEAM DETAIL 02.pdf` rendered and visually inspected | Base working cost RM31,089.07; optional 10% contingency RM3,108.91; with contingency RM34,197.98. No customer markup. |
| S06 | Under-slab plumbing, sewerage and drainage rough-in | COMPLETE AFTER RECHECK - WORKING-COST DRAWING/SPEC BASIS | `S06_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `Surau Sanitary Plumbing Schematic 1.pdf`, `Surau Sewerage Schematic 1.pdf` rendered, visually inspected and text/word-position checked | V2 base working cost RM10,794.50; optional 10% contingency RM1,079.45; with contingency RM11,873.95. No customer markup. V1 undercount superseded. |
| S07 | Ground floor slab, apron, steps and ramps | COMPLETE AFTER RECHECK - WORKING-COST DRAWING/SPEC BASIS | `S07_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `02-SURAU JERUSSALAM SLAB SECTION 01.pdf`, `03-SURAU JERUSSALAM SLAB SECTION 02.pdf` rendered and visually inspected | Base working cost RM43,805.56; optional 10% contingency RM4,380.56; with contingency RM48,186.12. No customer markup. |
| S08 | Columns, RC frame/roof beams and superstructure structural RC | START ALLOWED | - | NOT STARTED | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `06-SURAU JURESSALAM ROOF BEAM DETAIL-R01 Model.pdf`, `07-SURAU JURESSALAM INT RF BEAM DETAIL-R01 Model.pdf`, sections/elevations if needed | Must avoid duplicate with S05 stump/ground beam and S07 slab. Include columns/upper RC beams only if shown. |

## Next action

Proceed to S08 on working-cost drawing/spec path:

```text
S08_RCFrame_Columns_RoofBeams_Takeoff_Audit_V1.txt
S08_BOQXLSM_PASTE_READY_V1.txt
18_SXX_COSTING_TRACKER_V18.md
```
