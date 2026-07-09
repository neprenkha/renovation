# S13 Electrical / Aircond Size-Based Estimate Assumption V1

Generated MYT: 2026-07-10 08:01

## Owner instruction

Owner accepted a size-based estimate path for S13 so that the workflow can proceed to S14, while keeping clear that this is not an exact electrical design takeoff.

## Status

```text
S13 WORKING-COST ESTIMATE COMPLETE - OWNER ACCEPTED SIZE-BASED PROVISIONAL PATH
S13 DRAWING-SPEC EXACT ELECTRICAL DESIGN: HOLD UNTIL DEDICATED ELECTRICAL DRAWING / OWNER CONFIRMED ELECTRICAL SCHEDULE
S14 START ALLOWED: YES, ON WORKING-COST ESTIMATE PATH ONLY
```

## Area basis

| Basis | Quantity | Source/use |
|---|---:|---|
| Covered internal / ceiling finish area | 232.63 m2 / 2,504 ft2 | Used as full internal electrical coverage estimate area. |
| Main prayer / carpet substrate area | 98.50 m2 / 1,060 ft2 | Used for main hall aircond/fan comfort estimate. |
| Roof surface / high roof context | 390 m2 roof surface basis from S09 | Used as cooling-load risk indicator because high roof / larger envelope increases aircond demand. |

## Label basis from floor plan / Drawing.zip check

The floor plan has limited labels only:

```text
EL labels visible/extracted: 4
KS labels visible/extracted: 4
DP labels visible/extracted: 6
```

These labels remain insufficient for exact wiring design, but they are used as a sanity check only.

## Electrical point estimate for full covered building

| Item | Basis | Estimated qty | Note |
|---|---|---:|---|
| General lighting points | 1 point per 7.5-8.5 m2 over 232.63 m2 | 30 points | Includes prayer hall, circulation, toilets and ancillary spaces. |
| Emergency / exit light allowance | EL visible labels and small surau allowance | 4 points | If EL means emergency light, use 4 points. If not, revise after electrical legend. |
| Ceiling fan / air movement points | KS visible 4 plus size/high-roof comfort allowance | 8 points | 4 visible + 4 size-based additional allowance for full area comfort. |
| General power socket outlets | Full building working allowance | 22 points | Includes PA/cleaning/office/general outlet allowance; exact layout still pending. |
| Switch / control points | Lighting/fan grouping allowance | 14 points | Switching zones for prayer hall, toilets, circulation and exterior/control areas. |
| Aircond power isolator points | Full building allowance | 8 points | Allows main hall and ancillary rooms. Actual AC quantity/capacity to be confirmed. |
| Exhaust fan / ventilation points | Toilets/wet/internal areas | 4 points | Exact mechanical ventilation layout pending. |
| Distribution board / protection | Small public building 3-phase assumption | 1 lot | Includes DB, MCB/RCD/ELCB allowance, not authority fees. |
| Earthing / bonding | Small public building allowance | 1 lot | Exact design pending. |

## Aircond capacity estimate

This estimate is based on covered size, high roof context and prayer occupancy risk. It is not an HVAC design.

### Option A - practical main prayer / main occupied zone cooling

```text
Main prayer/carpet area: 98.50 m2 / 1,060 ft2
Suggested allowance: 4 units x 3.0HP class
Approx cooling capacity: 4 x 28,000 BTU/h = 112,000 BTU/h
Approx installed cooling: about 12HP class
```

This is the minimum sensible estimate if only the main worship zone is actively cooled.

### Option B - full internal building comfort allowance

```text
Main hall: 4 units x 3.0HP class = about 12HP / 112,000 BTU/h
Ancillary rooms / office / muslimah / support areas: 4 units x 1.5HP to 2.0HP class = about 6HP to 8HP / 54,000 to 72,000 BTU/h
Total full-building allowance: 8 AC points, about 18HP to 20HP class, about 166,000 to 184,000 BTU/h
```

S13 uses 8 aircond power isolator points as the working-cost wiring allowance.

## Electrical load estimate

Approximate full-building connected/running demand for preliminary DB sizing only:

```text
Aircond running input allowance: about 15kW to 18kW depending AC model/efficiency
Lighting: about 1.5kW to 2.5kW
Fans: about 0.6kW to 1.0kW
General socket / PA / cleaning / spare allowance: about 4kW to 6kW
Estimated working demand allowance: about 25kW to 30kW
Recommended estimate basis: 3-phase DB / submain allowance, final capacity by electrician/engineer
```

## Boundary / duplicate prevention

```text
S12 ceiling/finishes are not duplicated.
S06 plumbing rough-in is not duplicated.
S11 aluminium/glass/opening work is not duplicated.
AC unit supply/brand/model is not priced unless owner later wants it included.
Authority meter/deposit/TNB application fees are not included unless owner confirms.
Exact cable size/circuit design remains pending final electrical design.
```

## Gate decision

```text
S13 can proceed as working-cost estimate only.
This is not a 100% drawing-spec measured electrical design.
S14 may start because owner accepted size-based provisional path.
```
