# SPC Material Selection V1

## Source

Owner pointed to `AdditionalMaterials/SPC & Vynil` as the new SPC/Vinyl price reference and instructed to choose the cheaper SPC option.

A recent repository commit also records the earlier SPC price reference that was deleted from `AdditionalMaterials/SPC/PRICE.txt`; this is used only as trace evidence for the same material family until the current folder file can be listed directly by GitHub tools.

## Price options found

| Option | Coverage | Price | Approx RM/SF | Note |
|---|---:|---:|---:|---|
| 4.5mm SPC Flooring Virgin Material | 24.16 SF/box | RM68.90/box | RM2.85/SF | Cheapest SPC option found. |
| 5.5mm SPC Flooring Virgin Material | 19.33 SF/box | RM61.90/box | RM3.20/SF | Higher RM/SF than 4.5mm SPC. |
| 6mm SPC Flooring Virgin Material | 19.27 SF/box | RM77.10/box | RM4.00/SF | Higher RM/SF. |
| 5.5mm SPC Herringbone | 17.63 SF/box | RM76.80/box | RM4.36/SF approx | Decorative pattern; not cheapest. |
| 3mm Vinyl square tile | 36 SF/box | RM86.50/box | RM2.40/SF approx | Cheaper than SPC, but it is vinyl, not SPC. |
| 3mm Vinyl tile | 36 SF/box | RM86.50/box | RM2.40/SF approx | Cheaper than SPC, but it is vinyl, not SPC. |

## Selection

Selected item for customer SPC flooring:

`4.5mm SPC Flooring Virgin Material`

Selected rate:

`RM2.85/SF supply only`

Reason:

Customer requested SPC flooring. The 4.5mm SPC option is the cheapest SPC rate found. Vinyl is cheaper per SF but is not selected because it changes the material type from SPC to vinyl.

## ActiveBOQ estimate

Current provisional living hall area in `ActiveBOQ_Takeoff_Assumption_V1.tsv`:

`180 SF FLOORPLAN ESTIMATE`

SPC material supply estimate:

- 180 SF x RM2.85/SF = RM513.00

Recommended waste allowance for early budget:

- 10% waste = 198 SF order basis
- 198 SF x RM2.85/SF = RM564.30

Box estimate using 24.16 SF/box:

- 198 SF / 24.16 SF per box = 8.20 boxes
- Round up to 9 boxes
- 9 boxes x RM68.90 = RM620.10 supply only

## Not included in this material-only rate

- SPC installation labour;
- floor levelling;
- moisture treatment;
- old flooring hacking/removal;
- skirting;
- profiles/trims;
- adhesive/glue if required by selected system;
- delivery;
- wastage beyond the allowance;
- final colour/model selection.

## Next BOQ action

Use `4.5mm SPC Flooring Virgin Material` as provisional SPC material in `ActiveBOQ_Takeoff_Assumption_V2.tsv`.

Before final quotation, either:

1. add this item to `1.2 Materials.txt` through a controlled master-list update; or
2. keep it as an owner-approved provisional AdditionalMaterials quotation line.
