# Surau Nilai — SXX Costing Tracker V4

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/03_SXX_COSTING_TRACKER_V3.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

BOQ folder:

```text
ActiveBOQ/Surau Nilai/BOQ/
```

## V4 correction note

Owner corrected that `PROVISIONAL` must not be used simply because a material/labour/rate is missing. Every SXX must be completed as a muktamad working-cost basis before moving to the next SXX. Missing root master items must be filled through root master match, current web/market search, approved addendum reference, logical working-cost basis or supplier-needed remark, but quantity/UOM/rate/amount/markup status must not be left NIL or blank.

S01 has been upgraded to:

```text
ActiveBOQ/Surau Nilai/BOQ/S01_Preliminaries_Takeoff_Block1-3_V4.txt
```

## Current gate

```text
CURRENT ACTIVE SXX: S02
S01 COMPLETE FOR NEXT SXX: YES - MUKTAMAD WORKING-COST BASIS
S01 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S02 START ALLOWED: YES
```

## SXX tracker

| SXX | Proposed scope | Status | Cost file | Source evidence | Notes |
|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | COMPLETE FOR NEXT SXX - MUKTAMAD WORKING-COST BASIS | `S01_Preliminaries_Takeoff_Block1-3_V4.txt` | README, Materials/Labour, GPTEditable/Reference_Addendum, web/current market check, drawing/source register | Base working cost RM8,750.00; optional 10% contingency RM875.00; with contingency RM9,625.00. No customer markup. If later drawing/SXX creates contradiction/double count, revise S01 before continuing. |
| S02 | ESCP and temporary erosion/sediment control | NOT STARTED | - | ESCP drawing pending S02 takeoff | S02 may start next; must use SPEC A:C + Block 1-3 `.txt` and fill all required lines. |
| S03 | Site clearing, earthwork, cut/fill and platform formation | NOT STARTED | - | Drawing pending deep-read | Earthwork quantities must be verified from drawing. |
| S04 | Crossing bridge and permanent site entrance | NOT STARTED | - | Drawing pending deep-read | RC/bridge takeoff required. |
| S05 | Building substructure: footing, stump and ground beam | NOT STARTED | - | Structural drawings pending deep-read | Must include concrete, rebar, formwork, excavation. |
| S06 | Under-slab plumbing, sewerage and drainage rough-in | NOT STARTED | - | Plumbing/sewerage drawings pending deep-read | Must avoid duplicate with S12/S21. |
| S07 | Ground floor slab, apron, steps and ramps | NOT STARTED | - | Structural/architectural drawings pending deep-read | Must include slab build-up, BRC, DPM, hardcore if applicable. |
| S08 | RC columns, roof beams and internal roof beams | NOT STARTED | - | Structural drawings pending deep-read | Must include mark-by-mark structural takeoff. |
| S09 | Steel roof framing | NOT STARTED | - | Roof framing drawings pending deep-read | Must resolve duplicate/variant roof framing drawing if any. |
| S10 | Roof covering and rainwater goods | NOT STARTED | - | Roof/section/elevation drawings pending deep-read | Include gutter/downpipe/flashing if shown. |
| S11 | Masonry walls, brick screens and ventilation openings | NOT STARTED | - | Architectural drawings pending deep-read | W4-W6 and BS1 must not be treated as aluminium windows. |
| S12 | Internal plumbing, sanitary and ablution system | NOT STARTED | - | Sanitary plumbing schematic pending deep-read | Separate from under-slab rough-in. |
| S13 | Electrical, lighting, fans, power, earthing and ELV | NOT STARTED | - | Electrical drawing availability pending | May be reserved only with explicit reason; cannot be NIL if source/addendum can fill basis. |
| S14 | Internal/external plaster, render and skim coat | NOT STARTED | - | Architectural drawings pending deep-read | Surface areas required. |
| S15 | Waterproofing, screed and wet-area floor falls | NOT STARTED | - | Architectural/plumbing drawings pending deep-read | Wet-area scope required. |
| S16 | Floor and wall finishes | NOT STARTED | - | Architectural drawings pending deep-read | Finish schedule may be provisional only for real spec conflict; no blank rate lines. |
| S17 | Timber doors, frames and ironmongery | NOT STARTED | - | Door schedule + floor plan pending deep-read | D1/D3 counts must be verified. |
| S18 | Aluminium doors, windows, glass louvres and glazing | NOT STARTED | - | Door/window schedule + floor plan pending deep-read | D2/W1/W2/W3 counts must be verified. |
| S19 | Ceiling and access panels | NOT STARTED | - | Ceiling/RCP source if available | May be reserved only with explicit reason; cannot be NIL if source/addendum can fill basis. |
| S20 | Painting and architectural final fittings | NOT STARTED | - | Architectural drawings pending deep-read | Depends on plaster/wall/ceiling quantities. |
| S21 | External sewerage system | NOT STARTED | - | Sewerage schematic pending deep-read | Separate from stormwater drainage. |
| S22 | Permanent stormwater drainage | NOT STARTED | - | Road/drain drawings pending deep-read | Drains/catchpits/outfall required. |
| S23 | Permanent fencing and gates | NOT STARTED | - | Fence/gate drawing pending deep-read | Default in-house unless owner changes. |
| S24 | Road, parking, kerb, road base and premix | NOT STARTED | - | Road/drain/site drawings pending deep-read | Premix area must be measured, not residual lot area. |
| S25 | Road marking, parking marking and traffic signage | NOT STARTED | - | Road/parking drawings pending deep-read | Keep separate from premix package. |

## Per-SXX completion checklist

Before marking any SXX complete for next SXX, confirm:

- SPEC A:C basis is complete enough for takeoff;
- output is `.txt` tab-delimited if intended for Excel/XLS copy-paste;
- source drawing/reference is listed;
- raw quantity, deductions and final quantity are shown;
- material item names and UOM match root `1.2 Materials.txt` where available;
- if root material item is missing, approved addendum/current market working-cost reference is used and status is marked;
- labour/service names and UOM match root `1.3 Labour.txt` where available;
- if root labour/service item is missing, approved addendum/current market working-cost reference is used and status is marked;
- wastage is explicit;
- buffer/contingency is separate from wastage;
- practical stock/unit rounding is shown;
- MH productivity or fixed labour basis is shown;
- Block 1, Block 2 and Block 3 are separated;
- no required line is NIL/blank only because the master list lacks an item;
- markup status is stated for every rate line;
- if later SXX creates contradiction/double count/undercost/overprice, affected previous SXX is corrected before continuing.
