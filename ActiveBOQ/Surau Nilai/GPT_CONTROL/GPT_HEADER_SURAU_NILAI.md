# GPT HEADER — SURAU NILAI ACTIVEBOQ WORKSPACE

## Identity

Project workspace:

```text
ActiveBOQ/Surau Nilai/
```

Official project name from BOQ README context:

```text
SURAU JURESSALAM
```

Governing lot:

```text
Lot 20093
```

This header is for GPT working through GitHub. It is not a Cursor shell workflow.

## Absolute workspace boundary

GPT must stay inside this repository path only:

```text
ActiveBOQ/Surau Nilai/
```

Do not treat the wider `ActiveBOQ/` folder as the work area. `ActiveBOQ/` is only a parent that stores many separate project folders.

When the owner says the workspace is `ActiveBOQ/Surau Nilai`, GPT must not drift into other projects, local drive roots, or parent folders.

## Protected read-only folders

These folders are source/reference only:

```text
ActiveBOQ/Surau Nilai/Drawing/
ActiveBOQ/Surau Nilai/OriginalFile/
```

`OriginalFile/` may not exist yet. If the owner creates it later, it is automatically read-only.

GPT must not edit, rename, move, replace, reorganize, overwrite, or delete any file in those folders.

## Allowed GPT-created folders

GPT may create or edit only within GPT-created working/output folders under:

```text
ActiveBOQ/Surau Nilai/
```

Approved working folders:

```text
ActiveBOQ/Surau Nilai/GPT_CONTROL/
ActiveBOQ/Surau Nilai/Takeoff_Work/
ActiveBOQ/Surau Nilai/BOQ/
ActiveBOQ/Surau Nilai/BOQ_work/
```

Folder purpose:

| Folder | Purpose | Write allowed |
|---|---|---|
| `GPT_CONTROL/` | GPT headers, readme, guardrails, project instructions | Yes |
| `Takeoff_Work/` | Early measurement notes, takeoff detail, query logs | Yes |
| `BOQ/` | BOQ registers, AC files, supplier files, manifest | Yes |
| `BOQ_work/` | Temporary working notes or intermediate extraction | Yes, but do not auto-clean |
| `Drawing/` | Uploaded drawings/PDF source | No |
| `OriginalFile/` | Owner original source files if later created | No |

## No destructive actions

GPT must not instruct or perform file/folder deletion, recursive cleanup, mirror sync, forced overwrite, or source-folder reorganization.

Do not delete any folder as a completion step. If an older instruction says to remove a temporary folder before finishing, treat that as superseded for GPT/GitHub work. Instead, leave the folder and record it for owner manual review.

## Drawing and source handling

`Drawing/` is only for reference. GPT may read/list/download/inspect drawings for understanding, but must not change them.

If a new source/original folder is added by owner, it is read-only by default unless owner explicitly says it is a GPT working folder.

## Current work objective

The immediate job is not pricing first. The job is:

1. preserve workspace safety;
2. list and inspect the drawing PDFs;
3. create drawing register and takeoff trail;
4. extract visible drawing information;
5. build detailed takeoff;
6. rebuild BOQ foundation only after drawing evidence is checked;
7. keep outputs separated from source drawings.

## Uploaded BOQ README requirements captured

The uploaded BOQ README states that the previous foundation output is not approved and that work must not proceed to Block 1, Block 2, Block 3, pricing, online research, or workbook work before foundation rebuild and validation.

The uploaded BOQ README also defines:

```text
Drawing folder: ActiveBOQ/Surau Nilai/Drawing/
Generated-output folder: ActiveBOQ/Surau Nilai/BOQ/
```

For GitHub work, interpret those as repository paths.

## Key BOQ rebuild checkpoints to preserve

### Drawing/PDF audit

- Inspect all uploaded drawing PDFs visually.
- Do not abandon image-based or partially image-based drawings as unreadable.
- Zoom into schedules, callouts, reinforcement details, notes and legends.
- Record drawing title, number, revision, date, scale and readable status where visible.

### Structural drawings 01–07

Structural extraction must include, where shown:

- footing mark and count;
- footing width, length and thickness;
- X and Y reinforcement;
- ties;
- stump mark, size and reinforcement;
- column marks C1, C2 and C3;
- column size by level;
- main bars;
- outer/inner ties;
- ground beam marks and lengths;
- beam width/depth;
- top, bottom and extra reinforcement;
- link size and spacing;
- roof beam and internal roof beam marks;
- slab zones;
- slab thickness;
- suspended/non-suspended slab distinction;
- concrete grade;
- lean concrete;
- BRC designation and covered zone;
- apron thickness and reinforcement;
- formwork surfaces;
- estimating reinforcement quantity by diameter;
- lap, anchorage and waste basis.

Mandatory footing schedule checkpoints to verify against drawings:

| Mark | Size | Reinforcement |
|---|---|---|
| P1 | 550 x 550 x 250 mm | 3T12 each direction |
| P2 | 700 x 700 x 250 mm | 4T12 each direction |
| P3 | 850 x 850 x 250 mm | 4T12 each direction |
| P4 | 1050 x 1050 x 250 mm | 5T12 each direction |
| P5 | 1200 x 1200 x 250 mm | 6T12 each direction |

These checkpoints are not substitutes for drawing inspection.

### Door/window/opening checkpoints

Use door/window schedule for type and size. Use floor-plan symbols for quantity. Do not count the schedule symbol as an installed unit.

| Code | Size | Count |
|---|---:|---:|
| D1 | 900 x 2400 mm | 4 units |
| D2 | 2300 x 2400 mm | 3 units |
| D3 | 1000 x 2400 mm | 3 units |
| W1 | 900 x 1200 mm | 2 units |
| W2 | 2280 x 2400 mm | 5 units |
| W3 | 750 x 2400 mm | 2 units |
| W4 | 4650 x 600 mm | 2 openings |
| W5 | 2250 x 600 mm | 3 openings |
| W6 | 1150 x 600 mm | 1 opening |
| BS1 | 2300 x 2400 mm | 7 panels |

Locked corrections:

- Do not create D3B.
- Do not describe D3 as 900 x 2400 mm.
- Do not reverse W2 and W3 dimensions.
- D2 must remain heavy-duty commercial performance-grade aluminium sliding-door system with powder-coated aluminium frame and 10 mm clear tempered safety glass unless manufacturer shop drawing proves otherwise.

### Premix area

Reject 1202.63 m2 as exact unless independently proven from the actual tarmac/premix boundary.

Premix must be traced from site/road layout and recorded with polygons, deductions and status. If exact measurement is not defensible from PDF, mark it `PROJECT PROVISIONAL` and state tolerance.

Parking checkpoints to reconfirm:

```text
24 car bays
18 motorcycle bays
2 OKU bays
```

### BOQ outputs

When rebuilding foundation, output under:

```text
ActiveBOQ/Surau Nilai/BOQ/
```

Required BOQ foundation files include:

- drawing register;
- conflict/revision register;
- scope sequence register;
- measurement register;
- structural mark register;
- door/window/opening register;
- master coverage register;
- S01 AC.txt through S25 AC.txt;
- supplier enquiry files;
- generated file manifest.

## TSV and validation rules

- All register/supplier/AC TSV-style files must use actual tab characters.
- Do not use fragile string generation that changes tab structure.
- Every schema must be validated by field count.
- Do not claim PASS because a file was written.
- Reopen and validate the generated file content.

## Supplier file rules

Supplier files must remain short and contain only:

```text
Description<TAB>Qty<TAB>UOM
```

No internal notes, no SXX references, no drawing references and no long BOQ explanations.

No supplier row may contain unresolved placeholder quantities such as `INPUT NEEDED`, `TBC`, `TBA`, or `UNKNOWN`.

`NIL` is allowed only for an intentionally priced zero item.

## Final decision rules

Use:

```text
FOUNDATION REBUILT — READY FOR GPT AUDIT
```

only if all validation passes.

Otherwise use:

```text
FOUNDATION REBUILD INCOMPLETE — DO NOT PROCEED TO BLOCKS
```

## Future GPT response rule

When user says the workspace is `ActiveBOQ/Surau Nilai`, GPT must treat that as the hard boundary and never drift into wider `ActiveBOQ`, local drive roots, other projects, or source folders.
