# Surau Nilai — SXX Costing Tracker V21

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/20_SXX_COSTING_TRACKER_V20.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V21 note

Owner clarified the strict target:

```text
100% is the target.
99.9% is not a pass.
GPT must know what the 100% target is before proceeding.
```

For this SXX workflow, the active 100% target is:

```text
Current BOQ cost basis complete for the SXX, using customer drawing/spec and/or authorised customer/README/owner accepted full allowance basis.
Customer selling price/margin is separate and not part of the current 100% target unless owner explicitly asks for selling price.
```

S08 status was checked from V20 before S09. S08 is complete for next SXX using `CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS`; S08 V2 is the active paste file.

S09 was checked against rendered:

```text
Roof Framing.pdf
Roof Framing 1.pdf
Surau Plan Roof Plan Bldg Tender_Constn.pdf
Surau Juasseh sections and elevations tender_constn 1.pdf
```

Repeated check confirmed:

```text
Insulated metal roofing (POWIN or equivalent) on GI steel battens and rafters.
All GI rafters and associated roof supporting purlins are plain GI and not coloured type.
Exposed mild steel beams and columns require anti-rust primer and three coats approved micaceous paint.
Roof has 30 degree and 45 degree slopes and multi-level hipped roof planes.
Rainwater goods are Everplast brand or architect approval.
S08 RC roof beams/columns are excluded.
S22 ground drainage/longkang is excluded.
```

## Current gate

```text
CURRENT ACTIVE SXX: S10
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
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S06 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S07 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S08 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S09 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S10 START ALLOWED: YES - CURRENT BOQ 100% COST BASIS PATH
```

## S09 files

```text
Repeated recheck file:
ActiveBOQ/Surau Nilai/BOQ/S09_RoofFraming_RoofCover_Recheck_Audit_V1.txt

Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S09_RoofFraming_RoofCover_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S09_BOQXLSM_PASTE_READY_V1.txt
```

Only `S09_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm` for S09.

## S09 cost summary

```text
Block 1 material: RM66,930.00
Block 2 labour:   RM2,840.00
Block 3 service:  RM16,020.00
Base working cost: RM85,790.00
Optional 10% contingency: RM8,579.00
Working cost with contingency: RM94,369.00
Customer selling price: NOT READY - markup/gross margin not applied
```

## S09 undercost / overprice / double-count check

```text
Drawing/spec scope included: YES - rendered roof framing, roof plan and section/elevation drawings used and rechecked
Missing required line check: PASS - GI roof frame, insulated metal roofing, flashing/capping, fascia/eaves trim, rainwater goods/RWDP, fasteners/sealants, protective paint, installation labour and roof access/lifting included
Undercost check: PASS - roof is not priced as sheet-only; authorised full allowance roof area 390m2 used, not minimum quantity
Overprice check: PASS WITH NOTE - S08 RC roof beams/columns excluded; S12 ceiling/finishes excluded; S22 ground drainage/longkang excluded; final water tank/plumbing connection excluded
Double-count check: PASS - excludes S08 structural RC, S12 finishing/internal items and S22 ground drainage
Markup check: PASS - no customer markup included
Allowance status: CLOSED FOR CURRENT BOQ COST - authorised drawing/README/owner full allowance is not random unsupported allowance
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
| S09 | Roof framing, roof structure and roof covering interface | COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS | `S09_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON CURRENT BOQ COST BASIS | `Roof Framing.pdf`, `Roof Framing 1.pdf`, `Surau Plan Roof Plan Bldg Tender_Constn.pdf`, `Surau Juasseh sections and elevations tender_constn 1.pdf` rendered and visually inspected | V1 base working cost RM85,790.00; optional 10% contingency RM8,579.00; with contingency RM94,369.00. No customer markup. |
| S10 | External walls / masonry / brickwork / wall structural infill | START ALLOWED | - | NOT STARTED | Floor plan, sections/elevations, wall/finishes drawings as needed | Must avoid duplicate with S05/S08 structure and S12 finishes. Include walling/infill only if shown/specifiable. |

## Next action

Proceed to S10 on current BOQ 100% cost basis path:

```text
S10_Walls_Masonry_Infill_Takeoff_Audit_V1.txt
S10_BOQXLSM_PASTE_READY_V1.txt
22_SXX_COSTING_TRACKER_V22.md
```
