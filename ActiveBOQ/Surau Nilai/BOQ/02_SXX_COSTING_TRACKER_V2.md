# Surau Nilai — SXX Costing Tracker V2

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/01_SXX_COSTING_TRACKER_V1.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

BOQ folder:

```text
ActiveBOQ/Surau Nilai/BOQ/
```

## Rule

Cost one SXX at a time. Do not start the next SXX costing file until the current SXX is marked `COMPLETE FOR NEXT SXX` or `RESERVED WITH REASON`.

## Reference files

Read-only root references:

```text
README - BOQ.txt
1.2 Materials.txt
1.3 Labour.txt
```

Read-only Surau Nilai source folder:

```text
ActiveBOQ/Surau Nilai/Drawing/
```

## Required file pattern

Use cumulative versioned files.

Suggested naming:

```text
S01_<short_scope>_Costing_V1.md
S02_<short_scope>_Costing_V1.md
...
SXX_<short_scope>_Costing_V1.md
Surau_Nilai_Overall_Cost_Summary_V1.md
```

If an SXX requires correction later, create V2 with V1 useful/current content included. Do not edit/delete V1.

## V2 update note

S01 has been started as:

```text
ActiveBOQ/Surau Nilai/BOQ/S01_Preliminaries_Costing_V1.md
```

S01 is **not complete** and does **not** allow S02 yet. Current priced amount is only partial Block 2 labour working cost. Hoarding, signboard, mobilisation, temporary utilities, safety/protection/admin allowance and project duration remain unresolved.

## SXX tracker

| SXX | Proposed scope | Status | Cost file | Source evidence | Notes |
|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | IN PROGRESS | `S01_Preliminaries_Costing_V1.md` | Header, README, Materials/Labour, control/tracker checked; drawing deep-read still pending | Not complete. S02 cannot start yet. |
| S02 | ESCP and temporary erosion/sediment control | NOT STARTED | - | Drawing pending deep-read | Locked until S01 complete/reserved |
| S03 | Site clearing, earthwork, cut/fill and platform formation | NOT STARTED | - | Drawing pending deep-read | Earthwork quantities must be verified from drawing |
| S04 | Crossing bridge and permanent site entrance | NOT STARTED | - | Drawing pending deep-read | RC/bridge takeoff required |
| S05 | Building substructure: footing, stump and ground beam | NOT STARTED | - | Structural drawings pending deep-read | Must include concrete, rebar, formwork, excavation |
| S06 | Under-slab plumbing, sewerage and drainage rough-in | NOT STARTED | - | Plumbing/sewerage drawings pending deep-read | Must avoid duplicate with S12/S21 |
| S07 | Ground floor slab, apron, steps and ramps | NOT STARTED | - | Structural/architectural drawings pending deep-read | Must include slab build-up, BRC, DPM, hardcore if applicable |
| S08 | RC columns, roof beams and internal roof beams | NOT STARTED | - | Structural drawings pending deep-read | Must include mark-by-mark structural takeoff |
| S09 | Steel roof framing | NOT STARTED | - | Roof framing drawings pending deep-read | Must resolve duplicate/variant roof framing drawing if any |
| S10 | Roof covering and rainwater goods | NOT STARTED | - | Roof/section/elevation drawings pending deep-read | Include gutter/downpipe/flashing if shown |
| S11 | Masonry walls, brick screens and ventilation openings | NOT STARTED | - | Architectural drawings pending deep-read | W4-W6 and BS1 must not be treated as aluminium windows |
| S12 | Internal plumbing, sanitary and ablution system | NOT STARTED | - | Sanitary plumbing schematic pending deep-read | Separate from under-slab rough-in |
| S13 | Electrical, lighting, fans, power, earthing and ELV | NOT STARTED | - | Electrical drawing availability pending | May be RESERVED WITH REASON if no drawing/source |
| S14 | Internal/external plaster, render and skim coat | NOT STARTED | - | Architectural drawings pending deep-read | Surface areas required |
| S15 | Waterproofing, screed and wet-area floor falls | NOT STARTED | - | Architectural/plumbing drawings pending deep-read | Wet-area scope required |
| S16 | Floor and wall finishes | NOT STARTED | - | Architectural drawings pending deep-read | Finish schedule may be provisional |
| S17 | Timber doors, frames and ironmongery | NOT STARTED | - | Door schedule + floor plan pending deep-read | D1/D3 counts must be verified |
| S18 | Aluminium doors, windows, glass louvres and glazing | NOT STARTED | - | Door/window schedule + floor plan pending deep-read | D2/W1/W2/W3 counts must be verified |
| S19 | Ceiling and access panels | NOT STARTED | - | Ceiling/RCP availability pending | May be RESERVED WITH REASON if no drawing/source |
| S20 | Painting and architectural final fittings | NOT STARTED | - | Architectural drawings pending deep-read | Depends on plaster/wall/ceiling quantities |
| S21 | External sewerage system | NOT STARTED | - | Sewerage schematic pending deep-read | Separate from stormwater drainage |
| S22 | Permanent stormwater drainage | NOT STARTED | - | Road/drain drawings pending deep-read | Drains/catchpits/outfall required |
| S23 | Permanent fencing and gates | NOT STARTED | - | Fence/gate drawing pending deep-read | Default in-house unless owner changes |
| S24 | Road, parking, kerb, road base and premix | NOT STARTED | - | Road/drain/site drawings pending deep-read | Premix area must be measured, not residual lot area |
| S25 | Road marking, parking marking and traffic signage | NOT STARTED | - | Road/parking drawings pending deep-read | Keep separate from premix package |

## Per-SXX completion checklist

Before marking any SXX `COMPLETE FOR NEXT SXX`, confirm:

- SPEC A:C basis is complete enough for takeoff;
- source drawing/reference is listed;
- raw quantity, deductions and final quantity are shown;
- material item names and UOM match `1.2 Materials.txt` where available;
- labour/service names and UOM match `1.3 Labour.txt` where available;
- wastage is explicit;
- buffer/contingency is separate from wastage;
- practical stock/unit rounding is shown;
- MH productivity or fixed labour basis is shown;
- Block 1, Block 2 and Block 3 are separated;
- missing master/rate/design items are listed;
- SXX total status is labelled.

## Overall price rule

Overall project price must be built from completed SXX files only.

If some SXX are reserved/provisional, the overall summary must label them clearly and must not claim final customer-ready price.

## Current gate

```text
CURRENT ACTIVE SXX: S01
S01 COMPLETE FOR NEXT SXX: NO
S02 START ALLOWED: NO
NEXT ACTION: Deep-read source/drawing register and resolve S01 missing items.
```
