# Surau Nilai — S04 Drawing-Spec Rescan Gate V2

## Owner correction

Owner corrected GPT: S04 must be 100% according to the customer drawing/spec, not a random or broad working-cost allowance.

## Current S04 status

Existing S04 files:

```text
ActiveBOQ/Surau Nilai/BOQ/S04_CrossingBridge_Entrance_Takeoff_Audit_V1.txt
ActiveBOQ/Surau Nilai/BOQ/S04_BOQXLSM_PASTE_READY_V1.txt
```

Decision:

```text
S04 WORKING-COST BASIS: EXISTS
S04 BOQ.XLSM PASTE FILE: EXISTS
S04 DRAWING-SPEC MEASURED COMPLETE: NO
S04 100% CUSTOMER-SPEC COMPLETE: NO
S05 START: NOT ALLOWED UNTIL S04 DRAWING-SPEC VERIFICATION IS CLEARED
```

## Exact block

`CROSSING BRIDGE.pdf` exists in GitHub and was fetched as binary/base64 source.

```text
ActiveBOQ/Surau Nilai/Drawing/CROSSING BRIDGE.pdf
Blob SHA: fc6723eb5dd6b70c697cc69a3577a4a3946ba00c
```

However, this session/tool path did not successfully render or visually inspect the PDF drawing. Therefore S04 V1 cannot be claimed as a 100% drawing-spec measured takeoff.

## Why S04 V1 is not enough for owner requirement

S04 V1 used current working-cost locked quantities:

```text
Ready Mix Concrete G25: 3.20 m3 + 5% wastage
Reinforcement steel: 320 kg + 5% wastage
Formwork material: 22 m2 + 10% wastage
Crusher Run: 1 trip
Skilled worker: 48 MH
General helper: 32 MH
Backhoe hire: 1 day
```

Those quantities may be usable as working-cost placeholders, but they are not proven as drawing-derived quantities from `CROSSING BRIDGE.pdf`.

## Required S04 verification before S05

Render/visual-inspect or otherwise reliably extract `CROSSING BRIDGE.pdf`, then confirm or correct:

- bridge/access location and whether it belongs fully to S04;
- plan dimensions/length/width/thickness;
- concrete grade and concrete volume;
- reinforcement/bar schedule or reinforcement allowance;
- formwork area;
- approach/base/crusher run requirement;
- excavation/backfill or backhoe requirement;
- interface with S03 earthwork, S05 substructure, S22 drainage and S24 road/premix.

## Next allowed actions

Either:

1. render/read `CROSSING BRIDGE.pdf`, create `S04_CrossingBridge_Entrance_Takeoff_Audit_V2.txt` and `S04_BOQXLSM_PASTE_READY_V2.txt` with measured drawing-spec quantities, then update tracker; or
2. if rendering remains unavailable, keep S04 as HOLD and request owner-provided screenshot/export/dimensions of the crossing bridge drawing before S05.

## Governance note

Do not mark S04 as 100% drawing-spec complete from assumed quantities. Working-cost complete and drawing-spec measured complete are separate gates.
