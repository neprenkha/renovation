# Surau Nilai — S01 Web Market Check / Finality Basis V1

Active SXX:

```text
S01 — Preliminaries, mobilisation, setting out, hoarding and signboard
```

Current S01 file:

```text
ActiveBOQ/Surau Nilai/BOQ/S01_Preliminaries_Takeoff_Block1-3_V4.txt
```

## Owner correction applied

`PROVISIONAL` must not mean missing price. If an item is required for S01, it must be filled with quantity, UOM, working rate, amount, markup status and audit note. No required S01 line may be NIL/blank merely because root master files lack an item.

## Web/current market check result

Web/current search was used for current-market reasonableness. Public search did not return a reliable exact Malaysia unit-rate source for this exact Surau Nilai combination:

- temporary hoarding material per metre;
- temporary hoarding installation per metre;
- project signboard 4ft x 8ft with construction-project requirements;
- temporary utility setup allowance.

Because exact public Malaysia unit-rate data was not reliable, S01 is finalised as `MUKTAMAD WORKING-COST BASIS` using:

- root `1.3 Labour.txt` for skilled/helper MH rates;
- `GPTEditable/Reference_Addendum/1.2_AdditionalMaterials_OnlineReference.txt` for missing material items;
- `GPTEditable/Reference_Addendum/1.3_AdditionalLabourServices_OnlineReference.txt` for missing labour/service items;
- explicit markup status per line;
- supplier quote remark where later commercial confirmation is needed.

## S01 status after correction

```text
S01 STATUS: COMPLETE FOR NEXT SXX - MUKTAMAD WORKING-COST BASIS
S01 BASE WORKING COST: RM8,750.00
S01 OPTIONAL 10% CONTINGENCY: RM875.00
S01 WORKING COST WITH CONTINGENCY: RM9,625.00
CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
```

## Markup status

Root `1.2 Materials.txt` and `1.3 Labour.txt` are treated as no-markup cost/working-rate references unless a line says otherwise.

S01 V4 states markup status on every line:

- `NO MARKUP - ROOT COST`;
- `NO MARKUP - ADDENDUM COST BASIS`;
- `NO MARKUP - WORKING COST`;
- customer selling price is not calculated.

## Cross-SXX correction rule

If S02 or any later SXX reveals contradiction, overlap, double count, undercost or overprice affecting S01, the affected SXX must be revised immediately as a new cumulative version before continuing.
