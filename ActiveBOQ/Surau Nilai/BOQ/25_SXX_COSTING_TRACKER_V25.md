# Surau Nilai — SXX Costing Tracker V25

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/24_SXX_COSTING_TRACKER_V24.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V25 note — S11 strict 100 recheck after uploaded header

Owner uploaded/latest header checked:

```text
GPTRenovationHeader.txt
Generated MYT: 2026-07-10 07:00
```

Owner repeated the strict gate:

```text
Take off to next SXX is only allowed at 100%.
99.9% is not a pass.
```

For this SXX workflow, the active 100% target remains:

```text
Current BOQ cost basis complete for the SXX, using customer drawing/spec and/or authorised customer/README/owner accepted full allowance basis.
Customer selling price/margin is separate and not part of the current 100% target unless owner explicitly asks for selling price.
```

## S11 strict recheck file

```text
ActiveBOQ/Surau Nilai/BOQ/S11_Doors_Windows_Glazing_Openings_Strict100_Recheck_Audit_V2.txt
```

Decision:

```text
S11 STRICT 100% CURRENT BOQ COST BASIS: PASS
S11 ACTIVE AUDIT FILE: S11_Doors_Windows_Glazing_Openings_Takeoff_Audit_V3.txt
S11 ACTIVE PASTE FILE: S11_BOQXLSM_PASTE_READY_V2.txt
S11 ACTIVE ALUMINIUM/GLASS SCHEDULE: S11_AluminiumGlass_SpecSizeQuantity_Schedule_V2.txt
S12 START ALLOWED: YES
```

## Active S11 files

```text
Full aluminium/glass/spec schedule:
ActiveBOQ/Surau Nilai/BOQ/S11_AluminiumGlass_SpecSizeQuantity_Schedule_V2.txt

Strict recheck file:
ActiveBOQ/Surau Nilai/BOQ/S11_Doors_Windows_Glazing_Openings_Strict100_Recheck_Audit_V2.txt

Active audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S11_Doors_Windows_Glazing_Openings_Takeoff_Audit_V3.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S11_BOQXLSM_PASTE_READY_V2.txt
```

Do not use these S11 files as active paste/audit files:

```text
S11_Doors_Windows_Glazing_Openings_Takeoff_Audit_V1.txt
S11_Doors_Windows_Glazing_Openings_Takeoff_Audit_V2.txt
S11_BOQXLSM_PASTE_READY_V1.txt
```

## S11 final spec check

| Mark | Type | Size | Spec | Brand/system | Qty | Status |
|---|---|---:|---|---|---:|---|
| D1 | Solid timber door | 900W x 2400H | Solid timber door to detail, frame/ironmongery/finish allowance included | Not aluminium/glass | 4 nos | INCLUDED IN S11 |
| D2 | Aluminium sliding door | 2300W x 2400H | Powder coated aluminium frame, 10mm clear tempered glass, manufacturer specification | Brand not stated | 3 nos | INCLUDED IN S11, ACTUAL ALUMINIUM/GLASS PRICE TO BE REPLACED BY OWNER LATER |
| D3 | Solid timber door | 1000W x 2400H | Solid timber door to detail, frame/ironmongery/finish allowance included | Not aluminium/glass | 3 nos | INCLUDED IN S11 |
| W1 | Top hung aluminium window | 900W x 1200H | Powder coated aluminium frame, 8mm clear glass | Brand not stated | 2 nos | INCLUDED IN S11, ACTUAL ALUMINIUM/GLASS PRICE TO BE REPLACED BY OWNER LATER |
| W2 | Adjustable glass louvre | 2280W x 2400H | Tempered glass panels, adjustable glass louvre | Breezeway Altair | 5 nos | INCLUDED IN S11, ACTUAL ALUMINIUM/GLASS PRICE TO BE REPLACED BY OWNER LATER |
| W3 | Adjustable glass louvre | 750W x 2400H | Tempered glass panels, adjustable glass louvre | Breezeway Altair | 2 nos | INCLUDED IN S11, ACTUAL ALUMINIUM/GLASS PRICE TO BE REPLACED BY OWNER LATER |
| W4 | High-level opening | 2400W x 1250H | Lighting/ventilation opening only with no windows | Not applicable | 2 nos | NO S11 WINDOW COST |
| W5 | High-level opening | 1000W x 1250H | Lighting/ventilation opening only with no windows | Not applicable | 3 nos | NO S11 WINDOW COST |
| W6 | High-level opening | 1700W x 1250H | Lighting/ventilation opening only with no windows | Not applicable | 1 no | NO S11 WINDOW COST |
| BS1 | Brick screen ventilation opening | 850W x 2400H | Brick screen / ventilation opening by brick screen | Not aluminium/glass | 7 nos | EXCLUDED TO S10 BRICK SCREEN |

## S11 aluminium/glass actual-price-later schedule

These are the only S11 items for owner actual aluminium/glass pricing later:

| Mark | Pricing description | Qty | Total area |
|---|---|---:|---:|
| D2 | 2300W x 2400H powder coated aluminium sliding door with 10mm clear tempered glass, brand not stated, manufacturer specification, panel count not stated in drawing | 3 nos | 16.56 m2 |
| W1 | 900W x 1200H top hung powder coated aluminium window with 8mm clear glass, brand not stated | 2 nos | 2.16 m2 |
| W2 | 2280W x 2400H Breezeway Altair adjustable glass louvre with tempered glass panels | 5 nos | 27.36 m2 |
| W3 | 750W x 2400H Breezeway Altair adjustable glass louvre with tempered glass panels | 2 nos | 3.60 m2 |

## S11 cost summary

S11 total remains unchanged from V24 because the strict recheck did not change active rates/quantities:

```text
Block 1 material: RM43,606.80
Block 2 labour:   RM3,100.00
Block 3 service:  RM8,064.80
Base working cost: RM54,771.60
Optional 10% contingency: RM5,477.16
Working cost with contingency: RM60,248.76
Customer selling price: NOT READY - markup/gross margin not applied
```

## S11 strict gate checklist

```text
Drawing/spec source checked: PASS
Aluminium/glass schedule by mark: PASS
Size by mark: PASS
Quantity by mark: PASS
Brand/system checked: PASS
Glass thickness/type checked: PASS
Panel count: PASS WITH NOTE - D2 panel count not stated in drawing; no invented panel count
No-cost openings separated: PASS
BS1 duplicate prevention: PASS
S10 duplicate prevention: PASS
S12 duplicate prevention: PASS
Block 1 complete: PASS
Block 2 complete: PASS
Block 3 complete: PASS
Markup check: PASS
100% / 99.9% gate: PASS
```

## Header update decision

No new header update is required for this S11 recheck because the latest uploaded `GPTRenovationHeader.txt` already contains:

```text
13D Drawing-spec SXX completion gate
13E Authorised allowance / 100% current BOQ cost basis rule
13F Aluminium / Glass / Door-Window Spec Schedule Rule
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
S11 STRICT 100% CURRENT BOQ COST BASIS: PASS
S11 ACTIVE ALUMINIUM/GLASS SCHEDULE: USE V2
S11 ACTIVE AUDIT FILE: USE V3
S11 ACTIVE BOQ.XLSM PASTE FILE: USE V2
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
| S11 | Doors, windows, aluminium/glazing, louvres and ventilation/opening fixtures | STRICT 100% CURRENT BOQ COST BASIS PASS | `S11_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON CURRENT BOQ COST BASIS | `Surau Plan Roof Plan Bldg Tender_Constn.pdf`, `Surau Juasseh sections and elevations tender_constn 1.pdf`, `01-SURAU JERUSSALAM LP-R02 Layout1.pdf` rendered/text-extracted and visually inspected | Strict recheck V2 active. V3 audit active. Aluminium/glass spec schedule V2 required for actual price later. Base working cost RM54,771.60; optional 10% contingency RM5,477.16; with contingency RM60,248.76. No customer markup. |
| S12 | Internal plaster, ceiling, finishes, sanitary final fixtures and internal finish interface | START ALLOWED | - | NOT STARTED | Floor plan, finishes legend, sections/elevations, sanitary/plumbing schematic and relevant details as needed | Must avoid duplicate with S10 walling, S11 doors/windows and S06 rough-in. Include finishes/final fixtures only if shown/specifiable. |

## Next action

Proceed to S12 on current BOQ 100% cost basis path:

```text
S12_InternalFinishes_SanitaryFixtures_Takeoff_Audit_V1.txt
S12_BOQXLSM_PASTE_READY_V1.txt
26_SXX_COSTING_TRACKER_V26.md
```
