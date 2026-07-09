# GPT Header Renovation Addendum — SXX Final Cost and Contradiction Rule

This file records a permanent/general renovation workflow rule that must be merged into the next full replacement of:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt
```

## Rule: meaning of muktamad/final per SXX

For SXX costing, `muktamad` means final for the current SXX scope as an internal cost build-up, not necessarily customer selling price.

A SXX may be marked final/internal-cost complete only when:

- SPEC A:C is filled;
- Block 1, Block 2 and Block 3 are all filled;
- no required line is left as `NIL`, blank or unresolved;
- every missing root master item has been converted into an approved addendum/reference line;
- each rate is marked as `UNMARKED COST RATE`, `SELLING RATE USED`, `MARKUP INCLUDED`, or another clear rate basis;
- every SXX total states whether it is internal cost, cost with contingency, or customer selling price;
- markup/gross margin is not silently included or excluded.

## Rule: root Materials/Labour are unmarked cost unless marked otherwise

Root reference files such as:

```text
1.2 Materials.txt
1.3 Labour.txt
```

are treated as unmarked cost/reference rates by default unless the source line or owner explicitly states that markup/selling is already included.

If any SXX uses a rate that already includes markup, package margin, supplier selling margin or customer-facing selling price, the SXX must remark it clearly to prevent underquoting or overpricing.

## Rule: no SXX may remain hanging

Do not leave a SXX with `NIL`, blank or unresolved required cost lines.

If exact supplier quote is absent, GPT must use market/reference/addendum rates with clear status and update date, then mark the SXX as final internal cost for current scope. Later supplier quote or drawing contradiction triggers a correction/version update, not a stalled SXX.

## Rule: contradiction found later must trigger immediate correction

If any later SXX, drawing, supplier quote, owner correction or source evidence contradicts an earlier SXX, GPT must immediately create/update the correct versioned correction file before continuing too far.

The correction must prevent:

- double count;
- undercost;
- overprice;
- wrong markup assumption;
- duplicated preliminaries;
- item counted in wrong SXX;
- item omitted because another SXX was assumed to include it.

## Reason

Owner corrected that `provisional` caused confusion and wasted time. Each SXX must be completed to a usable internal cost level, with clear rate basis and immediate contradiction correction if later evidence changes the scope or price.
