# S13 Electrical / Lighting / Power / M&E Interface — Strict 100 Recheck HOLD V1

Generated MYT: 2026-07-10 07:44

## Purpose

Owner requested repeated careful verification that S13 can be taken off at 100% current BOQ cost basis according to customer drawing/specification before moving to S14.

Strict gate applied:

```text
100% target = current BOQ cost basis complete for S13.
99.9% is not a pass.
Customer selling price / margin is separate and not part of this gate unless owner asks for selling price.
```

## Header compliance

Latest owner uploaded header checked:

```text
GPTRenovationHeader.txt
Generated MYT: 2026-07-10 07:00
```

Relevant header rules applied:

```text
13 Sequential SXX costing gate
13B Drawing/spec and auditable takeoff rule
13C BOQ.xlsm paste-ready output rule
13D Drawing-spec SXX completion gate
13E Authorised allowance / 100% current BOQ cost basis rule
```

## Repository/source search performed

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

No dedicated electrical layout, lighting layout, power layout, switch/socket layout, DB schedule, single-line diagram, conduit/cable schedule, fan schedule, fitting schedule, earthing/lightning layout, or M&E specification file was found in the GitHub search result.

## Drawing/source files checked for S13

Existing drawing/source set around S13 includes:

```text
Surau Plan Roof Plan Bldg Tender_Constn.pdf
Surau Juasseh sections and elevations tender_constn 1.pdf
Surau Sanitary Plumbing Schematic 1.pdf
Surau Sewerage Schematic 1.pdf
SJ_02R&D-DT-02-S0-00.pdf
SJ_02R&D-LP-01-S0-01.pdf
```

The architectural floor plan contains limited `EL` and `KS` labels, but the available architectural drawing does not provide a complete electrical legend/specification, fitting schedule, switch/socket schedule, distribution board detail, wiring/conduit route or cable size basis.

## S13 items that cannot be closed to 100%

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

## Why authorised allowance cannot close S13 yet

For S08-S12, authorised full allowance could close the current BOQ cost basis because the drawing/spec/README/owner basis provided enough scope authority and duplicate boundaries.

For S13, the available source does not yet provide enough authorised scope basis for electrical quantities. A random lump sum would violate the 100% / 99.9% rule.

S13 cannot be marked:

```text
COMPLETE FOR NEXT SXX - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS
```

unless owner provides or confirms an authorised electrical/M&E allowance basis, or a dedicated electrical drawing/specification is supplied and checked.

## Duplicate boundary check

```text
S12 finishes/ceiling/sanitary final fixtures are not to be duplicated in S13.
S06 plumbing rough-in is not to be duplicated in S13.
S11 aluminium/glass/opening work is not to be duplicated in S13.
S13 should cover only electrical/lighting/power/mechanical interface items after proper source is available.
```

## Decision

```text
S13 STRICT 100% CURRENT BOQ COST BASIS: HOLD
S13 BOQ.XLSM PASTE FILE: NOT CREATED
S13 COST TOTAL: NOT CLOSED
S14 START ALLOWED: NO
```

## Exact blocker

S13 needs one of the following before it can pass 100% and open S14:

```text
1. Dedicated electrical / lighting / power / M&E drawings and specifications; or
2. Owner/customer-confirmed authorised S13 full allowance schedule with inclusions/exclusions, quantity basis and accepted working-cost rates.
```

Without one of the above, S13 would only be 99.9% or less and must not proceed to S14.

## Header update decision

No new header update is required because the current uploaded header already contains the rule that a SXX must HOLD when source/drawing/spec or authorised allowance is insufficient for 100% current BOQ cost basis.
