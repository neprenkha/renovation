# S15 Fencing and Gate — Strict Recheck Audit V1

Generated MYT: 2026-07-10 08:41

## Purpose

Owner requested repeated careful verification that S15 can be taken off at 100% current BOQ cost basis according to customer drawing/specification before moving to S16.

Strict gate applied:

```text
100% target = current BOQ cost basis complete for S15 using customer drawing/spec and customer/drawing accepted full allowance basis.
99.9% is not a pass.
Customer selling price / margin is separate and not part of this gate unless owner asks for selling price.
```

## Header compliance

Latest uploaded owner header checked:

```text
GPTRenovationHeader.txt
Generated MYT: 2026-07-10 07:00
```

Relevant rules applied:

```text
13 Sequential SXX costing gate
13B Drawing/spec and auditable takeoff rule
13C BOQ.xlsm paste-ready output rule
13D Drawing-spec SXX completion gate
13E Authorised allowance / 100% current BOQ cost basis rule
```

## Source drawing checked

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

## Drawing/spec facts recorded

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

## S15 included scope

```text
front anti-climb fence panels
main large metal vehicle gate
gate/fence posts, facing brick posts, meter/bin enclosure walling
RC gate/fence footing, plinth, coping and base beam allowance
small metal doors and meter/inspection panel
200 x 200mm ceramic wall and floor tiles for bin/meter enclosure areas
drainage outlet at gate/bin area
MS grating to engineer detail
meter interface enclosure sundries
gate/fence installation labour, masonry/tile/concrete labour and door/panel labour
anti-rust/paint/touch-up, gate hardware, final adjustment/test/cleaning
```

## Duplicate prevention

```text
S01 temporary hoarding/signboard excluded.
S04 crossing bridge/permanent entrance road/bridge works excluded.
S14 road/drain/culvert/long external drainage excluded.
S13 electrical DB/internal wiring excluded; only meter enclosure/interface sundries included.
S06 plumbing/sewer rough-in excluded.
S10 main building walling excluded.
Utility meter supply/deposit/authority application fees excluded.
Security/CCTV/data system excluded to S13 unless separately expanded later.
```

## Quantity basis

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

## Strict 100 checklist

| Check | Result | Note |
|---|---|---|
| Source drawing rendered/visually checked | PASS | Fencing and Gate 1.pdf rendered and inspected. |
| Frontage/gate dimensions checked | PASS | 4431 + 10883 + 4172 = 19486mm. |
| Main gate included | PASS | 10883mm wide gate included by m2 full allowance. |
| Anti-climb fence included | PASS | Left/right fencing panels included. |
| Gate/fence structural base included | PASS | Footing/plinth/coping/base allowance included. |
| Brick posts / enclosure walls included | PASS | Facing brick post and side enclosure basis included. |
| Metal doors / inspection panel included | PASS | 900x700 metal doors and right inspection panel included. |
| Tile finish included | PASS | 200x200 ceramic wall/floor tiles included. |
| Drainage outlet / MS grating included | PASS | Included without duplicating S14 long drainage. |
| Meter interface included | PASS | Meter enclosure/interface sundries included; authority meter fees excluded. |
| S01 duplicate prevention | PASS | Temporary hoarding/signboard excluded. |
| S04 duplicate prevention | PASS | Crossing bridge/permanent entrance works excluded. |
| S14 duplicate prevention | PASS | Road/drain/culvert long drainage excluded. |
| S13 duplicate prevention | PASS | Internal DB/wiring/security system excluded. |
| Block 1 complete | PASS | Materials and supply allowances included. |
| Block 2 complete | PASS | Installation/concrete/masonry/tile/direct labour included. |
| Block 3 complete | PASS | Paint/protection, hardware and final test/cleaning included. |
| Markup check | PASS | No customer markup applied. |
| 100% / 99.9% gate | PASS | Current S15 BOQ cost basis is closed from drawing-derived full allowance and no active hanging item remains. |

## Decision

```text
S15 STRICT 100% CURRENT BOQ COST BASIS: PASS
S15 BOQ.XLSM PASTE FILE: READY - USE V1
S16 START ALLOWED: YES
```

## Header update decision

No new header update is required for S15 because the latest uploaded `GPTRenovationHeader.txt` already contains the 100% SXX gate, drawing/spec gate, authorised allowance rule and paste-ready output rule needed for this step.
