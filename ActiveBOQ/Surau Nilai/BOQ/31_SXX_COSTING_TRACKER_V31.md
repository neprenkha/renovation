# Surau Nilai — SXX Costing Tracker V31

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/30_SXX_COSTING_TRACKER_V30.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V31 note — S15 fencing and gate strict recheck

Owner requested S15 to be repeatedly checked so that it can be taken off at 100% current BOQ cost basis and proceed to S16 only if it passes.

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

For S15, the active 100% target is:

```text
Current BOQ cost basis complete using customer fencing/gate drawing and customer/drawing accepted full allowance basis.
Customer selling price/margin is separate and not part of the current 100% target unless owner explicitly asks for selling price.
```

## S15 source checked

```text
Fencing and Gate 1.pdf
```

Rendered and visually inspected:

```text
Elevation from road outside
Plan
Sectional details
Fencing section
Title block: Fencing and Gate
Scale: 1:50
```

## S15 drawing/spec facts

```text
Total front gate/fencing structure width basis from plan: 4431mm + 10883mm + 4172mm = 19486mm = 19.486m.
Main gate width shown on plan: 10883mm.
Left side structure/fence run shown: 4431mm split 2462mm + 1969mm.
Right side structure/fence run shown: 4172mm split 2086mm + 2086mm.
Anti-climb fencing noted to manufacturer's detail.
Main gate / metalwork to manufacturer's detail.
Two 900 x 700mm metal door locations are noted.
Meter/inspection panel shown in right enclosure.
Facing brick brick post note shown.
200 x 200mm ceramic wall and floor tiles note shown.
Drainage outlet shown.
Electrical meter and water meter positions shown.
MS grating to engineer detail shown.
Fencing section shown with post/footing/plinth basis.
```

## S15 active files

```text
Rate reference:
ActiveBOQ/Surau Nilai/BOQ/S15_FencingGate_RateReference_V1.txt

Repeated recheck file:
ActiveBOQ/Surau Nilai/BOQ/S15_FencingGate_Recheck_Audit_V1.md

Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S15_FencingGate_Takeoff_Audit_V1.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S15_BOQXLSM_PASTE_READY_V1.txt
```

Only `S15_BOQXLSM_PASTE_READY_V1.txt` should be copied into `*BOQ.xlsm` for S15.

## S15 quantity basis

| Item | Quantity basis | S15 current BOQ quantity |
|---|---|---:|
| Total gate/frontage length | 4431 + 10883 + 4172 = 19486mm | 19.486m |
| Main vehicle gate | 10883mm width x 2073mm height drawing/elevation allowance | 22.56m2 |
| Anti-climb fence panels | Left/right front fencing length 4431 + 4172 = 8603mm x 1827mm height allowance | 15.72m2 |
| Facing brick posts / wall / meter-bin enclosures | Drawing-derived full allowance for posts, side enclosures and returns | 28.00m2 |
| RC footing/plinth/coping/base | Full frontage structural base allowance | 19.50m |
| 900 x 700mm metal doors | Door notes at bin/meter enclosure | 2 sets |
| Meter / inspection panel | Right enclosure inspection/glass/metal panel allowance | 1 set |
| 200 x 200 ceramic wall/floor tile | Bin/meter enclosure floor and wall finish full allowance | 35.00m2 |
| Drainage outlet | Gate/bin drainage outlet shown | 1 point |
| MS grating | Plan note to engineer detail | 1 set |
| Meter interface sundries | Electrical/water meter enclosure and sleeve/interface | 1 lot |

## S15 cost summary

```text
Block 1 material: RM38,602.20
Block 2 labour:   RM13,323.30
Block 3 service:  RM6,650.00
Base working cost: RM58,575.50
Optional 10% contingency: RM5,857.55
Working cost with contingency: RM64,433.05
Customer selling price: NOT READY - markup/gross margin not applied
```

## S15 strict gate checklist

```text
Source drawing rendered/visually checked: PASS
Frontage/gate dimensions checked: PASS
Main gate included: PASS
Anti-climb fence included: PASS
Gate/fence structural base included: PASS
Brick posts / enclosure walls included: PASS
Metal doors / inspection panel included: PASS
Tile finish included: PASS
Drainage outlet / MS grating included: PASS
Meter interface included: PASS
S01 duplicate prevention: PASS
S04 duplicate prevention: PASS
S14 duplicate prevention: PASS
S13 duplicate prevention: PASS
Block 1 complete: PASS
Block 2 complete: PASS
Block 3 complete: PASS
Markup check: PASS
100% / 99.9% gate: PASS
```

## Current gate

```text
CURRENT ACTIVE SXX: S16
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
S15 STRICT 100% CURRENT BOQ COST BASIS: PASS
S15 ACTIVE AUDIT FILE: USE V1
S15 ACTIVE BOQ.XLSM PASTE FILE: USE V1
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
S15 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S16 START ALLOWED: YES - CURRENT BOQ 100% COST BASIS PATH
```

## Header update decision

No new header update is required because the latest uploaded `GPTRenovationHeader.txt` already contains:

```text
13D Drawing-spec SXX completion gate
13E Authorised allowance / 100% current BOQ cost basis rule
13F Aluminium / Glass / Door-Window Spec Schedule Rule
```

## Next action

Proceed to S16 on current BOQ 100% cost basis path:

```text
S16_FinalExternalWorks_Signage_SiteFurniture_or_next_scope_Takeoff_Audit_V1.txt
S16_BOQXLSM_PASTE_READY_V1.txt
32_SXX_COSTING_TRACKER_V32.md
```
