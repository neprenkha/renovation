# Surau Nilai — SXX Costing Tracker V10

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/09_SXX_COSTING_TRACKER_V9.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

BOQ folder:

```text
ActiveBOQ/Surau Nilai/BOQ/
```

## V10 one-pass S04 note

S04 was created with one-pass preflight before output:

```text
ActiveBOQ/Surau Nilai/Takeoff_Work/S04_ONE_PASS_PREFLIGHT_V1.md
```

S03 remains complete and was not reopened.

## Current S04 final files

```text
Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S04_CrossingBridge_Entrance_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S04_BOQXLSM_PASTE_READY_V1.txt
```

Only `S04_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm`.

## Cross-SXX correction rule remains active

S04 is not hanging and may proceed to S05. If any later drawing/source/SXX proves overlap, double count, undercost or overprice, the affected SXX must be corrected immediately by creating the next cumulative version.

Watch points:

```text
S03 earthwork/backhoe vs S04 bridge/entrance excavation/backfill
S04 crusher run/access approach vs S24 road base/premix/parking works
S04 bridge/access concrete/rebar vs S05 building substructure
S04 entrance/access drainage interface vs S22 permanent drainage
```

## Current gate

```text
CURRENT ACTIVE SXX: S05
S01 COMPLETE FOR NEXT SXX: YES - MUKTAMAD WORKING-COST BASIS
S01 BOQ.XLSM PASTE FILE: READY
S02 COMPLETE FOR NEXT SXX: YES - 100% MUKTAMAD WORKING-COST BASIS
S02 BOQ.XLSM PASTE FILE: READY - USE V2
S03 COMPLETE FOR NEXT SXX: YES - 100% MUKTAMAD WORKING-COST BASIS
S03 BOQ.XLSM PASTE FILE: READY
S04 COMPLETE FOR NEXT SXX: YES - 100% MUKTAMAD WORKING-COST BASIS
S04 BOQ.XLSM PASTE FILE: READY
S01 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S02 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S03 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 START ALLOWED: YES
```

## SXX tracker

| SXX | Proposed scope | Status | Audit / takeoff file | BOQ.xlsm paste file | Source evidence | Notes |
|---|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | COMPLETE FOR NEXT SXX - MUKTAMAD WORKING-COST BASIS | `S01_Preliminaries_Takeoff_Block1-3_V4.txt` | `S01_BOQXLSM_PASTE_READY_V1.txt` | README, Materials/Labour, GPTEditable/Reference_Addendum, web/current market check, drawing/source register | Base working cost RM8,750.00; optional 10% contingency RM875.00; with contingency RM9,625.00. No customer markup. |
| S02 | ESCP and temporary erosion/sediment control | COMPLETE FOR NEXT SXX - 100% MUKTAMAD WORKING-COST BASIS | `S02_ESCP_Takeoff_Audit_V2.txt` + `Takeoff_Work/S02_ESCP_COMPLETION_CLOSURE_V2.md` | `S02_BOQXLSM_PASTE_READY_V2.txt` | `SJ_01ESCP-LP-01-S0-00.pdf`, Materials/Labour, GPTEditable/Reference_Addendum, web/current market check | Base working cost RM1,944.00; optional 10% contingency RM194.40; with contingency RM2,138.40. No customer markup. If later contradiction/double count appears, correct affected SXX immediately. |
| S03 | Site clearing, earthwork, cut/fill and platform formation | COMPLETE FOR NEXT SXX - 100% MUKTAMAD WORKING-COST BASIS | `S03_Earthwork_Takeoff_Audit_V1.txt` + `Takeoff_Work/S03_ONE_PASS_PREFLIGHT_V1.md` | `S03_BOQXLSM_PASTE_READY_V1.txt` | `SJ_01EW-CS-01-S0-00.pdf`, `SJ_01EW-DT-01-S0-00.pdf`, `SJ_01EW-LP-01-S0-00.pdf`, site plan/survey, Materials/Labour | Base working cost RM2,090.00; optional 10% contingency RM209.00; with contingency RM2,299.00. No customer markup. |
| S04 | Crossing bridge and permanent site entrance | COMPLETE FOR NEXT SXX - 100% MUKTAMAD WORKING-COST BASIS | `S04_CrossingBridge_Entrance_Takeoff_Audit_V1.txt` + `Takeoff_Work/S04_ONE_PASS_PREFLIGHT_V1.md` | `S04_BOQXLSM_PASTE_READY_V1.txt` | `CROSSING BRIDGE.pdf`, site plan/survey, Materials/Labour, GPTEditable/Reference_Addendum | Base working cost RM6,550.20; optional 10% contingency RM655.02; with contingency RM7,205.22. No customer markup. |
| S05 | Building substructure: footing, stump and ground beam | NOT STARTED | - | - | `04-SURAU JERUSSALAM GROUND BEAM DETAIL 01.pdf`, `05-SURAU JERUSSALAM GROUND BEAM DETAIL 02.pdf`, slab/section/source drawings as needed | S05 may start next; must produce both audit/reference and BOQ.xlsm paste-ready output. |
| S06 | Under-slab plumbing, sewerage and drainage rough-in | NOT STARTED | - | - | Plumbing/sewerage drawings pending deep-read | Must avoid duplicate with S12/S21. |
| S07 | Ground floor slab, apron, steps and ramps | NOT STARTED | - | - | Structural/architectural drawings pending deep-read | Must include slab build-up, BRC, DPM, hardcore if applicable. |
| S08 | RC columns, roof beams and internal roof beams | NOT STARTED | - | - | Structural drawings pending deep-read | Must include mark-by-mark structural takeoff. |
| S09 | Steel roof framing | NOT STARTED | - | - | Roof framing drawings pending deep-read | Must resolve duplicate/variant roof framing drawing if any. |
| S10 | Roof covering and rainwater goods | NOT STARTED | - | - | Roof/section/elevation drawings pending deep-read | Include gutter/downpipe/flashing if shown. |
| S11 | Masonry walls, brick screens and ventilation openings | NOT STARTED | - | - | Architectural drawings pending deep-read | W4-W6 and BS1 must not be treated as aluminium windows. |
| S12 | Internal plumbing, sanitary and ablution system | NOT STARTED | - | - | Sanitary plumbing schematic pending deep-read | Separate from under-slab rough-in. |
| S13 | Electrical, lighting, fans, power, earthing and ELV | NOT STARTED | - | - | Electrical drawing availability pending | May be reserved only with explicit reason; cannot be NIL if source/addendum can fill basis. |
| S14 | Internal/external plaster, render and skim coat | NOT STARTED | - | - | Architectural drawings pending deep-read | Surface areas required. |
| S15 | Waterproofing, screed and wet-area floor falls | NOT STARTED | - | - | Architectural/plumbing drawings pending deep-read | Wet-area scope required. |
| S16 | Floor and wall finishes | NOT STARTED | - | - | Architectural drawings pending deep-read | Finish schedule may be provisional only for real spec conflict; no blank rate lines. |
| S17 | Timber doors, frames and ironmongery | NOT STARTED | - | - | Door schedule + floor plan pending deep-read | D1/D3 counts must be verified. |
| S18 | Aluminium doors, windows, glass louvres and glazing | NOT STARTED | - | - | Door/window schedule + floor plan pending deep-read | D2/W1/W2/W3 counts must be verified. |
| S19 | Ceiling and access panels | NOT STARTED | - | - | Ceiling/RCP source if available | May be reserved only with explicit reason; cannot be NIL if source/addendum can fill basis. |
| S20 | Painting and architectural final fittings | NOT STARTED | - | - | Architectural drawings pending deep-read | Depends on plaster/wall/ceiling quantities. |
| S21 | External sewerage system | NOT STARTED | - | - | Sewerage schematic pending deep-read | Separate from stormwater drainage. |
| S22 | Permanent stormwater drainage | NOT STARTED | - | - | Road/drain drawings pending deep-read | Drains/catchpits/outfall required. |
| S23 | Permanent fencing and gates | NOT STARTED | - | - | Fence/gate drawing pending deep-read | Default in-house unless owner changes. |
| S24 | Road, parking, kerb, road base and premix | NOT STARTED | - | - | Road/drain/site drawings pending deep-read | Premix area must be measured, not residual lot area. |
| S25 | Road marking, parking marking and traffic signage | NOT STARTED | - | - | Road/parking drawings pending deep-read | Keep separate from premix package. |

## Per-SXX one-pass checklist

Before marking any SXX complete for next SXX, confirm:

- latest tracker was read;
- current active SXX is correct;
- previous SXX is closed for sequence;
- source drawing list is recorded;
- README - BOQ paste rules were followed;
- material/labour/root/addendum references were checked;
- cross-SXX duplicate risks were listed;
- audit/takeoff file exists if needed for review;
- BOQ.xlsm paste-ready file exists for owner paste;
- paste target headers are outside TSV data;
- SPEC uses `SXX!A:C` only;
- Block 1 uses `SXX!E:K` only;
- Block 2 uses `SXX!P:V` only;
- Block 3 uses `SXX!AA:AG` only;
- no formula columns or total columns are included in paste blocks;
- no audit-only columns are included in paste blocks;
- no required line is NIL/blank;
- markup status is stated in Note;
- if later SXX creates contradiction/double count/undercost/overprice, affected previous SXX is corrected before continuing.
