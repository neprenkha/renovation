# Surau Nilai — Deep Read Drawing / Source Register V1

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

Read-only customer/spec source folder:

```text
ActiveBOQ/Surau Nilai/Drawing/
```

Writable takeoff/work folders:

```text
ActiveBOQ/Surau Nilai/Takeoff_Work/
ActiveBOQ/Surau Nilai/BOQ/
ActiveBOQ/Surau Nilai/BOQ_work/
ActiveBOQ/Surau Nilai/GPT_CONTROL/
```

## Purpose

This register is the mandatory source-control layer before final takeoff/BOQ finalisation.

The drawing folder is the customer's requested specification source. Takeoff must not rely only on memory or a short chat explanation. Every SXX must trace back to drawing/source evidence, previous owner corrections and clear measurement logic so that QS, owner, contractor and a future GPT session can understand and audit it.

## Project identity / lot rule

| Item | Governing value | Status | Notes |
|---|---|---|---|
| Project folder | `ActiveBOQ/Surau Nilai/` | ACTIVE | Working folder name only. |
| Project/drawing name | `SURAU JURESSALAM` / Surau Juasseh Sentosa references | OWNER/SESSION CAPTURE | Use actual drawing title where visible during visual read. |
| Governing working lot | `Lot 20093` | OWNER-CORRECTED / GOVERNING | Previous session correction: use Lot 20093. If a drawing/source shows Lot 20059 or other lot number, record as conflict and do not silently override owner-corrected lot. |
| Drawing folder authority | Customer/spec source | GOVERNING SOURCE | Read-only. Must be checked for takeoff. |

## Takeoff completeness definition

A takeoff line is not complete unless it records:

- SXX scope/trade;
- source drawing filename;
- sheet/title/revision/page where visible;
- measured element/location;
- dimension source;
- formula;
- raw quantity;
- deductions;
- net quantity;
- UOM;
- wastage and stock rounding where relevant;
- buffer/contingency if any;
- material/labour/addendum reference;
- status: measured, drawing-derived, owner-corrected, provisional, supplier quote needed, conflict, or unreadable.

Takeoff must be understandable by owner, QS, contractor, future GPT session and future reviewer. It is not just a private working note.

## Mandatory before asking owner

Before asking the owner a question or saying an item is unknown, GPT must check:

1. latest owner instruction;
2. uploaded/current `GPTRenovationHeader.txt`;
3. GitHub canonical governance and GPTEditable files;
4. this register and active Surau Nilai files;
5. previous session discussion/corrections available in context;
6. drawing/source files;
7. `README - BOQ.txt`, `1.2 Materials.txt`, `1.3 Labour.txt`;
8. `GPTEditable/Reference_Addendum/`.

Only unresolved conflicts or missing source after those checks should be asked back to owner.

## Drawing register

| No. | Drawing filename | Source role | Relevant SXX | Visual/deep-read status | Immediate takeoff notes |
|---:|---|---|---|---|---|
| 1 | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf` | Layout / architectural base | S01, S05-S20 | PENDING VISUAL READ | Must verify layout, dimensions, door/window/opening positions, hoarding/site relation if shown. |
| 2 | `02-SURAU JERUSSALAM SLAB SECTION 01.pdf` | Structural slab section | S05-S08 | PENDING VISUAL READ | Slab/section quantities must trace here. |
| 3 | `03-SURAU JERUSSALAM SLAB SECTION 02.pdf` | Structural slab section | S05-S08 | PENDING VISUAL READ | Slab/section quantities must trace here. |
| 4 | `04-SURAU JERUSSALAM GROUND BEAM DETAIL 01.pdf` | Ground beam detail | S05 | PENDING VISUAL READ | Ground beam concrete/rebar/formwork takeoff source. |
| 5 | `05-SURAU JERUSSALAM GROUND BEAM DETAIL 02.pdf` | Ground beam detail | S05 | PENDING VISUAL READ | Ground beam concrete/rebar/formwork takeoff source. |
| 6 | `06-SURAU JURESSALAM ROOF BEAM DETAIL-R01 Model.pdf` | Roof beam detail | S08 | PENDING VISUAL READ | RC beam concrete/rebar/formwork takeoff source. |
| 7 | `07-SURAU JURESSALAM INT RF BEAM DETAIL-R01 Model.pdf` | Internal roof beam detail | S08 | PENDING VISUAL READ | Internal roof beam takeoff source. |
| 8 | `CROSSING BRIDGE.pdf` | Crossing bridge / access structure | S04 | PENDING VISUAL READ | Bridge/entrance quantity source. |
| 9 | `Fencing and Gate 1.pdf` | Permanent fence/gate | S23 | PENDING VISUAL READ | Fence/gate takeoff source; may also inform site boundary. |
| 10 | `Hoarding and Signboard 1.pdf` | Hoarding and signboard | S01 | PENDING VISUAL READ | S01 must reference this before final. Hoarding is included if shown/required. |
| 11 | `Roof Framing 1.pdf` | Roof framing | S09 | PENDING VISUAL READ | Check against `Roof Framing.pdf` for duplicate/revision conflict. |
| 12 | `Roof Framing.pdf` | Roof framing | S09 | PENDING VISUAL READ | Check against `Roof Framing 1.pdf` for duplicate/revision conflict. |
| 13 | `SJ_01ESCP-LP-01-S0-00.pdf` | ESCP layout | S02 | PENDING VISUAL READ | S02 source for temporary erosion/sediment control. |
| 14 | `SJ_01EW-CS-01-S0-00.pdf` | Earthwork cross section | S03 | PENDING VISUAL READ | Earthwork cross-section/source. |
| 15 | `SJ_01EW-DT-01-S0-00.pdf` | Earthwork detail | S03 | PENDING VISUAL READ | Earthwork details/source. |
| 16 | `SJ_01EW-LP-01-S0-00.pdf` | Earthwork layout | S03 | PENDING VISUAL READ | Site clearing/cut/fill/platform source. |
| 17 | `SJ_02R&D-DT-02-S0-00.pdf` | Road and drainage detail | S22, S24, S25 | PENDING VISUAL READ | Road/drainage build-up/detail source. |
| 18 | `SJ_02R&D-LP-01-S0-01.pdf` | Road and drainage layout | S22, S24, S25 | PENDING VISUAL READ | Road/parking/drainage/marking source. |
| 19 | `Surau Juasseh sections and elevations tender_constn 1.pdf` | Architectural sections/elevations | S10-S20 | PENDING VISUAL READ | Wall height, roof, finishes, openings. |
| 20 | `Surau Plan Roof Plan Bldg Tender_Constn.pdf` | Building plan / roof plan | S09-S20 | PENDING VISUAL READ | Roof, layout, openings, finishes and door/window basis. |
| 21 | `Surau Sanitary Plumbing Schematic 1.pdf` | Sanitary/plumbing schematic | S06, S12 | PENDING VISUAL READ | Must avoid duplicate with external sewerage. |
| 22 | `Surau Sewerage Schematic 1.pdf` | Sewerage schematic | S06, S21 | PENDING VISUAL READ | External sewerage and under-slab interface. |
| 23 | `Surau Site Plan Tender_Constn.pdf` | Site plan / lot/site relation | S01-S04, S21-S25 | PENDING VISUAL READ | Lot, site boundary, hoarding/site access, road/parking/drainage. Must verify Lot 20093 conflict if shown. |
| 24 | `Survey Tapak Surau Juassewh Sentosa.pdf` | Survey / existing site | S01-S04, S21-S25 | PENDING VISUAL READ | Survey/lot/levels/source. Must verify lot/size conflict if shown. |

## S01 impact

S01 `Preliminaries, mobilisation, setting out, hoarding and signboard` is included in the project sequence.

Current S01 costing file:

```text
ActiveBOQ/Surau Nilai/BOQ/S01_Preliminaries_Costing_V2.txt
```

Current S01 status:

```text
COMPLETE FOR NEXT SXX - PROVISIONAL
```

Reason: S01 can proceed using provisional/addendum rates, but final S01 must return to this drawing register and specifically verify:

- `Hoarding and Signboard 1.pdf`;
- site plan / survey for boundary/length/access;
- exact hoarding length/type;
- exact signboard size/spec;
- temporary utilities and preliminaries requirements.

## SXX dependency map

| SXX | Scope | Minimum source check before final |
|---|---|---|
| S01 | Preliminaries / hoarding / signboard | Hoarding and Signboard, Site Plan, Survey, previous owner corrections |
| S02 | ESCP | ESCP layout/details and site plan |
| S03 | Site clearing / earthwork | Earthwork layout/details/cross sections, survey, site plan |
| S04 | Crossing bridge / entrance | Crossing Bridge, site/road interface |
| S05 | Footing / stump / ground beam | Structural layout, footing/ground beam drawings |
| S06 | Under-slab plumbing/sewerage rough-in | Sanitary and sewerage schematics, slab plan/interface |
| S07 | Slab/apron/steps/ramps | Slab sections, building plan, sections/elevations |
| S08 | RC columns/roof beams/internal roof beams | Roof beam/internal roof beam/structural drawings |
| S09 | Steel roof framing | Roof framing drawings and roof plan |
| S10 | Roof covering / gutter / downpipe | Roof plan, elevations/sections |
| S11 | Masonry / brick screen / openings | Layout, elevations/sections, opening schedule |
| S12 | Internal plumbing/sanitary/ablution | Sanitary plumbing schematic and architectural wet areas |
| S13 | Electrical | Electrical source if available; if absent, mark reserved/provisional with reason |
| S14 | Plaster/render/skim | Wall/elevation/height drawings |
| S15 | Waterproofing/screed/falls | Wet area layout and plumbing/interface drawings |
| S16 | Floor/wall finishes | Floor plan/finish notes/elevations |
| S17 | Timber doors/ironmongery | Door schedule/floor plan/opening confirmation |
| S18 | Aluminium/windows/glass/louvres | Door-window schedule/floor plan/elevations |
| S19 | Ceiling/access panels | Ceiling/RCP source if available; otherwise reserved/provisional with reason |
| S20 | Painting/final fittings | Plaster/wall/ceiling/finish area basis |
| S21 | External sewerage | Sewerage schematic/site plan |
| S22 | Stormwater drainage | R&D layout/details/site plan |
| S23 | Fence/gate | Fencing and Gate drawing/site boundary |
| S24 | Road/parking/kerb/premix | R&D layout/details/site plan/survey; exact premix polygon required |
| S25 | Road marking/signage | R&D/parking layout and marking/signage source |

## Register status

```text
REGISTER STATUS: CREATED - VISUAL DEEP READ PENDING
NEXT ACTION: Render/visually inspect drawings and convert this register into measured takeoff evidence per SXX.
DO NOT CLAIM FINAL OVERALL BOQ UNTIL DRAWING REGISTER AND SXX TAKEOFF ARE RECONCILED.
```
