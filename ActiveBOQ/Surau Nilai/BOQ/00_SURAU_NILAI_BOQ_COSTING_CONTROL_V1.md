# Surau Nilai — BOQ Costing Control V1

Generated for active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## Purpose

This file creates and controls the Surau Nilai `BOQ/` working folder for pricing and overall project cost build-up.

This folder is for customer estimate, BOQ, supplier pricing files, SXX cost build-up and final summary files only.

## Hard workspace boundary

Writable BOQ folder:

```text
ActiveBOQ/Surau Nilai/BOQ/
```

Related writable work folders:

```text
ActiveBOQ/Surau Nilai/Takeoff_Work/
ActiveBOQ/Surau Nilai/BOQ_work/
ActiveBOQ/Surau Nilai/GPT_CONTROL/
```

Read-only source folders:

```text
ActiveBOQ/Surau Nilai/Drawing/
ActiveBOQ/Surau Nilai/OriginalFile/
```

Do not edit, rename, move, overwrite or delete anything in `Drawing/` or `OriginalFile/`.

Do not write generated Surau Nilai files directly under `ActiveBOQ/`.

Do not write Surau Nilai files inside another ActiveBOQ customer/site folder.

## Pricing workflow

Do not jump straight to one final lump-sum price.

Required order:

```text
Deep Read Register
-> Scope Sequence S01-SXX
-> S01 SPEC + Cost
-> S01 Check
-> S02 SPEC + Cost
-> S02 Check
-> continue by construction sequence
-> Overall Cost Summary
```

Every SXX must be completed or formally reserved before starting the next SXX.

Completion status allowed:

| Status | Meaning |
|---|---|
| `NOT STARTED` | SXX not yet read/measured/priced |
| `IN PROGRESS` | SXX started but not checked |
| `COMPLETE FOR NEXT SXX` | measured, costed, checked and ready to proceed |
| `RESERVED WITH REASON` | sequence exists but cannot be priced yet because input is genuinely absent |
| `HOLD - CONFLICT` | source conflict prevents reliable pricing |

## Master references

Use repository root references as read-only sources:

```text
README - BOQ.txt
1.2 Materials.txt
1.3 Labour.txt
```

Rules:

- Material Description and UOM must match `1.2 Materials.txt` exactly when a matching item exists.
- Labour / plant / rental / service Description and UOM must match `1.3 Labour.txt` exactly when a matching item exists.
- If no exact master item exists, do not invent a final BOQ master name silently.
- Record missing items in the SXX costing file and prepare a missing-master/provisional-rate note inside the allowed Surau Nilai work folder.
- Do not edit root master lists unless owner explicitly asks to update that exact file.

## Cost blocks

Every SXX costing file must separate:

| Block | Meaning |
|---|---|
| Block 1 | Material / product / consumable purchase |
| Block 2 | Labour / own work / plant / rental / productivity-based work |
| Block 3 | External subcontract / specialist / supplier complete package |

Do not place own-work material into Block 3 only because it is easier.

Do not split true subcontract complete-package items into fake material/labour unless supplier scope requires it.

## Wastage, buffer and rounding

Every SXX must show:

- raw measured quantity;
- deduction;
- net quantity;
- wastage percentage or fixed allowance;
- purchase quantity after wastage;
- practical supplier rounding;
- buffer / contingency separately from wastage.

Wastage is for physical material loss, cutting, laps, breakage, overlaps and practical installation loss.

Buffer/contingency is commercial/site-risk allowance and must not be hidden inside measured quantity.

Round after wastage to the correct stock unit, such as:

- BAG;
- PCS;
- LENGTH;
- SHEET;
- BOX;
- ROLL;
- TRIP;
- M3;
- M2;
- LOT;
- DAY;
- HOUR;
- WORKER-DAY.

## MH productivity rule

Where labour is not a fixed master-list package rate, every SXX costing file must show manpower-hour or productivity basis.

Minimum required fields:

- trade / worker type;
- crew size;
- productivity rate per hour or per day;
- calculated duration;
- total man-hours or worker-days;
- labour rate source;
- total labour cost status.

Do not write only a labour total without explaining productivity when the total is derived from crew output.

## Price status rule

Every SXX total and overall total must state one of:

- `WORKING COST`;
- `PROVISIONAL COST`;
- `SELLING RATE USED`;
- `CUSTOMER SELLING PRICE`.

Do not call a figure customer-ready unless markup or margin is explicitly calculated.

## Surau Nilai immediate rule

Surau Nilai must not proceed to final overall price until:

1. all 24 Drawing PDFs are deep-read / visually inspected;
2. the drawing register is created;
3. the S01-SXX scope sequence is locked;
4. each SXX is priced and checked sequentially;
5. reserved/provisional items are clearly labelled.

First BOQ-related working file after this control file should be the costing tracker.
