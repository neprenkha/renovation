# Surau Nilai — SXX Costing Tracker V20

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/19_SXX_COSTING_TRACKER_V19.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V20 correction note

Owner corrected the S08 strict hold interpretation:

```text
If customer/drawing/README/owner gives an allowance or accepted working basis, use that allowance.
The requirement is not to use the minimum quantity.
Use the customer/authority-derived allowance so excess risk is already costed.
Do not treat an authorised allowance as a failure merely because it is called allowance.
```

This correction supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/S08_STRICT_100_PERCENT_GATE_REVIEW_V2.md
ActiveBOQ/Surau Nilai/BOQ/19_SXX_COSTING_TRACKER_V19.md
```

## README basis

`README - BOQ.txt` is an authoritative source for the workbook workflow. It allows standalone/full purchase/full allowance/already-rounded quantities to be used as final Usage Qty with Wastage/Buffer = 0.

Therefore S08 V2 now uses:

```text
CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS - CLOSED FOR CURRENT BOQ COST
```

instead of treating all allowance wording as a failure.

## Current gate

```text
CURRENT ACTIVE SXX: S09
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
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S06 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S07 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S08 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S09 START ALLOWED: YES - WORKING-COST DRAWING/SPEC PATH
```

## S08 corrected files

```text
Correction note:
ActiveBOQ/Surau Nilai/BOQ/S08_ALLOWANCE_AUTHORITY_CORRECTION_V3.md

Corrected audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S08_RCFrame_Columns_RoofBeams_Takeoff_Audit_V2.txt

Corrected owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S08_BOQXLSM_PASTE_READY_V2.txt
```

Only `S08_BOQXLSM_PASTE_READY_V2.txt` should be copied into `*BOQ.xlsm` for S08. Do not use S08 V1 for current paste.

## S08 V2 cost summary

```text
Block 1 material: RM17,740.76
Block 2 labour:   RM5,680.00
Block 3 service:  RM2,760.00
Base working cost: RM26,180.76
Optional 10% contingency: RM2,618.08
Working cost with contingency: RM28,798.84
Customer selling price: NOT READY - markup/gross margin not applied
```

## S08 V2 undercost / overprice / double-count check

```text
Drawing/spec scope included: YES - rendered layout, RF roof beam detail and internal roof beam detail drawings used and rechecked
Missing required line check: PASS - G25 concrete, reinforcement, formwork, labour, concrete placing, scaffolding bays and jack/U-head support included
Undercost check: PASS - S08 is not priced as minimum quantity; customer/README accepted full allowance basis is used
Overprice check: PASS WITH NOTE - S05 footings/stumps/ground beams excluded; S07 slab/apron excluded; S09 roof framing/roof covering excluded
Double-count check: PASS - excludes S05 substructure, S07 slab/apron, S09 roof framing/cover, S12 finishes and later services
Markup check: PASS - no customer markup included
Allowance status: CLOSED FOR CURRENT BOQ COST - authorised allowance is not treated as random unsupported allowance
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
| S08 | Columns, RC frame/roof beams and superstructure structural RC | COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS | `S08_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON CURRENT BOQ COST BASIS | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `06-SURAU JURESSALAM ROOF BEAM DETAIL-R01 Model.pdf`, `07-SURAU JURESSALAM INT RF BEAM DETAIL-R01 Model.pdf` rendered and visually inspected | V2 base working cost RM26,180.76; optional 10% contingency RM2,618.08; with contingency RM28,798.84. No customer markup. |
| S09 | Roof framing, roof structure and roof covering interface | START ALLOWED | - | NOT STARTED | `Roof Framing 1.pdf`, `Roof Framing.pdf`, roof layout/source drawings as needed | Must avoid duplicate with S08 RC roof beams. Include steel/timber roof frame, battens, roofing sheets/tiles and accessories only if shown/specifiable. |

## Next action

Proceed to S09 on working-cost drawing/spec path:

```text
S09_RoofFraming_RoofCover_Takeoff_Audit_V1.txt
S09_BOQXLSM_PASTE_READY_V1.txt
21_SXX_COSTING_TRACKER_V21.md
```
