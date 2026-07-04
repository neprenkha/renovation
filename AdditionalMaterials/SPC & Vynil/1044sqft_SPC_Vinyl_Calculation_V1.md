# 1044sqft SPC / Vinyl Calculation V1

## Purpose

This document records the standard logic for estimating SPC/Vinyl additional materials when a customer gives only total floor area.

Example area:

`1044 sqft`

Owner example labour rate:

`RM1.20/sqft`

This is a calculation example for another job, not the earlier ActiveBOQ customer quotation.

## Price reference used

Source folder:

`AdditionalMaterials/SPC & Vynil/`

Current price list reference:

`PRICE.txt`

Known stock prices from the current price list:

| Item | Stock coverage / size | Price |
|---|---:|---:|
| 4.5mm SPC Flooring Virgin Material | 24.16 sqft/box | RM68.90/box |
| 5.5mm SPC Flooring Virgin Material | 19.33 sqft/box | RM61.90/box |
| 6mm SPC Flooring Virgin Material | 19.27 sqft/box | RM77.10/box |
| 5.5mm SPC Herringbone | 17.63 sqft/box | RM76.80/box |
| 3mm Vinyl Square Tile | 36 sqft/box | RM86.50/box |
| 3mm Vinyl Tile | 36 sqft/box | RM86.50/box |
| Glue 5kg | tub | RM85 |
| Glue 10kg | tub | RM120 |
| Glue 20kg | tub | RM235 |
| Skirting 70mm x 8ft | piece | RM11/pcs |
| Skirting 100mm x 8ft | piece | RM13/pcs |
| Profile A/T/L x 9ft | piece | RM12/pcs |

Old-price uplift used for this example:

`+10%`

## Area and square-root method

When no room dimension is given, use quick square estimate:

| Formula | Result |
|---|---:|
| Side = sqrt(1044) | 32.31 ft |
| 4-side perimeter = 32.31 x 4 | 129.24 ft |

## Skirting calculation

Current price list skirting length is 8ft/pcs, not 9ft/pcs.

| Formula | Result |
|---|---:|
| Perimeter | 129.24 ft |
| Add 10% wastage | 142.17 ft |
| Divide by 8ft stock length | 17.77 pcs |
| Round up order quantity | 18 pcs |

Skirting cost:

| Option | Qty | Base price | Base amount | +10% old-price amount |
|---|---:|---:|---:|---:|
| 70mm skirting x 8ft | 18 pcs | RM11 | RM198.00 | RM217.80 |
| 100mm skirting x 8ft | 18 pcs | RM13 | RM234.00 | RM257.40 |

Default cheaper option:

`70mm skirting = 18 pcs = RM217.80 with +10% uplift`

## Door / profile calculation

If exact door count is unknown, use safe standard estimate.

For a 1044 sqft house, use up to 8 door openings as a maximum practical allowance unless the floor plan shows more.

| Formula | Result |
|---|---:|
| Door count allowance | 8 doors |
| Door width allowance | 3ft/door |
| Total profile length | 24ft |
| Add 10% wastage | 26.40ft |
| Divide by 9ft profile stock length | 2.93 pcs |
| Round up order quantity | 3 pcs |

Profile cost:

| Item | Qty | Base price | Base amount | +10% old-price amount |
|---|---:|---:|---:|---:|
| Profile A/T/L x 9ft | 3 pcs | RM12 | RM36.00 | RM39.60 |

## Floor material box calculation

Floor area with 10% wastage:

`1044 sqft x 1.10 = 1148.40 sqft`

Round up by full box because supplier does not sell exact small loose sqft.

| Product | Coverage | Box qty | Base amount | +5% | +10% |
|---|---:|---:|---:|---:|---:|
| 4.5mm SPC | 24.16 sqft/box | 48 boxes | RM3,307.20 | RM3,472.56 | RM3,637.92 |
| 5.5mm SPC | 19.33 sqft/box | 60 boxes | RM3,714.00 | RM3,899.70 | RM4,085.40 |
| 6mm SPC | 19.27 sqft/box | 60 boxes | RM4,626.00 | RM4,857.30 | RM5,088.60 |
| 5.5mm SPC Herringbone | 17.63 sqft/box | 66 boxes | RM5,068.80 | RM5,322.24 | RM5,575.68 |
| 3mm Vinyl Square Tile | 36 sqft/box | 32 boxes | RM2,768.00 | RM2,906.40 | RM3,044.80 |
| 3mm Vinyl Tile | 36 sqft/box | 32 boxes | RM2,768.00 | RM2,906.40 | RM3,044.80 |

Cheapest SPC by current price reference and stock rounding:

`4.5mm SPC = 48 boxes = RM3,637.92 after +10% uplift`

Cheapest Vinyl by current price reference and stock rounding:

`3mm Vinyl = 32 boxes = RM3,044.80 after +10% uplift`

## Labour calculation

Owner example rate:

`RM1.20/sqft`

| Formula | Amount |
|---|---:|
| 1044 sqft x RM1.20/sqft | RM1,252.80 |

## Foam rule

For SPC:

- Ground floor: choose foam-backed / foam-included SPC product when available. If product includes foam, do not add separate foam cost.
- Upper floor: no separate foam by default unless product spec, acoustic requirement, or site requirement says otherwise.
- If foam must be separate, calculate by stock roll/box size only; do not price loose small sqft unless supplier sells it that way.

For Vinyl:

- Vinyl usually follows its system requirement. Glue-down vinyl needs glue.
- Foam is not added unless product/system specifically requires underlay.

## Glue rule

SPC:

- Do not include glue by default if click-system SPC is used.
- Include glue only for edge/profile/detail if needed.
- Small optional allowance can use 5kg tub.

Vinyl:

- Treat glue as required unless product says otherwise.
- Because price list has no glue coverage rate, use a practical stock allowance.
- For this 1044 sqft example, use 20kg glue tub as provisional full-area allowance.

Glue cost with +10% uplift:

| Item | Qty | Base amount | +10% amount |
|---|---:|---:|---:|
| Glue 5kg optional | 1 tub | RM85.00 | RM93.50 |
| Glue 20kg vinyl allowance | 1 tub | RM235.00 | RM258.50 |

## Package estimate examples

### Option A - Cheapest SPC, ground floor foam-included product assumption

| Item | Amount |
|---|---:|
| 4.5mm SPC, 48 boxes, +10% uplift | RM3,637.92 |
| 70mm skirting, 18 pcs, +10% uplift | RM217.80 |
| Profile A/T/L, 3 pcs, +10% uplift | RM39.60 |
| Installation labour, 1044 sqft x RM1.20 | RM1,252.80 |

Subtotal excluding optional glue:

`RM5,148.12`

If optional 5kg glue is required:

`RM5,241.62`

### Option B - Cheapest Vinyl, glue-down assumption

| Item | Amount |
|---|---:|
| 3mm Vinyl, 32 boxes, +10% uplift | RM3,044.80 |
| 70mm skirting, 18 pcs, +10% uplift | RM217.80 |
| Profile A/T/L, 3 pcs, +10% uplift | RM39.60 |
| Glue 20kg, +10% uplift | RM258.50 |
| Installation labour, 1044 sqft x RM1.20 | RM1,252.80 |

Subtotal:

`RM4,813.50`

## Important notes

- This calculation is working cost / material-and-labour estimate only. It is not customer selling price unless markup is added.
- Use 10% wastage for floor material, skirting and door/profile estimate.
- Use stock unit rounding: full box, full piece, full tub or full roll.
- If exact floor plan is available, replace the square-root perimeter estimate with actual room perimeter and actual door count.
- If customer asks for SPC, do not substitute Vinyl just because Vinyl is cheaper unless owner approves substitution.
