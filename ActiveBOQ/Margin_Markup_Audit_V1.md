# Margin Markup Audit V1

## Audit question

Owner asked whether the current RM39,000 customer figure already includes margin or markup.

## Result

No clear margin or markup was included.

`ActiveBOQ_Full_Estimate_V1.tsv` is a working cost / provisional pricing summary. It rounds the working total to RM39,000, but it does not apply a defined profit margin, markup percentage, overhead allowance, or risk margin.

## Evidence from current files

Current working total excluding optional glue:

`RM38,748.21`

Rounded customer figure used earlier:

`RM39,000`

Difference:

`RM251.79`

This is only about:

`0.65%` above the working total.

Therefore the RM39,000 figure is only a rounded budget figure, not a real markup.

If optional SPC glue is required:

`RM38,841.71`

Difference to RM39,000:

`RM158.29`

This is only about:

`0.41%` above the working total.

## Classification

| Item | Current status |
|---|---|
| `ActiveBOQ_Full_Estimate_V1.tsv` | Working cost / provisional estimate. |
| `Customer_Quotation_Draft_V2.md` | Customer budget draft based on that working cost. |
| RM39,000 rounded figure | Not margin-protected. |
| Cabinet rates | Provisional package rates; margin status not separately proven. |
| Electrical rates | Based on Labour master rates; treated as working cost unless owner says these are selling rates. |
| SPC | Material cost with old-price uplift + installation labour; not overall project margin. |

## Selling price options from working cost

Using working cost RM38,748.21:

| Markup on cost | Selling amount | Practical customer figure |
|---:|---:|---:|
| 10% | RM42,623.03 | RM43,000 |
| 15% | RM44,560.44 | RM45,000 |
| 20% | RM46,497.85 | RM46,500 / RM47,000 |

Using working cost with optional glue RM38,841.71:

| Markup on cost | Selling amount | Practical customer figure |
|---:|---:|---:|
| 10% | RM42,725.88 | RM43,000 |
| 15% | RM44,667.97 | RM45,000 |
| 20% | RM46,610.05 | RM47,000 |

## Recommendation

Do not issue RM39,000 as the customer selling quotation if the owner wants margin/markup protected.

Use:

- `RM43,000` as minimum customer selling figure with about 10% markup on current working cost;
- `RM45,000` as safer customer selling figure with about 15% markup;
- `RM47,000` if owner wants around 20% markup or more risk allowance.

## Required correction

Create `Customer_Quotation_Draft_V3.md` so the customer-facing draft no longer presents RM39,000 as the main quotation figure without explaining that it was only a cost-based rough budget.
