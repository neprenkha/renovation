# Surau Nilai — Takeoff Method

## Work sequence

1. Confirm drawing file list from `Drawing/`.
2. Identify sheet name/title/revision/date if visible.
3. Create a drawing register.
4. Break scope into trade sections.
5. Measure quantities from drawings.
6. Record all assumptions and unresolved dimensions.
7. Create takeoff detail.
8. Convert approved quantities into BOQ format.

## Drawing register format

| No. | Drawing file | Sheet title / content | Revision / date | Pages | Use for takeoff | Notes |
|---:|---|---|---|---:|---|---|
| 1 | To be listed | To be checked | To be checked | - | Pending | Do not edit source PDF |

## Trade breakdown for checking

| Trade | What to check | Unit basis | Notes |
|---|---|---|---|
| Roof / awning / metal work | Roof pitch, span, ridge height, frame, purlin, gutter, flashing | m, m2, no. | Confirm with drawing before final quantity |
| Ceiling / soffit | Ceiling board/strip, support, edge trim | m2, m, no. | Check actual coverage and openings |
| Wall / partition / cladding | Panel, board, frame, finishing | m2, m | Separate by material/type |
| Door / window / glass | Size, panel count, frame, glass type | no., m2 | Confirm schedule if provided |
| Drainage / gutter | Hidden gutter, outlet, downpipe, flashing | m, no. | Confirm routing and discharge |
| Electrical / lighting | Point, fitting, wiring route | no., m | Only if shown in drawings |
| Floor / finishes | Floor area, skirting, steps, threshold | m2, m | Only if shown in drawings |
| Miscellaneous | Any item visible but not classified | item | Record query if unclear |

## Measurement rules

- Keep every item traceable to a drawing file/sheet.
- Do not combine unlike materials in one quantity line.
- Use millimetres for raw dimensions and convert to metres/metres square in quantity table where needed.
- If drawing is not to scale or scale is unclear, do not measure by image scale unless owner approves.
- If roof pitch or dimension is derived by formula, show the formula.

## Standard takeoff table

| No. | Trade | Item | Drawing reference | Location | L (mm) | W (mm) | H/Rise (mm) | Qty calculation | Unit | Quantity | Remarks |
|---:|---|---|---|---|---:|---:|---:|---|---|---:|---|
| 1 | Roof | Ridge height check | Earlier discussion / drawing to verify | Main roof | 3075 half-span | - | 2153 approx | tan(35°) × 3075 | mm | 2153 | Verify against section |

## Query log format

| No. | Drawing reference | Issue / missing detail | Why it matters | Owner decision / answer |
|---:|---|---|---|---|
| 1 | Pending drawing review | Confirm whether 6150 mm is true horizontal projection/span | Affects roof height and sloping length | Pending |

## Output expected before pricing

A complete takeoff detail should be produced first. Pricing/quotation text should only be prepared after quantities and assumptions are checked.