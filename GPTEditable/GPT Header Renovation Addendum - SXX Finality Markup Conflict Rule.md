# GPT Header Renovation Addendum — SXX Finality / Markup / Conflict Rule

This file records a permanent/general renovation workflow rule that must be merged into the next full replacement of:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt
```

## SXX finality / no-hanging-cost rule

For each SXX, GPT must complete the SXX as a muktamad working-cost basis before moving to the next SXX.

`PROVISIONAL` must not be used merely because GPT has not found a material/labour price. If a root master item is missing, GPT must use web/current search, approved addendum reference, logical working-cost basis, or supplier-needed remark and still fill the SXX line.

A line may be marked `SUPPLIER QUOTE NEEDED` for later commercial confirmation, but the SXX cannot be left hanging: quantity, UOM, working rate basis, amount, markup status and audit note must still be filled.

Use `PROVISIONAL` only for real unresolved design/source conflicts, drawing unreadability, or owner scope decisions that cannot be resolved from existing material. The exact reason must be written.

## Markup / selling-rate rule

Root master files `1.2 Materials.txt` and `1.3 Labour.txt` are treated as cost / unmarked-up working rates unless the line itself states otherwise.

Every SXX rate line must state its markup status:

- `NO MARKUP - ROOT COST`;
- `NO MARKUP - ADDENDUM COST BASIS`;
- `MARKET CHECKED - NO MARKUP WORKING COST`;
- `SELLING RATE USED`;
- `MARKUP INCLUDED / DO NOT MARK UP AGAIN`;
- `SUPPLIER QUOTE NEEDED BEFORE CUSTOMER PRICE`.

If a rate appears to be a retail package, subcontract complete rate, selling rate, or already-marked-up rate, GPT must remark it clearly to avoid double markup, underquote or overprice.

## Cross-SXX contradiction / double-count rule

When working on any later SXX, if GPT finds a contradiction, overlap, duplicate scope, missing scope, undercost risk or overprice risk affecting a previous SXX, GPT must stop and revise the affected SXX first.

Required correction workflow:

1. create the next cumulative version of the affected SXX file;
2. preserve useful content from the previous version;
3. correct the double count / undercount / rate status / markup note;
4. update the SXX tracker;
5. update any overall summary if it already exists;
6. only then continue to the current SXX.

Do not wait until the end of the project to fix a known contradiction.

## Reason

Owner corrected that every SXX must be muktamad for its working-cost basis, must not leave missing prices as provisional, and must immediately correct any contradiction/double-count/undercost/overprice discovered in later SXX stages.
