# Surau Nilai — SXX Costing Tracker V30

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/29_SXX_COSTING_TRACKER_V29.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V30 note — S14 road and drainage strict recheck

Owner requested S14 to be repeatedly checked so that it can be taken off at 100% current BOQ cost basis and proceed to S15 only if it passes.

Latest owner uploaded header checked:

```text
GPTRenovationHeader.txt
Generated MYT: 2026-07-10 07:00
```

Owner repeated the strict gate:

```text
Take off to next SXX is only allowed at 100%.
99.9% is not a pass.
```

For S14, the active 100% target is:

```text
Current BOQ cost basis complete using customer road/drainage drawings and customer/drawing accepted full allowance basis.
Customer selling price/margin is separate and not part of the current 100% target unless owner explicitly asks for selling price.
```

## S14 source checked

```text
SJ_02R&D-LP-01-S0-01.pdf
SJ_02R&D-DT-02-S0-00.pdf
Surau Plan Roof Plan Bldg Tender_Constn.pdf
S09 roof rainwater goods boundary
S03 earthwork boundary
S04 crossing bridge/permanent entrance boundary
S06 plumbing/sewer rough-in boundary
```

## S14 drawing/spec facts

```text
Drawing title: ROAD AND DRAIN
Drawing no: SJ/RD/LP/01
Scale: 1:200 (A1)
Legend includes proposed premix road, proposed kerb, 375mm wide drain with 225mm HRGW, 200mm diameter subsoil drain, S1 - 1200 x 1200 brick sump, DO - drain opening and entrance culvert.

Drawing title: ROAD & DRAINAGE - SUBSOIL DRAIN DETAILS
Drawing no: SJ/RD/DT/02
Details include on-field trench design, off-field trench design, T-joint, bend, straight joint, anchor rod detail and jointing to sump.
```

## S14 active files

```text
Rate reference:
ActiveBOQ/Surau Nilai/BOQ/S14_RoadDrainage_RateReference_V1.txt

Repeated recheck file:
ActiveBOQ/Surau Nilai/BOQ/S14_RoadDrainage_Recheck_Audit_V1.md

Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S14_RoadDrainage_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S14_BOQXLSM_PASTE_READY_V1.txt
```

Only `S14_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm` for S14.

## S14 quantity basis

| Item | Quantity basis | S14 current BOQ quantity |
|---|---|---:|
| Proposed premix road / parking / hardstanding | Drawing yellow road/parking/hardstanding full allowance | 430 m2 |
| Proposed kerb | Kerb around proposed premix road/parking edge full allowance | 155 m |
| 375mm wide drain with 225mm HRGW | Blue drain route around road/site perimeter and discharge path full allowance | 145 m |
| 200mm diameter subsoil drain | Subsoil drain route shown by dashed/blue drainage line full allowance | 110 m |
| S1 1200 x 1200 brick sump | S1 sump points visible at drain/culvert/perimeter positions | 4 nos |
| DO drain opening | Drain opening points at entrance/drain interface | 2 nos |
| Entrance culvert | Entrance culvert crossing length allowance | 6 m |
| RWDP ground connection | Connection from S09 rainwater downpipe discharge to S14 ground drain | 4 points |
| Road marking | Parking bay/direction marking over premix road/hardstanding | 1 lot |
| Excavation/backfill/disposal | S14 road/drain trenching and making-good | 1 lot |
| Plant | Backhoe/roller/plate compactor/drainage plant | 1 lot |
| Flushing/testing/cleaning | Drainage final flow check/cleaning | 1 lot |

## S14 cost summary

```text
Block 1 material: RM70,110.00
Block 2 labour:   RM25,095.00
Block 3 service:  RM21,950.00
Base working cost: RM117,155.00
Optional 10% contingency: RM11,715.50
Working cost with contingency: RM128,870.50
Customer selling price: NOT READY - markup/gross margin not applied
```

## S14 strict gate checklist

```text
Road and drainage source checked: PASS
Premix road included: PASS
Kerb included: PASS
375mm drain + 225mm HRGW included: PASS
200mm subsoil drain included: PASS
S1 sump included: PASS
DO drain opening included: PASS
Entrance culvert included: PASS
RWDP ground connection included: PASS
S03 duplicate prevention: PASS
S04 duplicate prevention: PASS
S06 duplicate prevention: PASS
S09 duplicate prevention: PASS
Block 1 complete: PASS
Block 2 complete: PASS
Block 3 complete: PASS
Markup check: PASS
100% / 99.9% gate: PASS
```

## Current gate

```text
CURRENT ACTIVE SXX: S15
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
S08 COMPLETE FOR NEXT SXX - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS
S08 BOQ.XLSM PASTE FILE: READY - USE V2
S09 COMPLETE FOR NEXT SXX - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS
S09 BOQ.XLSM PASTE FILE: READY - USE V1
S10 COMPLETE FOR NEXT SXX - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS
S10 BOQ.XLSM PASTE FILE: READY - USE V1
S11 STRICT 100% CURRENT BOQ COST BASIS: PASS
S11 ACTIVE ALUMINIUM/GLASS SCHEDULE: USE V2
S11 ACTIVE AUDIT FILE: USE V3
S11 ACTIVE BOQ.XLSM PASTE FILE: USE V2
S12 STRICT 100% CURRENT BOQ COST BASIS: PASS
S12 ACTIVE AUDIT FILE: USE V1
S12 ACTIVE BOQ.XLSM PASTE FILE: USE V1
S13 WORKING-COST ESTIMATE COMPLETE - OWNER ACCEPTED PREMIUM-SENSIBLE SIZE-BASED PROVISIONAL PATH
S13 ACTIVE AUDIT FILE: USE V2
S13 ACTIVE BOQ.XLSM PASTE FILE: USE V2
S13 DRAWING-SPEC EXACT ELECTRICAL DESIGN: HOLD UNTIL DEDICATED ELECTRICAL DRAWING / OWNER CONFIRMED ELECTRICAL SCHEDULE
S14 STRICT 100% CURRENT BOQ COST BASIS: PASS
S14 ACTIVE AUDIT FILE: USE V1
S14 ACTIVE BOQ.XLSM PASTE FILE: USE V1
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S06 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S07 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S08 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S09 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S10 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S11 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S12 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S13 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S14 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S15 START ALLOWED: YES - CURRENT BOQ 100% COST BASIS PATH
```

## Header update decision

No new header update is required because the latest uploaded `GPTRenovationHeader.txt` already contains:

```text
13D Drawing-spec SXX completion gate
13E Authorised allowance / 100% current BOQ cost basis rule
```

## Next action

Proceed to S15 on current BOQ 100% cost basis path:

```text
S15_Fencing_Gate_ExternalSecurity_or_next_scope_Takeoff_Audit_V1.txt
S15_BOQXLSM_PASTE_READY_V1.txt
31_SXX_COSTING_TRACKER_V31.md
```
