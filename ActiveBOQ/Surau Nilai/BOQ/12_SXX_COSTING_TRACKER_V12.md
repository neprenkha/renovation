# Surau Nilai — SXX Costing Tracker V12

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/11_SXX_COSTING_TRACKER_V11.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

BOQ folder:

```text
ActiveBOQ/Surau Nilai/BOQ/
```

## V12 correction note

Owner corrected GPT that S04 must be 100% according to customer drawing/spec, not a random or broad working-cost allowance.

That same drawing-spec gate must be applied retrospectively to S01-S03.

Existing S01-S04 paste files are kept as working-cost paste files only until each relevant source drawing is rendered/visually inspected or reliably extracted and quantities are confirmed/corrected.

## Gate definition

```text
WORKING-COST BASIS COMPLETE = cost basis exists and no required cost line is blank
BOQ.XLSM PASTE READY = workbook input file exists
DRAWING-SPEC MEASURED COMPLETE = drawing/source has been rendered/visually inspected or reliably extracted and quantities are proved against it
CUSTOMER SELLING PRICE COMPLETE = markup/gross margin has been applied and accepted separately
```

## Current gate

```text
CURRENT ACTIVE SXX: S04
S01 WORKING-COST BASIS: COMPLETE
S01 BOQ.XLSM PASTE FILE: READY - WORKING-COST ONLY
S01 DRAWING-SPEC MEASURED COMPLETE: NO - HOLD FOR RESCAN
S02 WORKING-COST BASIS: COMPLETE
S02 BOQ.XLSM PASTE FILE: READY - WORKING-COST ONLY
S02 DRAWING-SPEC MEASURED COMPLETE: NO - HOLD FOR RESCAN
S03 WORKING-COST BASIS: COMPLETE
S03 BOQ.XLSM PASTE FILE: READY - WORKING-COST ONLY
S03 DRAWING-SPEC MEASURED COMPLETE: NO - HOLD FOR RESCAN
S04 WORKING-COST BASIS: EXISTS
S04 BOQ.XLSM PASTE FILE: EXISTS - WORKING-COST ONLY
S04 DRAWING-SPEC MEASURED COMPLETE: NO - HOLD
S05 START ALLOWED: NO
NEXT ACTION: clear S04 drawing-spec gate first by rendering/inspecting CROSSING BRIDGE.pdf and creating S04 measured V2, or keep HOLD if unreadable.
```

## Rescan register

```text
ActiveBOQ/Surau Nilai/Takeoff_Work/S01-S04_DRAWING_SPEC_RESCAN_REGISTER_V1.md
```

## SXX tracker

| SXX | Proposed scope | Working-cost status | BOQ.xlsm paste file | Drawing-spec measured status | Required source check | Notes |
|---|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | COMPLETE | `S01_BOQXLSM_PASTE_READY_V1.txt` working-cost only | HOLD - DRAWING SPEC VERIFICATION REQUIRED | `Hoarding and Signboard 1.pdf`, `Surau Site Plan Tender_Constn.pdf`, `Survey Tapak Surau Juassewh Sentosa.pdf` | Base working cost RM8,750.00; optional 10% contingency RM875.00; with contingency RM9,625.00. No customer markup. Not confirmed as drawing-spec measured. |
| S02 | ESCP and temporary erosion/sediment control | COMPLETE | `S02_BOQXLSM_PASTE_READY_V2.txt` working-cost only | HOLD - DRAWING SPEC VERIFICATION REQUIRED | `SJ_01ESCP-LP-01-S0-00.pdf` | Base working cost RM1,944.00; optional 10% contingency RM194.40; with contingency RM2,138.40. No customer markup. Not confirmed as drawing-spec measured. |
| S03 | Site clearing, earthwork, cut/fill and platform formation | COMPLETE | `S03_BOQXLSM_PASTE_READY_V1.txt` working-cost only | HOLD - DRAWING SPEC VERIFICATION REQUIRED | `SJ_01EW-CS-01-S0-00.pdf`, `SJ_01EW-DT-01-S0-00.pdf`, `SJ_01EW-LP-01-S0-00.pdf`, site plan/survey as needed | Base working cost RM2,090.00; optional 10% contingency RM209.00; with contingency RM2,299.00. No customer markup. Not confirmed as drawing-spec measured. |
| S04 | Crossing bridge and permanent site entrance | EXISTS | `S04_BOQXLSM_PASTE_READY_V1.txt` working-cost only | HOLD - DRAWING SPEC VERIFICATION REQUIRED | `CROSSING BRIDGE.pdf`, site plan/survey as needed | S04 V1 base working cost RM6,550.20; optional 10% contingency RM655.02; with contingency RM7,205.22. Not accepted as 100% drawing-spec complete until `CROSSING BRIDGE.pdf` is rendered/verified and S04 V2 is created or V1 is proven. |
| S05 | Building substructure: footing, stump and ground beam | NOT ALLOWED YET | - | NOT STARTED | `04-SURAU JERUSSALAM GROUND BEAM DETAIL 01.pdf`, `05-SURAU JERUSSALAM GROUND BEAM DETAIL 02.pdf`, slab/section/source drawings as needed | Start only after S04 drawing-spec gate is cleared. |

## Correction rule

Do not call any S01-S04 file `100% drawing-spec complete` unless the required source drawings are actually rendered/visually inspected or reliably extracted and quantities are confirmed.

Working-cost paste files may still be used for internal cost planning, but must be labelled `WORKING-COST ONLY` until drawing-spec measured verification is complete.
