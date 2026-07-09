# Surau Nilai — SXX Costing Tracker V7

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/06_SXX_COSTING_TRACKER_V6.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

BOQ folder:

```text
ActiveBOQ/Surau Nilai/BOQ/
```

## V7 correction note

Owner asked for S02 to be scanned/check again against customer/spec source before moving to the next SXX.

S02 was previously marked complete too quickly. S02 is complete as a working-cost paste basis, but not yet 100% customer-spec scanned because the ESCP drawing still needs render/visual inspection.

## S02 current files

```text
Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S02_ESCP_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S02_BOQXLSM_PASTE_READY_V1.txt

Rescan gate note:
ActiveBOQ/Surau Nilai/Takeoff_Work/S02_ESCP_RESCAN_GATE_V1.md
```

The paste-ready file may be used as a working-cost paste file, but S02 must not be treated as 100% customer-spec complete until ESCP visual scan is cleared.

## Required S02 visual scan source

```text
ActiveBOQ/Surau Nilai/Drawing/SJ_01ESCP-LP-01-S0-00.pdf
```

Visual scan must confirm or correct:

- actual silt fence/perimeter sediment-control length;
- actual sandbag/check/inlet protection point count;
- whether temporary drain/check-dam items are shown;
- whether any item overlaps S01 hoarding or later permanent drainage scopes;
- whether the drawing contains notes/specs requiring a different ESCP method or quantity.

## Current gate

```text
CURRENT ACTIVE SXX: S02
S01 COMPLETE FOR NEXT SXX: YES - MUKTAMAD WORKING-COST BASIS
S01 BOQ.XLSM PASTE FILE: READY
S02 WORKING-COST BASIS: COMPLETE
S02 BOQ.XLSM PASTE FILE: READY FOR WORKING-COST PASTE
S02 CUSTOMER-SPEC SCAN: HOLD - VISUAL SCAN REQUIRED
S02 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S03 START ALLOWED: NO
NEXT ACTION: Render/visual-inspect SJ_01ESCP-LP-01-S0-00.pdf, then either clear S02 or create S02 V2 correction.
```

## SXX tracker

| SXX | Proposed scope | Status | Audit / takeoff file | BOQ.xlsm paste file | Source evidence | Notes |
|---|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | COMPLETE FOR NEXT SXX - MUKTAMAD WORKING-COST BASIS | `S01_Preliminaries_Takeoff_Block1-3_V4.txt` | `S01_BOQXLSM_PASTE_READY_V1.txt` | README, Materials/Labour, GPTEditable/Reference_Addendum, web/current market check, drawing/source register | Base working cost RM8,750.00; optional 10% contingency RM875.00; with contingency RM9,625.00. No customer markup. |
| S02 | ESCP and temporary erosion/sediment control | HOLD - VISUAL SCAN REQUIRED BEFORE 100% CUSTOMER-SPEC COMPLETE | `S02_ESCP_Takeoff_Audit_V1.txt` + `Takeoff_Work/S02_ESCP_RESCAN_GATE_V1.md` | `S02_BOQXLSM_PASTE_READY_V1.txt` | `SJ_01ESCP-LP-01-S0-00.pdf`, Materials/Labour, GPTEditable/Reference_Addendum, web/current market check | Working-cost basis RM1,944.00; optional 10% contingency RM194.40; with contingency RM2,138.40. Not cleared for S03 until visual scan confirms or corrects quantities/spec. |
| S03 | Site clearing, earthwork, cut/fill and platform formation | NOT ALLOWED YET | - | - | Earthwork drawing pending S03 takeoff | Start only after S02 visual scan gate is cleared. |
| S04 | Crossing bridge and permanent site entrance | NOT STARTED | - | - | Drawing pending deep-read | RC/bridge takeoff required. |
| S05 | Building substructure: footing, stump and ground beam | NOT STARTED | - | - | Structural drawings pending deep-read | Must include concrete, rebar, formwork, excavation. |
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

## Per-SXX visual scan checklist

Before marking any SXX 100% customer-spec complete:

- confirm all relevant source drawings were rendered or visually inspected;
- if a source cannot be rendered/read, mark `UNREADABLE / NEEDS REVIEW` and do not proceed as 100%;
- do not treat PDF existence, base64 fetch, filename match or working-cost default as a visual scan;
- confirm no overlap/double count with previous SXX;
- update affected SXX immediately if visual scan changes quantity, method or scope.
