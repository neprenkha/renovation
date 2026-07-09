# Floorplan Estimate Rule V1

## Purpose

This file records the working rule for cases where the customer supplied a floor plan but exact dimensions are incomplete, unreadable or not directly stated.

The active customer request is an interior renovation / fit-out scope, so floorplan-based assumptions may be used for early budgeting, but must remain clearly marked as estimates.

## Allowed estimate approach

When exact sizes are missing:

1. Use the customer request first.
2. Use the supplied floor plan/drawing where readable.
3. If the drawing has no clear dimension for one item, estimate from room proportion and normal terrace-house layout.
4. Use realistic sizes only; do not choose sizes that look too small, too large or impossible for the room.
5. Mark every such quantity as `FLOORPLAN ESTIMATE`.
6. Use a `+/-` allowance where practical.
7. Keep the quotation subject to final site measurement and final design confirmation.

## Typical default assumptions when drawing is unclear

These are not final measurements. They are only early-budget assumptions until the floor plan is measured.

| Item | Reasonable early-budget basis |
|---|---|
| Kitchen base cabinet | Estimate by kitchen wall run, commonly 8ft-12ft for terrace kitchen unless floor plan shows otherwise. |
| Kitchen wall cabinet | Usually follows part or full base run, commonly 6ft-10ft unless window/hood blocks the wall. |
| Countertop | Follows base cabinet run; depth usually around 2ft unless design says otherwise. |
| Backsplash | Follows countertop run; height commonly 2ft-3ft unless full-height wall finish requested. |
| TV cabinet | Estimate by TV wall width, commonly 6ft-10ft for living area. |
| Master bedroom cabinet | Estimate by available bedroom wall, commonly 6ft-10ft. |
| Make-up table | Commonly 3ft-4ft if not drawn. |
| Shoe cabinet | Commonly 3ft-5ft near entrance if not drawn. |
| Living C-box ceiling | Estimate by living perimeter/feature area from floor plan. |
| Kitchen flat ceiling | Estimate from kitchen floor area. |
| SPC flooring | Estimate living hall floor area from floor plan. |
| Painting | Estimate from listed rooms/walls, not from whole house unless requested. |
| Wiring | Use stated point quantities first; estimate only the missing point counts from floor plan and lighting layout. |
| Plumbing relocation | Estimate route only when old/new washing-machine positions are visible. |
| Mirror/fluted/wainscoting | Estimate by dining wall width/height from floor plan or mark design confirmation required. |

## Prohibited

- Do not edit the original floor plan, drawing or `Customer Request.txt`.
- Do not hide assumptions.
- Do not present estimated quantities as final measured quantities.
- Do not use customer-facing wording that implies brand/model is confirmed.
- Do not expose internal raw costing or supplier names in customer quotation.

## Next use

Use this rule to create upgraded SPEC, takeoff and quotation files such as:

- `Customer_Request_SPEC_V2.tsv`
- `ActiveBOQ_Takeoff_Assumption_V1.tsv`
- `Customer_Quotation_Draft_V1.md`
