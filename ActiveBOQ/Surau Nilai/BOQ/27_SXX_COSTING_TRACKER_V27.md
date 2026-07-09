# Surau Nilai — SXX Costing Tracker V27

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/26_SXX_COSTING_TRACKER_V26.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V27 note — S13 strict 100 recheck HOLD

Owner uploaded/latest header checked:

```text
GPTRenovationHeader.txt
Generated MYT: 2026-07-10 07:00
```

Owner repeated the strict gate:

```text
Take off to next SXX is only allowed at 100%.
99.9% is not a pass.
```

For this SXX workflow, the active 100% target remains:

```text
Current BOQ cost basis complete for the SXX, using customer drawing/spec and/or authorised customer/README/owner accepted full allowance basis.
Customer selling price/margin is separate and not part of the current 100% target unless owner explicitly asks for selling price.
```

## S13 strict recheck file

```text
ActiveBOQ/Surau Nilai/BOQ/S13_Electrical_Lighting_Power_Mechanical_Strict100_Recheck_HOLD_V1.md
```

Decision:

```text
S13 STRICT 100% CURRENT BOQ COST BASIS: HOLD
S13 BOQ.XLSM PASTE FILE: NOT CREATED
S13 COST TOTAL: NOT CLOSED
S14 START ALLOWED: NO
```

## S13 source search/check performed

S13 electrical/source search was performed for:

```text
electrical
lighting
power
socket
switch
DB
distribution board
EL
KS
fan
lamp
M&E
S13
```

No dedicated electrical layout, lighting layout, power layout, switch/socket layout, DB schedule, single-line diagram, conduit/cable schedule, fan schedule, fitting schedule, earthing/lightning layout, or M&E specification file was found.

Available sources checked/considered:

```text
Surau Plan Roof Plan Bldg Tender_Constn.pdf
Surau Juasseh sections and elevations tender_constn 1.pdf
Surau Sanitary Plumbing Schematic 1.pdf
Surau Sewerage Schematic 1.pdf
SJ_02R&D-DT-02-S0-00.pdf
SJ_02R&D-LP-01-S0-01.pdf
```

The architectural floor plan contains limited `EL` and `KS` labels, but not a complete electrical legend/specification, fitting schedule, switch/socket schedule, distribution board detail, wiring/conduit route or cable size basis.

## S13 blocker list

| Required S13 scope | Status | Reason |
|---|---|---|
| Lighting points / light fitting schedule | HOLD | No full lighting layout, fitting type/brand/wattage/count/switching schedule found. `EL` labels alone are not enough for 100% electrical takeoff. |
| Fan / mechanical ventilation points | HOLD | No fan schedule, quantity, type, control, mounting or wiring basis found. |
| Switches / socket outlets | HOLD | No complete switch/socket layout, height, type, quantity or circuit basis found. |
| DB / MCB / RCD / ELCB / isolator | HOLD | No distribution board schedule or single-line diagram found. |
| Wiring / conduit / trunking / cable size | HOLD | No cable schedule, conduit route, containment type, cable size or circuit length basis found. |
| Earthing / bonding / lightning protection | HOLD | No earthing/lightning protection source/spec found for S13. |
| Emergency/exit lighting if `EL` means emergency light | HOLD | Meaning and specification of `EL` not sufficiently defined in available source. |
| Testing / commissioning | HOLD | Cannot define full test/commissioning scope without electrical design package. |

## Exact blocker before S14

S13 needs one of the following before it can pass 100% and open S14:

```text
1. Dedicated electrical / lighting / power / M&E drawings and specifications; or
2. Owner/customer-confirmed authorised S13 full allowance schedule with inclusions/exclusions, quantity basis and accepted working-cost rates.
```

Without one of the above, S13 would only be 99.9% or less and must not proceed to S14.

## Current gate

```text
CURRENT ACTIVE SXX: S13
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
S13 STRICT 100% CURRENT BOQ COST BASIS: HOLD
S13 BOQ.XLSM PASTE FILE: NOT CREATED
S13 COST TOTAL: NOT CLOSED
S14 START ALLOWED: NO
S04 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S05 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S06 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S07 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S08 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S09 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S10 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S11 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
S12 CUSTOMER SELLING PRICE: NOT READY - MARKUP/GROSS MARGIN NOT APPLIED
```

## Header update decision

No new header update is required because the latest uploaded `GPTRenovationHeader.txt` already contains:

```text
13D Drawing-spec SXX completion gate
13E Authorised allowance / 100% current BOQ cost basis rule
```

## Next action required

Do not proceed to S14 yet.

Owner must provide or approve one of:

```text
Dedicated S13 electrical / lighting / power / M&E drawings and specifications;
OR
Owner/customer-confirmed authorised S13 full allowance schedule with inclusions/exclusions, quantity basis and accepted working-cost rates.
```
