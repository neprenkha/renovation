# Surau Nilai — SXX Costing Tracker V15

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/14_SXX_COSTING_TRACKER_V14.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V15 note

S06 has been completed on the owner-confirmed path:

```text
WORKING-COST DRAWING/SPEC BASIS
Margin/profit/customer selling price later
Undercost / overprice / double-count check recorded
```

## Current gate

```text
CURRENT ACTIVE SXX: S07
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
S06 WORKING-COST DRAWING/SPEC BASIS: COMPLETE
S06 BOQ.XLSM PASTE FILE: READY - USE V1
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S06 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S07 START ALLOWED: YES - WORKING-COST DRAWING/SPEC PATH
```

## S06 final files

```text
Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S06_UnderSlabPlumbing_DrainageRoughIn_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S06_BOQXLSM_PASTE_READY_V1.txt
```

Only `S06_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm` for S06.

## S06 cost summary

```text
Block 1 material: RM5,234.50
Block 2 labour:   RM3,460.00
Block 3 service:  RM1,100.00
Base working cost: RM9,794.50
Optional 10% contingency: RM979.45
Working cost with contingency: RM10,773.95
Customer selling price: NOT READY - markup/gross margin not applied
```

## S06 undercost / overprice / double-count check

```text
Drawing/spec scope included: YES - rendered sanitary plumbing and sewerage schematics used
Missing required line check: PASS - sewer pipe, waste pipe, ABS water supply pipe, traps, WC connectors, outlet rough-in, consumables, labour, backhoe and rough-in test included
Undercost check: PASS - fittings/solvent/sleeves/caps/testing protection added so pipe lengths are not undercosted alone
Overprice check: PASS WITH NOTE - roof tanks, pump, water meter, final taps, WC pans, basins and final fixture commissioning excluded to S12; external manholes/public sewer connection excluded to S21
Double-count check: PASS - excludes S05 substructure, S07 slab/hardcore/DPM/BRC, S12 final sanitary/plumbing fixtures, S21 external sewer and S22 stormwater drainage
Markup check: PASS - no customer markup included
Supplier/site verification items: exact pipe run lengths, trap model, pump/meter interface and final outlet positions may refine later
```

## SXX tracker

| SXX | Proposed scope | Working-cost status | BOQ.xlsm paste file | Drawing/spec status | Required source check | Notes |
|---|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | COMPLETE | `S01_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `Hoarding and Signboard 1.pdf`, site plan, survey | Existing base working cost RM8,750.00; optional 10% contingency RM875.00; with contingency RM9,625.00. No customer markup. |
| S02 | ESCP and temporary erosion/sediment control | COMPLETE | `S02_BOQXLSM_PASTE_READY_V2.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01ESCP-LP-01-S0-00.pdf` | Existing base working cost RM1,944.00; optional 10% contingency RM194.40; with contingency RM2,138.40. No customer markup. |
| S03 | Site clearing, earthwork, cut/fill and platform formation | COMPLETE | `S03_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01EW-CS-01-S0-00.pdf`, `SJ_01EW-DT-01-S0-00.pdf`, `SJ_01EW-LP-01-S0-00.pdf`, site plan/survey | Existing base working cost RM2,090.00; optional 10% contingency RM209.00; with contingency RM2,299.00. No customer markup. |
| S04 | Crossing bridge and permanent site entrance | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S04_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `CROSSING BRIDGE.pdf` rendered and visually inspected | Base working cost RM36,004.11; optional 10% contingency RM3,600.41; with contingency RM39,604.52. No customer markup. V1 undercost superseded. |
| S05 | Building substructure: footing, stump and ground beam | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S05_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `04-SURAU JERUSSALAM GROUND BEAM DETAIL 01.pdf`, `05-SURAU JERUSSALAM GROUND BEAM DETAIL 02.pdf` rendered and visually inspected | Base working cost RM31,089.07; optional 10% contingency RM3,108.91; with contingency RM34,197.98. No customer markup. |
| S06 | Under-slab plumbing, sewerage and drainage rough-in | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S06_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `Surau Sanitary Plumbing Schematic 1.pdf`, `Surau Sewerage Schematic 1.pdf` rendered and visually inspected | Base working cost RM9,794.50; optional 10% contingency RM979.45; with contingency RM10,773.95. No customer markup. |
| S07 | Ground floor slab, apron, steps and ramps | START ALLOWED | - | NOT STARTED | `02-SURAU JERUSSALAM SLAB SECTION 01.pdf`, `03-SURAU JERUSSALAM SLAB SECTION 02.pdf`, floor plan/site sections/source drawings as needed | Must avoid duplicate with S05 ground beams and S06 pipe rough-ins. Include slab build-up, BRC, DPM, hardcore if shown. |

## Next action

Proceed to S07 on working-cost drawing/spec path:

```text
S07_GroundFloorSlab_Apron_StepsRamps_Takeoff_Audit_V1.txt
S07_BOQXLSM_PASTE_READY_V1.txt
16_SXX_COSTING_TRACKER_V16.md
```
