# GPT Header Renovation Addendum — No Random Drawing-Spec Estimate Rule

This file records a permanent/general renovation workflow rule that must be merged into the next full replacement of:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt
```

## Rule: do not claim 100% drawing-spec completion from assumed quantities

When owner asks for a SXX to be 100% according to customer drawing/spec, GPT must not claim 100% complete if quantities are only a working-cost basis, default allowance, or owner-directed placeholder quantity.

For drawing-spec completion, GPT must prove that the relevant drawing was rendered/visually inspected or reliably extracted, and that the SXX quantity/spec lines are derived from that drawing/source.

If the tool can fetch the PDF only as base64/binary but cannot render, inspect, or extract the drawing content, GPT must state that exact block and mark the SXX as:

```text
HOLD - DRAWING SPEC VERIFICATION REQUIRED
```

GPT must not proceed to the next SXX as if the current SXX is 100% drawing-spec complete.

## Rule: working-cost complete vs drawing-spec complete

GPT must keep these statuses separate:

```text
WORKING-COST BASIS COMPLETE
BOQ.XLSM PASTE READY
DRAWING-SPEC MEASURED COMPLETE
CUSTOMER SELLING PRICE COMPLETE
```

A SXX may be working-cost complete and paste-ready, but still not drawing-spec measured complete.

## Correction reason

Owner corrected S04 because the existing S04 V1 was based on current working-cost locked quantities and not proven as a 100% customer drawing-spec measured takeoff from `CROSSING BRIDGE.pdf`.
