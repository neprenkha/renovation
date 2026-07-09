# Surau Nilai — SXX Costing Tracker V23

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/22_SXX_COSTING_TRACKER_V22.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V23 note

Owner repeated the strict gate:

```text
Take off to next SXX is only allowed at 100%.
99.9% is not a pass.
```

For this SXX workflow, the active 100% target is:

```text
Current BOQ cost basis complete for the SXX, using customer drawing/spec and/or authorised customer/README/owner accepted full allowance basis.
Customer selling price/margin is separate and not part of the current 100% target unless owner explicitly asks for selling price.
```

S11 was checked against rendered/text-extracted:

```text
Surau Plan Roof Plan Bldg Tender_Constn.pdf
Surau Juasseh sections and elevations tender_constn 1.pdf
01-SURAU JERUSSALAM LP-R02 Layout1.pdf
```

Repeated check confirmed:

```text
D1 qty 4: solid timber door 900x2400 to detail.
D2 qty 3: powder coated aluminium sliding door 2300x2400 with 10mm clear tempered glass.
D3 qty 3: solid timber door 1000x2400 to detail.
W1 qty 2: top hung powder coated aluminium window 900x1200 with 8mm clear glass.
W2 qty 5: Breezeway Altair adjustable glass louvres 2280x2400 with tempered glass panels.
W3 qty 2: Breezeway Altair adjustable glass louvres 750x2400 with tempered glass panels.
W4 qty 2, W5 qty 3 and W6 qty 1: high-level lighting/ventilation opening only with no windows; no S11 window supply charged.
BS1 qty 7: brick screen ventilation opening; excluded to S10 brick screen scope.
S10 masonry/opening formation excluded.
S12 plaster/paint/tile/final finishes excluded.
```

## Current gate

```text
CURRENT ACTIVE SXX: S12
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
S11 COMPLETE FOR NEXT SXX - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS
S11 BOQ.XLSM PASTE FILE: READY - USE V1
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S06 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S07 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S08 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S09 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S10 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S11 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S12 START ALLOWED: YES - CURRENT BOQ 100% COST BASIS PATH
```

## S11 files

```text
Repeated recheck file:
ActiveBOQ/Surau Nilai/BOQ/S11_Doors_Windows_Glazing_Openings_Recheck_Audit_V1.txt

Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S11_Doors_Windows_Glazing_Openings_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S11_BOQXLSM_PASTE_READY_V1.txt
```

Only `S11_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm` for S11.

## S11 cost summary

```text
Block 1 material: RM43,606.80
Block 2 labour:   RM3,100.00
Block 3 service:  RM8,064.80
Base working cost: RM54,771.60
Optional 10% contingency: RM5,477.16
Working cost with contingency: RM60,248.76
Customer selling price: NOT READY - markup/gross margin not applied
```

## S11 undercost / overprice / double-count check

```text
Drawing/spec scope included: YES - rendered/text-extracted floor plan, window schedule, door schedule, elevations/opening context and structural boundary layout used and rechecked
Missing required line check: PASS - solid timber doors, aluminium sliding doors with 10mm tempered glass, top hung aluminium windows with 8mm clear glass, Breezeway Altair adjustable glass louvres, ironmongery/sealant/flashing/fixing sundries, direct labour, specialist installation and opening access/protection included
Undercost check: PASS - S11 is not priced as door leaf/window glass only; frames/ironmongery/sundries/installation/access included
Overprice check: PASS WITH NOTE - W4/W5/W6 are not charged as windows; BS1 brick screens excluded to S10; S10 masonry/opening formation and S12 finishes excluded
Double-count check: PASS - excludes S10 masonry/brick screens/opening formation and S12 finishing
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
| S06 | Under-slab plumbing, sewerage and drainage rough-in | COMPLETE AFTER RECHECK - WORKING-COST DRAWING/SPEC BASIS | `S06_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `Surau Sanitary Plumbing Schematic 1.pdf`, `Surau Sewerage Schematic 1.pdf` rendered, visually inspected and text/word-position checked | V2 base working cost RM10,794.50; optional 10% contingency RM1,079.45; with contingency RM11,873.95. No customer markup. |
| S07 | Ground floor slab, apron, steps and ramps | COMPLETE AFTER RECHECK - WORKING-COST DRAWING/SPEC BASIS | `S07_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `02-SURAU JERUSSALAM SLAB SECTION 01.pdf`, `03-SURAU JERUSSALAM SLAB SECTION 02.pdf` rendered and visually inspected | Base working cost RM43,805.56; optional 10% contingency RM4,380.56; with contingency RM48,186.12. No customer markup. |
| S08 | Columns, RC frame/roof beams and superstructure structural RC | COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS | `S08_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON CURRENT BOQ COST BASIS | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `06-SURAU JURESSALAM ROOF BEAM DETAIL-R01 Model.pdf`, `07-SURAU JURESSALAM INT RF BEAM DETAIL-R01 Model.pdf` rendered and visually inspected | V2 base working cost RM26,180.76; optional 10% contingency RM2,618.08; with contingency RM28,798.84. No customer markup. |
| S09 | Roof framing, roof structure and roof covering interface | COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS | `S09_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON CURRENT BOQ COST BASIS | `Roof Framing.pdf`, `Roof Framing 1.pdf`, `Surau Plan Roof Plan Bldg Tender_Constn.pdf`, `Surau Juasseh sections and elevations tender_constn 1.pdf` rendered and visually inspected | V1 base working cost RM85,790.00; optional 10% contingency RM8,579.00; with contingency RM94,369.00. No customer markup. |
| S10 | External walls / masonry / brickwork / wall structural infill | COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS | `S10_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON CURRENT BOQ COST BASIS | `Surau Plan Roof Plan Bldg Tender_Constn.pdf`, `Surau Juasseh sections and elevations tender_constn 1.pdf`, `01-SURAU JERUSSALAM LP-R02 Layout1.pdf` rendered/text-extracted and visually inspected | V1 base working cost RM75,660.00; optional 10% contingency RM7,566.00; with contingency RM83,226.00. No customer markup. |
| S11 | Doors, windows, aluminium/glazing, louvres and ventilation/opening fixtures | COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS | `S11_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON CURRENT BOQ COST BASIS | `Surau Plan Roof Plan Bldg Tender_Constn.pdf`, `Surau Juasseh sections and elevations tender_constn 1.pdf`, `01-SURAU JERUSSALAM LP-R02 Layout1.pdf` rendered/text-extracted and visually inspected | V1 base working cost RM54,771.60; optional 10% contingency RM5,477.16; with contingency RM60,248.76. No customer markup. |
| S12 | Internal plaster, ceiling, finishes, sanitary final fixtures and internal finish interface | START ALLOWED | - | NOT STARTED | Floor plan, finishes legend, sections/elevations, sanitary/plumbing schematic and relevant details as needed | Must avoid duplicate with S10 walling, S11 doors/windows and S06 rough-in. Include finishes/final fixtures only if shown/specifiable. |

## Next action

Proceed to S12 on current BOQ 100% cost basis path:

```text
S12_InternalFinishes_SanitaryFixtures_Takeoff_Audit_V1.txt
S12_BOQXLSM_PASTE_READY_V1.txt
24_SXX_COSTING_TRACKER_V24.md
```
