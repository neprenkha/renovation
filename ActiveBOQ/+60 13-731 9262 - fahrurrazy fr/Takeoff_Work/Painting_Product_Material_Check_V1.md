# Painting Product Material Check V1

## Purpose

Owner asked whether the painting amount already includes paint material, and whether the colour names in the customer request identify the paint brand.

## Customer colour wording

Customer request says:

`Cat (Vanilla latte/timeless)`

## Result

The current painting amount should be treated as labour/application working rate only unless a paint material line is added separately.

Reason:

- The current estimate used RM1.80/sqft as a generic painting rate.
- The previous correction did not separate topcoat paint, sealer/primer, sundries, tools or brand-grade material cost.
- There is no locked paint product/material line yet for Vanilla Latte or Timeless in the ActiveBOQ estimate.

Therefore, the current paint amount is not safely material-included.

## Brand / colour check

`Timeless` appears to match a Dulux paint colour name.

`Vanilla Latte` is not yet confirmed from the repo/source as a specific brand colour. Treat it as an unverified customer colour name until confirmed from customer colour chart, paint shop, or final selected product.

Do not assume Vanilla Latte and Timeless are from the same brand unless confirmed.

## Existing paint quantity from V1 correction

Known-area paint quantity from `Painting_Dimension_Correction_V1.md`:

`3,610.36 sqft`

Existing painting amount:

`3,610.36 sqft x RM1.80 = RM6,498.66`

Classify this as:

`Painting application / labour working amount`

## Provisional paint material quantity

Use this only for rough estimate until final product and paint coverage are confirmed.

Assumption:

- Two topcoat coats.
- One sealer/primer coat if needed.
- Approx 100 sqft/litre coverage for rough quantity planning.
- Use full pail rounding.

| Item | Formula | Provisional quantity |
|---|---|---:|
| Topcoat paint | 3,610.36 sqft x 2 coats / 100 sqft per litre | 72.21 litres |
| Topcoat pails | 72.21 / 18L | 5 pails if rounding safely |
| Sealer/primer | 3,610.36 sqft / 100 sqft per litre | 36.10 litres |
| Sealer/primer pails | 36.10 / 18L | 3 pails if rounding safely |

## Provisional material allowance

Because exact brand/product and current supplier price are not locked, use a provisional material allowance instead of pretending exact price is known.

Recommended provisional allowance:

`RM2,000`

This covers:

- topcoat paint allowance;
- sealer/primer allowance if needed;
- roller, tray, brush, masking, plastic protection, sandpaper and small sundries.

## Estimate impact

Previous V5 working cost:

`RM74,753.67`

Add provisional paint material allowance:

`RM2,000.00`

Revised working cost:

`RM76,753.67`

## Selling impact

| Option | Amount | Practical figure |
|---|---:|---:|
| 10 percent markup | RM84,429.04 | RM84,500 / RM85,000 |
| 15 percent markup | RM88,266.72 | RM88,500 / RM89,000 |
| 20 percent markup | RM92,104.40 | RM92,000 / RM93,000 |

## Recommendation

Use RM89,000 as the safer revised customer estimate if paint material is included.

Use RM86,000 only if owner confirms the RM1.80/sqft painting rate already includes paint material, sealer/primer and sundries.

Use RM93,000 if whole-house paint, premium paint grade or wider paint scope is expected.

## Final confirmation needed

Before final quotation, confirm:

1. Exact paint brand.
2. Exact product line, for example interior emulsion, easy-clean, premium, odourless, anti-mould.
3. Exact colour code for Vanilla Latte.
4. Exact colour code for Timeless.
5. Whether ceiling paint is same product or separate ceiling white.
6. Whether primer/sealer is required on existing wall condition.
