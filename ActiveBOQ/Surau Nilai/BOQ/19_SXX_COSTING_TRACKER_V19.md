# Surau Nilai — SXX Costing Tracker V19

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/18_SXX_COSTING_TRACKER_V18.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V19 correction note

Owner clarified the active requirement:

```text
100% means 100%.
99.9% means not solved.
No hanging Block 1 - Block 3 prices.
Do not continue to S09 unless S08 is truly 100% according to customer drawing/spec.
```

After this strict gate review, S08 V1 cannot be treated as 100% drawing/spec complete because it still contains refinable / verification / allowance items.

## Current gate

```text
CURRENT ACTIVE SXX: S08
S01 WORKING-COST BASIS: COMPLETE - KEEP FOR INTERNAL COST PLANNING
S01 BOQ.XLSM PASTE FILE: READY - WORKING-COST ONLY
S01 DRAWING/SPEC RESCAN: STILL REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ
S02 WORKING-COST BASIS: COMPLETE - KEEP FOR INTERNAL COST PLANNING
S02 BOQ.XLSM PASTE FILE: READY - WORKING-COST ONLY
S02 DRAWING/SPEC RESCAN: STILL REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ
S03 WORKING-COST BASIS: COMPLETE - KEEP FOR INTERNAL COST PLANNING
S03 BOQ.XLSM PASTE FILE: READY - WORKING-COST ONLY
S03 DRAWING/SPEC RESCAN: STILL REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ
S04 WORKING-COST DRAWING/SPEC BASIS: COMPLETE
S04 BOQ.XLSM PASTE FILE: READY - USE V2
S05 WORKING-COST DRAWING/SPEC BASIS: COMPLETE
S05 BOQ.XLSM PASTE FILE: READY - USE V1
S06 WORKING-COST DRAWING/SPEC BASIS: COMPLETE AFTER RECHECK - USE V2
S06 BOQ.XLSM PASTE FILE: READY - USE V2
S07 WORKING-COST DRAWING/SPEC BASIS: COMPLETE AFTER RECHECK - USE V1
S07 BOQ.XLSM PASTE FILE: READY - USE V1
S08 WORKING-COST DRAWING/SPEC BASIS: EXISTS BUT STRICT 100% GATE HOLD
S08 BOQ.XLSM PASTE FILE: V1 EXISTS BUT DO NOT USE AS STRICT 100% FINAL
S08 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S09 START ALLOWED UNDER STRICT 100% OWNER REQUEST: NO
```

## S08 strict gate review file

```text
ActiveBOQ/Surau Nilai/BOQ/S08_STRICT_100_PERCENT_GATE_REVIEW_V2.md
```

## Why S08 is blocked

The existing S08 V1 contains these unresolved / refinable points:

```text
Column height uses 3.0m height allowance.
RF beam length basis is compiled as 121.20m.
IRB beam length basis is compiled as 57.60m.
IRB is priced using 125x350 average to reduce undercost.
Reinforcement is a 1600kg working-cost basis and marked SUPPLIER/BBS VERIFICATION ITEM.
Concrete pump/access says supplier quote can replace later.
Scaffold bay and jack/U-head quantities say exact site staging / exact shoring design can refine.
```

Therefore S08 is not 100% settled under the owner's strict standard.

## S08 V1 cost status

S08 V1 remains as a reference working-cost file only:

```text
Block 1 material: RM17,740.76
Block 2 labour:   RM5,680.00
Block 3 service:  RM2,760.00
Base working cost: RM26,180.76
Optional 10% contingency: RM2,618.08
Working cost with contingency: RM28,798.84
Customer selling price: NOT READY - markup/gross margin not applied
```

Do not paste S08 V1 into final strict 100% workbook unless owner explicitly accepts it as working-cost basis only.

## SXX tracker

| SXX | Proposed scope | Working-cost status | BOQ.xlsm paste file | Drawing/spec status | Required source check | Notes |
|---|---|---|---|---|---|---|
| S01 | Preliminaries, mobilisation, setting out, hoarding and signboard | COMPLETE | `S01_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `Hoarding and Signboard 1.pdf`, site plan, survey | Existing base working cost RM8,750.00; optional 10% contingency RM875.00; with contingency RM9,625.00. No customer markup. |
| S02 | ESCP and temporary erosion/sediment control | COMPLETE | `S02_BOQXLSM_PASTE_READY_V2.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01ESCP-LP-01-S0-00.pdf` | Existing base working cost RM1,944.00; optional 10% contingency RM194.40; with contingency RM2,138.40. No customer markup. |
| S03 | Site clearing, earthwork, cut/fill and platform formation | COMPLETE | `S03_BOQXLSM_PASTE_READY_V1.txt` working-cost only | RESCAN REQUIRED BEFORE FINAL OVERALL CUSTOMER BOQ | `SJ_01EW-CS-01-S0-00.pdf`, `SJ_01EW-DT-01-S0-00.pdf`, `SJ_01EW-LP-01-S0-00.pdf`, site plan/survey | Existing base working cost RM2,090.00; optional 10% contingency RM209.00; with contingency RM2,299.00. No customer markup. |
| S04 | Crossing bridge and permanent site entrance | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S04_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `CROSSING BRIDGE.pdf` rendered and visually inspected | Base working cost RM36,004.11; optional 10% contingency RM3,600.41; with contingency RM39,604.52. No customer markup. V1 undercost superseded. |
| S05 | Building substructure: footing, stump and ground beam | COMPLETE - WORKING-COST DRAWING/SPEC BASIS | `S05_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `04-SURAU JERUSSALAM GROUND BEAM DETAIL 01.pdf`, `05-SURAU JERUSSALAM GROUND BEAM DETAIL 02.pdf` rendered and visually inspected | Base working cost RM31,089.07; optional 10% contingency RM3,108.91; with contingency RM34,197.98. No customer markup. |
| S06 | Under-slab plumbing, sewerage and drainage rough-in | COMPLETE AFTER RECHECK - WORKING-COST DRAWING/SPEC BASIS | `S06_BOQXLSM_PASTE_READY_V2.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `Surau Sanitary Plumbing Schematic 1.pdf`, `Surau Sewerage Schematic 1.pdf` rendered, visually inspected and text/word-position checked | V2 base working cost RM10,794.50; optional 10% contingency RM1,079.45; with contingency RM11,873.95. No customer markup. V1 undercount superseded. |
| S07 | Ground floor slab, apron, steps and ramps | COMPLETE AFTER RECHECK - WORKING-COST DRAWING/SPEC BASIS | `S07_BOQXLSM_PASTE_READY_V1.txt` | COMPLETE FOR NEXT SXX ON WORKING-COST DRAWING/SPEC PATH | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `02-SURAU JERUSSALAM SLAB SECTION 01.pdf`, `03-SURAU JERUSSALAM SLAB SECTION 02.pdf` rendered and visually inspected | Base working cost RM43,805.56; optional 10% contingency RM4,380.56; with contingency RM48,186.12. No customer markup. |
| S08 | Columns, RC frame/roof beams and superstructure structural RC | V1 EXISTS ONLY AS WORKING-COST BASIS | `S08_BOQXLSM_PASTE_READY_V1.txt` exists but HOLD for strict 100% | HOLD - STRICT 100% NOT COMPLETE | `01-SURAU JERUSSALAM LP-R02 Layout1.pdf`, `06-SURAU JURESSALAM ROOF BEAM DETAIL-R01 Model.pdf`, `07-SURAU JURESSALAM INT RF BEAM DETAIL-R01 Model.pdf` rendered and visually inspected | S08 V1 has allowance/refine-later items. Need S08 V2 strict takeoff or exact missing information before S09. |
| S09 | Roof framing, roof structure and roof covering interface | NOT STARTED | - | BLOCKED BY S08 STRICT 100% HOLD | `Roof Framing 1.pdf`, `Roof Framing.pdf`, roof layout/source drawings as needed | S09 cannot start under current owner strict 100% instruction until S08 is cleared. |

## Next action

```text
Do not start S09.
Resolve S08 strict 100% gate first.
Create S08 V2 only if exact beam/column/BBS/formwork/staging basis can be fully closed from drawing/spec without refine-later items.
```
