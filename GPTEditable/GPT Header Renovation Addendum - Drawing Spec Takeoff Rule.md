# GPT Header Renovation Addendum — Drawing Spec Takeoff Rule

This file records a permanent/general renovation workflow rule that must be merged into the next full replacement of:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt
```

## Rule: drawing/customer source is the specification source

For project/customer work, the active job `Drawing/` folder is not optional background material. It is the customer's requested specification/source of truth for takeoff and BOQ.

For Surau Nilai, the drawing folder is:

```text
ActiveBOQ/Surau Nilai/Drawing/
```

Those drawings are read-only source files. GPT must not edit, rename, move, overwrite or delete them.

## Rule: takeoff must be auditable by other people/sessions

Takeoff does not mean only a private understanding by GPT or the current chat.

A valid takeoff must be understandable and auditable by:

- the owner;
- QS;
- contractor;
- future GPT session;
- future reviewer.

Each takeoff item must record enough detail to re-check it later:

- SXX scope and trade;
- source drawing filename;
- sheet/title/revision/page where visible;
- exact measured element/location;
- dimension source;
- calculation formula;
- raw quantity;
- deductions;
- net quantity;
- UOM;
- wastage;
- buffer/contingency if any;
- master material/labour/addendum reference;
- status: measured, drawing-derived, owner-corrected, provisional, supplier quote needed, or conflict.

If a line cannot be audited later, it is not a complete takeoff line.

## Rule: no missing drawing/spec item

Before a final SXX or overall BOQ is claimed, GPT must prove that all relevant drawings/specs were checked for that SXX.

For Surau Nilai, GPT must maintain a drawing register and show which drawings affect each SXX. If a drawing cannot be read or rendered, mark it clearly as `UNREADABLE / NEEDS REVIEW`; do not silently ignore it.

## Rule: previous session and owner corrections are source evidence

Before asking the owner a question or claiming an item is unknown, GPT must check:

1. current owner instruction;
2. uploaded/current `GPTRenovationHeader.txt`;
3. GitHub canonical header / GPTEditable files;
4. active workspace files;
5. previous session discussion captured in this chat/context;
6. drawing/source files;
7. README/material/labour/addendum references.

For Surau Nilai, previous-session corrections include the governing project identity/lot correction: use `Lot 20093` as the governing working lot unless a later owner instruction changes it. If a drawing shows a conflicting lot number, record it as a drawing/source conflict instead of silently reverting to the wrong lot.

## Rule: hoarding/preliminaries

If drawings or customer requirements include hoarding/signboard/preliminaries, S01 must include them. If exact length/type is not yet confirmed, S01 may use clearly-marked provisional takeoff, but final S01 must later reconcile against drawing/site boundary/source evidence.

## Reason

Owner corrected that S01/takeoff must not be treated as a casual session understanding. The drawing folder contains customer-requested specs, and takeoff must be complete enough for owner/QS/future sessions to understand and audit.
