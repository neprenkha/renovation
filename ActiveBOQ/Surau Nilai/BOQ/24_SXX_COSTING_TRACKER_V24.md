# Surau Nilai — SXX Costing Tracker V24

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/23_SXX_COSTING_TRACKER_V23.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V24 correction note

Owner corrected a permanent rule after S11:

```text
If there is aluminium/glass work, GPT must extract the complete spec, size, quantity and brand/system if any.
Owner will calculate/replace actual aluminium/glass price later.
Different aluminium/glass specs must be separated.
Example: 10ftW x 8ftH 3 panel powder coated frame 8mm glass sliding door - 10 nos.
```

This is now recorded as a header amendment:

```text
GPTEditable/GPT_Header_Amendment_Aluminium_Glass_SpecSchedule_20260710.md
```

Owner local header replacement generated in chat:

```text
GPTRenovationHeader_UPDATED_20260710_0700.txt
```

## Active 100% target

```text
Current BOQ cost basis complete for the SXX, using customer drawing/spec and/or authorised customer/README/owner accepted full allowance basis.
Customer selling price/margin is separate and not part of the current 100% target unless owner explicitly asks for selling price.
```

## S11 corrected active files

```text
Full aluminium/glass/spec schedule:
ActiveBOQ/Surau Nilai/BOQ/S11_AluminiumGlass_SpecSizeQuantity_Schedule_V2.txt

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

V2 paste-ready is required because aluminium/glass items must be split by spec/size/quantity for owner actual price later.

## S11 aluminium/glass/spec schedule

| Mark | Item type | Drawing size mm | Approx size ft | Panel/leaf basis | Frame / finish | Glass spec | Brand / system | Qty | Total area m2 | Pricing status |
|---|---|---:|---:|---|---|---|---|---:|---:|---|
| D2 | Sliding door | 2300W x 2400H | 7.55ftW x 7.87ftH | Panel count not stated in drawing - supplier/owner actual price basis | Powder coated aluminium frame | 10mm clear tempered glass | Brand not stated; manufacturer specification stated | 3 nos | 16.56 | ACTUAL ALUMINIUM/GLASS PRICE TO BE REPLACED BY OWNER LATER |
| W1 | Top hung window | 900W x 1200H | 2.95ftW x 3.94ftH | Top hung sash basis; exact sash split not stated | Powder coated aluminium framed window | 8mm clear glass | Brand not stated | 2 nos | 2.16 | ACTUAL ALUMINIUM/GLASS PRICE TO BE REPLACED BY OWNER LATER |
| W2 | Adjustable glass louvre | 2280W x 2400H | 7.48ftW x 7.87ftH | Adjustable glass louvre panels | Louvre framing/system to manufacturer detail | Tempered glass panels | Breezeway Altair | 5 nos | 27.36 | ACTUAL ALUMINIUM/GLASS PRICE TO BE REPLACED BY OWNER LATER |
| W3 | Adjustable glass louvre | 750W x 2400H | 2.46ftW x 7.87ftH | Adjustable glass louvre panels | Louvre framing/system to manufacturer detail | Tempered glass panels | Breezeway Altair | 2 nos | 3.60 | ACTUAL ALUMINIUM/GLASS PRICE TO BE REPLACED BY OWNER LATER |

Non-priced / excluded opening records:

| Mark | Drawing size mm | Approx size ft | Qty | Status | Reason |
|---|---:|---:|---:|---|---|
| W4 | 2400W x 1250H | 7.87ftW x 4.10ftH | 2 nos | NO S11 WINDOW COST | High-level lighting/ventilation opening only with no windows. |
| W5 | 1000W x 1250H | 3.28ftW x 4.10ftH | 3 nos | NO S11 WINDOW COST | High-level lighting/ventilation opening only with no windows. |
| W6 | 1700W x 1250H | 5.58ftW x 4.10ftH | 1 no | NO S11 WINDOW COST | High-level lighting/ventilation opening only with no windows. |
| BS1 | 850W x 2400H | 2.79ftW x 7.87ftH | 7 nos | EXCLUDED TO S10 | Brick screen ventilation opening already included under S10. |

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
S11 ALUMINIUM/GLASS SPEC-SIZE-QUANTITY SCHEDULE: READY - USE V2
S11 BOQ.XLSM PASTE FILE: READY - USE V2
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

## S11 cost summary

S11 total remains unchanged from V1 because V2/V3 split the aluminium/glass schedule without changing the interim working rates:

```text
Block 1 material: RM43,606.80
Block 2 labour:   RM3,100.00
Block 3 service:  RM8,064.80
Base working cost: RM54,771.60
Optional 10% contingency: RM5,477.16
Working cost with contingency: RM60,248.76
Customer selling price: NOT READY - markup/gross margin not applied
```

## S11 updated undercost / overprice / double-count check

```text
Drawing/spec scope included: YES - rendered/text-extracted floor plan, window schedule, door schedule, elevations/opening context and structural boundary layout used and rechecked
Missing required line check: PASS - solid timber doors, D2 aluminium sliding door, W1 top hung aluminium window, W2/W3 Breezeway Altair adjustable louvres, ironmongery/sealant/flashing/fixing sundries, direct labour, specialist installation and opening access/protection included
Aluminium/glass spec schedule check: PASS - D2/W1/W2/W3 split by mark, size, glass thickness, brand/system and quantity for owner actual price later
No-cost opening check: PASS - W4/W5/W6 are no-cost openings, not priced as windows
BS1 duplicate check: PASS - excluded to S10 brick screen scope
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
| S11 | Doors, windows, aluminium/glazing, louvres and ventilation/opening fixtures | COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS | `S11_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON CURRENT BOQ COST BASIS | `Surau Plan Roof Plan Bldg Tender_Constn.pdf`, `Surau Juasseh sections and elevations tender_constn 1.pdf`, `01-SURAU JERUSSALAM LP-R02 Layout1.pdf` rendered/text-extracted and visually inspected | V3 audit active. Aluminium/glass spec schedule V2 required for actual price later. Base working cost RM54,771.60; optional 10% contingency RM5,477.16; with contingency RM60,248.76. No customer markup. |
| S12 | Internal plaster, ceiling, finishes, sanitary final fixtures and internal finish interface | START ALLOWED | - | NOT STARTED | Floor plan, finishes legend, sections/elevations, sanitary/plumbing schematic and relevant details as needed | Must avoid duplicate with S10 walling, S11 doors/windows and S06 rough-in. Include finishes/final fixtures only if shown/specifiable. |

## Next action

Proceed to S12 on current BOQ 100% cost basis path:

```text
S12_InternalFinishes_SanitaryFixtures_Takeoff_Audit_V1.txt
S12_BOQXLSM_PASTE_READY_V1.txt
25_SXX_COSTING_TRACKER_V25.md
```
