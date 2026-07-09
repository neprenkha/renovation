# Surau Nilai — S01 Preliminaries Costing V1

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

BOQ folder:

```text
ActiveBOQ/Surau Nilai/BOQ/
```

## Status

```text
S01 STATUS: IN PROGRESS - NOT COMPLETE FOR S02
PRICE STATUS: PARTIAL WORKING COST ONLY
NEXT SXX ALLOWED: NO
```

Reason S01 is not complete yet:

- all Surau Nilai drawing PDFs still need deep-read / visual inspection before final preliminaries;
- hoarding length and exact signboard requirement must be confirmed from drawing/source;
- project duration/programme is not yet confirmed;
- temporary water/electricity requirement is not yet confirmed;
- no exact master-list item found yet for hoarding, project signboard, mobilisation/demobilisation or temporary utilities;
- S01 may only move to `COMPLETE FOR NEXT SXX` after missing items are resolved or formally reserved.

## Source and governance checked

| Source | Status | Notes |
|---|---|---|
| `GPTRenovationHeader.txt` owner uploaded header | CHECKED | Full replacement header, 531 lines / 20,698 bytes / SHA-256 C25B79C30C527CFC4ED2447EBE14973E086BF9A241B600539A47A5AC4A3816CF |
| `GPTEditable/GPT Header Renovation.md` | CHECKED | Has owner-copy full header and correction-triggered update rules |
| `GPT Header Renovation.md` | CHECKED | Aligned with canonical editable header as of previous update |
| `GPTEditable/README_GPTEDITABLE.md` | CHECKED | Has full owner header and correction-triggered update rules |
| `README - BOQ.txt` | CHECKED | Manual BOQ workflow: SPEC first, then takeoff/cost blocks |
| `1.2 Materials.txt` | CHECKED | Root master material list, read-only |
| `1.3 Labour.txt` | CHECKED | Root master labour/service/rental list, read-only |
| `ActiveBOQ/Surau Nilai/BOQ/00_SURAU_NILAI_BOQ_COSTING_CONTROL_V1.md` | CHECKED | Sequential SXX costing rule applies |
| `ActiveBOQ/Surau Nilai/BOQ/01_SXX_COSTING_TRACKER_V1.md` | CHECKED | S01 is first scope and must complete before S02 |

## S01 scope title

| Spec | Description | Note |
|---|---|---|
| S01-TITLE | Preliminaries, mobilisation, setting out, hoarding and signboard | Site/project setup for Surau Nilai before measured trade works start |
| S01-OVERVIEW | Includes initial mobilisation, basic site setting out, preliminary site labour, coordination allowance, temporary protection/control notes, hoarding/signboard allowance check and temporary utilities check | Does not include measured construction work from S02 onward. Does not include authority/consultant/permanent utility deposit unless owner confirms inclusion. |
| S01-SOURCE | Source drawing/reference | Drawing deep-read register still required before final S01 completion. |
| S01-SEQUENCE | Sequence control | S01 must be completed or formally reserved before starting S02 costing. |
| S01-MASTER-LIST | Master list use | Exact descriptions from `1.2 Materials.txt` and `1.3 Labour.txt` must be used when available. Missing items must be listed instead of invented silently. |
| S01-PRICE-STATUS | Price status | Current file contains partial working cost only, not customer selling price. |

## Measured / quantity basis

| Item | Raw quantity | Deduction | Net quantity | UOM | Source/evidence | Status |
|---|---:|---:|---:|---|---|---|
| Mobilisation / demobilisation | 1 | 0 | 1 | LOT | Required for project setup, but no exact master item/rate yet | INPUT NEEDED / PROVISIONAL |
| Building/site setting out labour | 1 | 0 | 1 | DAY | Labour master list has MH rates; exact site duration pending | PARTIAL WORKING BASIS |
| Hoarding / temporary site fencing | INPUT NEEDED | 0 | INPUT NEEDED | M or LOT | Need drawing/site boundary measurement and required hoarding type | HOLD |
| Project signboard | INPUT NEEDED | 0 | INPUT NEEDED | PCS or LOT | Need signboard requirement/spec from drawing/authority/client | HOLD |
| Temporary water/electricity for construction | INPUT NEEDED | 0 | INPUT NEEDED | LOT | Need owner/project decision and supply arrangement | HOLD |
| Site safety/protection/admin allowance | INPUT NEEDED | 0 | INPUT NEEDED | LOT | Need scope decision; no exact master item found yet | HOLD |

## Block 1 — Material / product / consumable purchase

No final Block 1 material line is priced in this V1 because exact master-list material items for S01 preliminaries are not yet confirmed.

| Master description | UOM | Raw qty | Wastage | Purchase qty | Rate (RM) | Amount (RM) | Status | Notes |
|---|---|---:|---:|---:|---:|---:|---|---|
| INPUT NEEDED - Hoarding material / temporary fencing | M or LOT | - | - | - | - | - | MISSING MASTER / RATE | Need exact type and source before pricing |
| INPUT NEEDED - Project signboard material | PCS or LOT | - | - | - | - | - | MISSING MASTER / RATE | Need exact signboard size/spec/source before pricing |
| INPUT NEEDED - Temporary utilities consumables | LOT | - | - | - | - | - | MISSING MASTER / RATE | Need inclusion/exclusion decision |

## Block 2 — Labour / own work / plant / rental / productivity-based work

Partial working cost only, using exact available labour master descriptions.

| Master description from `1.3 Labour.txt` | UOM | Crew / productivity basis | Raw qty | Wastage | Charge qty | Rate (RM) | Amount (RM) | Status | Notes |
|---|---|---|---:|---:|---:|---:|---:|---|---|
| Labour - Skilled Worker (Per MH) | MH | 2 skilled workers x 8 hours for initial setting out / setup check | 16.00 | 0% | 16.00 | 22.50 | 360.00 | WORKING COST | Master note: skilled worker rate = RM180/day / 8h |
| Labour - General Helper (Per MH) | MH | 2 helpers x 8 hours for basic site setup/assistance | 16.00 | 0% | 16.00 | 16.25 | 260.00 | WORKING COST | Master note: helper rate = RM130/day / 8h |

Block 2 subtotal currently priced:

```text
RM 620.00
```

This is not the full S01 amount. It only covers the initial labour basis available from the current master labour list.

## Block 3 — External subcontract / specialist / service

No final Block 3 line is priced in this V1.

| Item | UOM | Quantity | Rate (RM) | Amount (RM) | Status | Notes |
|---|---|---:|---:|---:|---|---|
| Mobilisation / demobilisation complete package | LOT | - | - | - | INPUT NEEDED | No exact master item/rate found yet |
| Hoarding / temporary fencing complete package | M or LOT | - | - | - | INPUT NEEDED | Need length/type/source |
| Project signboard complete package | PCS or LOT | - | - | - | INPUT NEEDED | Need size/spec/source |
| Temporary utilities / temporary board / site connection | LOT | - | - | - | INPUT NEEDED | Need inclusion/exclusion and licensed contractor/source if required |

## Wastage, buffer and rounding

| Cost part | Wastage | Buffer / contingency | Rounding | Status |
|---|---:|---:|---|---|
| Block 2 labour MH | 0% | Not included | MH calculated directly | Partial working cost only |
| Hoarding/signboard materials | INPUT NEEDED | Not applied yet | Must round to full stock/panel/length/lot after source is known | HOLD |
| Temporary utilities | INPUT NEEDED | Not applied yet | Must follow supplier/electrician package or actual bill/lot | HOLD |

Wastage and buffer are deliberately not hidden inside S01 total.

## Current S01 subtotal

```text
Confirmed partial working cost: RM 620.00
Unpriced / missing S01 items: hoarding, signboard, mobilisation package, temporary utilities, safety/protection/admin allowance
S01 final total: NOT READY
Customer selling price: NOT READY
```

## Missing master / source list

These items must be resolved before S01 can be marked `COMPLETE FOR NEXT SXX`:

| Missing item | Required decision/source | Current action |
|---|---|---|
| Mobilisation / demobilisation | Decide whether to use provisional LOT, actual subcontract/service, or include inside preliminaries percentage | Pending |
| Hoarding / temporary fencing | Need length, height/type, material/system and whether in-house or subcontract | Pending drawing/site boundary check |
| Project signboard | Need size/spec/authority/client requirement and whether material/labour/subcontract | Pending drawing/source check |
| Temporary water/electricity | Confirm included/excluded and whether construction temporary supply only | Pending owner/project decision |
| Site safety/protection/admin allowance | Confirm required allowance basis and duration | Pending project programme |
| Project duration | Need programme/duration basis to price time-related preliminaries | Pending |

## Gate result

```text
S01 RESULT: IN PROGRESS
S01 COMPLETE FOR NEXT SXX: NO
REASON: S01 has only partial working labour cost. Major preliminary items remain missing/pending source evidence.
NEXT REQUIRED ACTION: Deep-read drawing/source register and resolve S01 missing items before S02 starts.
```
