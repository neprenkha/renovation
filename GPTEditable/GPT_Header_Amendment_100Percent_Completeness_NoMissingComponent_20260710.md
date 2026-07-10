# GPT Header Amendment — 100% Completeness / Logical Estimate / No Missing Component

Generated MYT: 2026-07-10 19:25

Repository:

```text
neprenkha/renovation
```

Applies to:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt owner local full replacement
```

## Owner correction captured

Owner clarified that the `100% / 99.9% gate` must not be misunderstood.

`100%` means the current BOQ cost basis must be complete and correct for the available drawing/spec/customer information. If data is incomplete or unclear, GPT may use a logical, buildable and suitably complete estimate/allowance, but every required component and rate must still be included.

`99.9%` means fail when any known component, required price/rate, explicit drawing dimension, or buildable accessory/work item is missing or wrong.

## Permanent rule to merge as Section 13G

```text
====================================================================
13G) 100% COMPLETENESS / LOGICAL ESTIMATE / NO-MISSING-COMPONENT RULE
====================================================================

When owner says `100%`, `99.9% is fail`, `betul ikut drawing/spec`, or equivalent, GPT must interpret this as a completeness and correctness gate for the current BOQ cost basis.

`100%` does NOT mean GPT must always have perfect supplier pricing or exact final customer-selected design for every unclear item. It means:
- every visible or required scope component has been counted or logically allowed for;
- every item that needs a material/product/labour/service/plant/rental rate has a rate or a clearly marked accepted provisional/logical rate;
- no known quantity, item, fitting, accessory, cable, switch, elbow, hack/making-good, fixing, sealant, plant, labour or service component is silently missing;
- explicit drawing dimensions/specifications are followed exactly;
- unclear or missing drawing data is closed with a logical, buildable and suitably complete allowance instead of leaving a gap;
- the calculation basis is recorded so future review can see whether the line is exact, drawing-derived, owner-accepted, logical provisional, supplier-needed, or future replacement only.

If a drawing clearly states a size/spec/quantity, GPT must not change it. Example: if the drawing states a window is 10ft x 7ft, pricing it as 10ft x 6ft is a fail unless a later owner/customer correction changes the size.

If the drawing does not state or does not clearly show the size/spec/quantity, GPT may use a logical size/spec/rate that is common, buildable and suitable for the project quality level. For Surau Nilai, where the building has premium aluminium/glass/Breezeway cues, the logical allowance should be premium-sensible and may intentionally be slightly complete/over-provided to prevent undercost.

For estimate-based scopes such as S13 electrical/M&E, a SXX can pass the current 100% working-cost basis when the estimate includes all normal complete components for a building of that size and quality, including but not limited to points, lights, fans, sockets, switches, isolators, cabling, conduits/trunking, fittings, DB/protection, earthing, accessories, hacking/making-good where relevant, testing, commissioning, labour and service items. It must not omit an obvious required item merely because exact final design is unavailable.

A SXX fails the 100% gate if:
- any visible/required component is not counted or not logically allowed for;
- a required material/product/labour/service line has no rate and no accepted provisional/logical rate;
- a drawing-explicit size/spec/quantity is copied incorrectly;
- a line count is incomplete, for example pricing only 9 lights when the takeoff requires 10 lights;
- accessories/fittings/labour/making-good required to make the item buildable are omitted without clear exclusion;
- unsupported/random allowance is used only to hide missing measurement or missing rates;
- a future supplier/design update is used as an excuse to leave the current BOQ cost basis incomplete.

A later actual supplier quotation, final M&E drawing, customer-selected brand, or markup/gross-margin stage may replace a current logical/provisional rate, but it must be recorded as a future replacement only. It must not block SXX continuity when the owner has accepted the current logical complete working-cost basis.

Before moving to the next SXX under this rule, GPT must record:
- explicit drawing data followed exactly where available;
- unclear/missing data closed by logical allowance where needed;
- all required components included;
- all required rates present or accepted as provisional/logical;
- no missing item/rate/component remains;
- undercost/overprice/double-count checks completed;
- whether future actual-price/design replacement is only a future update and not a current blocker.
```

## Immediate execution rule

Until the full canonical header merge is completed safely, GPT must still obey this amendment as active governance for Surau Nilai and all future SXX costing.

## Owner local header

A full owner local `GPTRenovationHeader.txt` replacement must be produced from the latest uploaded full owner header and include Section 13G without deleting old valid rules.
