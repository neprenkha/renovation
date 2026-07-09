# GPT Header Amendment — Aluminium / Glass Spec Schedule Rule

Generated MYT: 2026-07-10 07:00

Repository:

```text
neprenkha/renovation
```

This amendment must be merged into:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt full owner-copy replacement
```

## Why this amendment exists

Owner corrected GPT after S11 because aluminium/glass work must not be left as vague grouped pricing. Even if the owner will calculate or replace actual aluminium/glass price later, the BOQ/takeoff must extract the full specification, size, quantity and brand/system where available.

## Permanent rule

For any SXX containing aluminium, glass, glazing, sliding door, window, louvre, shopfront, aluminium frame, powder coated frame, tempered glass, laminated glass, mirror, shower screen, glass balustrade, glass partition, or related opening work, GPT must produce a separate full specification schedule.

The schedule must list every different aluminium/glass/opening item separately by:

```text
SXX
item mark from drawing, such as D2, W1, W2, W3 or equivalent
item type
exact width and height from drawing/schedule
unit conversion where useful, such as mm and ft
panel/leaf count where visible or specified
frame material and finish
brand/system where stated
glass type and thickness
opening type
quantity / number of units
area per unit and total area where relevant
inclusions such as frame, tracks, rollers, handle/lock/ironmongery, sealant, flashing, setting blocks and fixing accessories
exclusions and no-cost opening notes where relevant
```

Do not merge different sizes/specs into one vague line when they have different dimensions, glass type, brand/system, panel count, opening method or cost basis.

Example required style:

```text
10ftW x 8ftH 3 panel powder coated frame 8mm glass sliding door - 10 nos
```

The actual dimensions and specs must follow the drawing/schedule. Do not invent a panel count or brand if not shown. If brand exists, record it. If brand is absent, write `brand not stated`.

## Actual-price-later rule

If owner says aluminium/glass actual price will be entered/calculated later, GPT must still output the full spec-size-quantity schedule so the owner/supplier can price accurately.

The line may be marked:

```text
ACTUAL ALUMINIUM/GLASS PRICE TO BE REPLACED BY OWNER LATER
```

but it must not omit spec, size, quantity or brand/system.

## SXX gate rule

If a previous SXX already grouped aluminium/glass items too broadly, GPT must revise that SXX with a new cumulative version before continuing later SXX. The revised version must preserve old useful content and add the full spec-size-quantity schedule.

Before moving to the next SXX, any aluminium/glass SXX must record:

```text
full spec schedule complete
size and quantity checked from drawing/schedule
brand/system checked
no-cost openings separated from priced aluminium/glass items
masonry/opening formation excluded if already counted elsewhere
actual-price-later status if owner will replace the rate
undercost/overprice/double-count check
```

If any aluminium/glass spec/size/quantity is unclear and no authorised allowance or pricing schedule basis can close it, mark:

```text
HOLD - ALUMINIUM / GLASS SPEC SCHEDULE INCOMPLETE
```

and do not proceed to the next SXX under a 100% owner instruction.

## S11 application

S11 must be revised to include a dedicated aluminium/glass/spec schedule showing D2, W1, W2 and W3 separately by size, glass thickness, frame/spec, quantity and brand/system.

W4/W5/W6 must be recorded as no-cost high-level lighting/ventilation openings with no window supply.

BS1 must remain excluded to S10 brick screen scope.
