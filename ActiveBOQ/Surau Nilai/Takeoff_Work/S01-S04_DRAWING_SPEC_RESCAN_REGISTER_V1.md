# Surau Nilai — S01-S04 Drawing-Spec Rescan Register V1

## Reason

Owner corrected GPT that S04 must be 100% according to customer drawing/spec, not a random or broad working-cost allowance. The same check must be applied retrospectively to S01-S03.

## Gate separation

Every SXX must separate these states:

```text
WORKING-COST BASIS COMPLETE
BOQ.XLSM PASTE READY
DRAWING-SPEC MEASURED COMPLETE
CUSTOMER SELLING PRICE COMPLETE
```

## Current retrospective status

| SXX | Existing working-cost / paste status | Drawing-spec measured status | Required source check |
|---|---|---|---|
| S01 | Working-cost basis and BOQ.xlsm paste file exist | HOLD - drawing-spec verification required | `Hoarding and Signboard 1.pdf`, `Surau Site Plan Tender_Constn.pdf`, `Survey Tapak Surau Juassewh Sentosa.pdf` |
| S02 | Working-cost basis and BOQ.xlsm paste file exist | HOLD - drawing-spec verification required | `SJ_01ESCP-LP-01-S0-00.pdf` |
| S03 | Working-cost basis and BOQ.xlsm paste file exist | HOLD - drawing-spec verification required | `SJ_01EW-CS-01-S0-00.pdf`, `SJ_01EW-DT-01-S0-00.pdf`, `SJ_01EW-LP-01-S0-00.pdf`, site plan/survey as needed |
| S04 | Working-cost basis and BOQ.xlsm paste file exist | HOLD - drawing-spec verification required | `CROSSING BRIDGE.pdf`, site plan/survey as needed |

## What remains usable

Existing S01-S04 paste files may remain usable only as working-cost workbook input:

```text
S01_BOQXLSM_PASTE_READY_V1.txt
S02_BOQXLSM_PASTE_READY_V2.txt
S03_BOQXLSM_PASTE_READY_V1.txt
S04_BOQXLSM_PASTE_READY_V1.txt
```

They must not be described as 100% drawing-spec measured output until the listed source drawings are rendered/visually inspected or otherwise reliably extracted and the quantities are confirmed or corrected.

## Required correction path

For each affected SXX, do one of these:

1. render/read the relevant source drawing, prove the current quantities are correct, and create a measured confirmation file; or
2. create the next cumulative measured correction version:

```text
SXX_*_Takeoff_Audit_V2.txt
SXX_BOQXLSM_PASTE_READY_V2.txt
```

For S02 already using V2, the next correction would be V3 if drawing-spec quantities change.

## Stop rule

Do not start S05 as drawing-spec sequence while S04 is still `HOLD - DRAWING SPEC VERIFICATION REQUIRED`.
