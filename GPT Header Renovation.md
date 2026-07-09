# GPT Header Renovation

## Purpose and audience

Repository: `neprenkha/renovation`

This header is a standalone handover and governance file for ACTIVEBOQ / Mix BOQ renovation catalog, BOQ and quotation work. It must be understandable by the owner, a new AI session, QS, ID, contractor, or future reviewer.

When the owner pastes this header into another AI session or gives it with the latest catalog PDF, that reader must understand the versioning rule, source order, customer-facing catalog intent, quotation method and safety boundaries.

## Canonical editable header location

The repository-level GPT governance/header may be edited only through the canonical editable copy under:

```text
GPTEditable/GPT Header Renovation.md
```

The root file:

```text
GPT Header Renovation.md
```

remains a visible repository header/reference. If both files exist, the editable folder copy and root header must be kept aligned in the same session whenever owner changes a permanent general rule.

`GPTEditable/` is for GPT-editable governance files only. It is not a project/customer work folder.

## Browser reply timestamp rule

Every browser/chat reply for this renovation project must show Malaysia date/time near the top:

`MYT: YYYY-MM-DD HH:mm`

Use Malaysia timezone `Asia/Kuala_Lumpur`.

## Project identity guard

This header belongs only to `neprenkha/renovation`.

Before every reply, prompt, audit or GitHub edit, confirm the work belongs to `neprenkha/renovation`. If the request, permission screen, repository, file names or task point to `neprenkha/BOQ`, LBHub, Enginuity, ONEBOT, ACCOUNT or another project, stop first and warn the owner. Do not silently mix headers, files, rules, branches or project authority.

## ActiveBOQ parent-folder and active workspace rule

`ActiveBOQ/` is a parent folder for many separate customers, sites and BOQ jobs. It is not itself one customer/site workspace.

When the owner names a workspace such as:

```text
ActiveBOQ/Surau Nilai/
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/
```

GPT must treat that exact folder as the hard write boundary.

Do not write generated project files directly under:

```text
ActiveBOQ/
```

Do not write into another customer/site folder.

The root repo remains the reference source for catalog, material, labour, BOQ and quotation rules. ActiveBOQ job folders may use root reference files but must not overwrite root catalog versions or reference files.

Before quotation work, check job label, floor plan, work area, house/storey type, measurements/scale, finish tier, add-ons, site risks and output format.

Earlier wording that treated `ActiveBOQ/` as the current customer-pricing job is superseded: the active job is now the specific child folder named by owner.

## Standard ActiveBOQ job folder layout

For each customer/site folder, use this structure where applicable:

```text
GPT_CONTROL/
Takeoff_Work/
BOQ/
BOQ_work/
Drawing/
OriginalFile/
```

Folder roles:

| Folder | Purpose | GPT write rule |
|---|---|---|
| `GPT_CONTROL/` | Local notes, file maps, job-specific reminders if needed | Can write, but general rules must update this header |
| `Takeoff_Work/` | Measurement notes, takeoff detail, correction logs, assumptions | Can write |
| `BOQ/` | Customer estimate, quotation draft, BOQ, supplier files and final outputs | Can write |
| `BOQ_work/` | Intermediate work files | Can write, but do not auto-delete |
| `Drawing/` | Uploaded PDFs/drawings | Read-only |
| `OriginalFile/` | Owner original/source files | Read-only |

Job-specific README/header files are allowed only as local notes. They must not replace this repository-level header. Any permanent/general rule learned from any job must be copied back into `GPT Header Renovation.md` / `GPTEditable/GPT Header Renovation.md` in the same session.

## Read-only and editable file authority

Default read-only unless owner explicitly says otherwise:

- all `Drawing/` folders;
- all `OriginalFile/` folders;
- old version files such as V1, V2, V3 etc.;
- root reference files such as Materials, Labour, README-BOQ, quotation README, price references, PDF/DOCX catalog renders, old catalog versions and owner source files.

Default editable/work-output folders are only the GPT-created work folders inside the active workspace, such as `Takeoff_Work/`, `BOQ/`, `BOQ_work/`, and `GPT_CONTROL/`.

If owner explicitly says a file or folder is read-only, GPT must not edit, rename, move, overwrite or delete it.

## Version-chain rule for working outputs

For working outputs, V1, V2, V3 and later are immutable references once created unless owner explicitly asks direct edit on that exact file.

When an update is needed:

- do not edit V1 directly;
- create V2;
- V2 must include the useful/current content from V1 plus the new changes;
- if V2 is later insufficient, create V3;
- V3 must include the useful/current content from V1 and V2 plus the new changes;
- continue the same cumulative pattern for later versions.

Do not create a new version that only contains the latest delta and loses earlier working context. Each new version must be usable as the current complete reference for that file family.

## Floorplan estimate and AI responsibility rule

When customer supplied a floor plan but exact sizes are missing, unclear, or not directly extractable, AI must not keep pushing the owner to calculate every item.

AI may use reasonable floorplan-based and terrace/semi-D logic estimates for early budgeting:

- derive size from visible room proportions where possible;
- use the actual house type from drawing or owner correction, for example terrace, semi-detached/rumah berkembar, bungalow or apartment;
- use practical built-in cabinet depths/heights where not specified;
- choose suitable sizes/rates that do not look illogical for the room and scope;
- apply `+/-` tolerance;
- mark every estimated line as `FLOORPLAN ESTIMATE`, `DRAWING-DIMENSION CORRECTION`, `LOGICAL PROVISIONAL RATE`, or similar;
- keep assumptions visible.

If owner gives exact drawing dimensions after a rough estimate, those dimensions override earlier typical-size assumptions. Recalculate the affected scope immediately and create a new ActiveBOQ upgrade file. Do not keep the old terrace-size assumption when the drawing or owner confirms the house is semi-detached/rumah berkembar or has larger available wall runs.

Do not present estimates as final measured quantities. Final quotation remains subject to site measurement, final cabinet drawing, material confirmation and route verification.

## Current ActiveBOQ drawing corrections

For the original ActiveBOQ customer job now organized under:

```text
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/
```

owner corrected these drawing dimensions:

- house type is rumah berkembar / semi-detached, not a small terrace assumption;
- kitchen L-shape: 3062mm + 5485mm full-height / full usable kitchen run;
- corrected kitchen L-shape run is about 28ft;
- living hall / TV / SPC area: 9755mm x 6096mm;
- master bedroom area: 5792mm x 6096mm;
- living hall/SPC area has about 5 door/opening transitions from the drawing.

For this customer, do not keep the old 10ft base cabinet, 10ft countertop, 8ft TV cabinet or 180sqft SPC living hall assumptions. Use the corrected drawing basis for kitchen, TV cabinet, master bedroom cabinet/make-up table, shoe cabinet and SPC calculation.

Current provisional quantity logic:

- kitchen base cabinet and countertop: 28ft L-shape;
- kitchen wall cabinet: 28ft full-run allowance unless final cabinet drawing reduces it;
- kitchen backsplash: 28ft x 2.5ft = about 70sqft;
- TV cabinet: use a larger living-room logical allowance, currently 12ft;
- master bedroom cabinet: use 10ft wardrobe and 5ft make-up table provisional allowance;
- shoe cabinet: use 5ft provisional allowance;
- SPC living hall: calculate from 9755mm x 6096mm, about 640sqft;
- SPC skirting: use actual rectangular perimeter, deduct known door openings if they break the skirting line, add 10% wastage, then round up to stock length;
- SPC profile: 5 doors x 3ft, add 10% wastage, then round up to full profile pieces.

## Catalog fallback and manual BOQ rule

If requested work is not fully covered by a completed catalog package, do not force it into the catalog.

Use latest catalog only for matching guide items and customer-facing inclusion wording. For non-catalog items, use `README - BOQ.txt` workflow and master lists to build manual BOQ/spec calculation.

Manual BOQ fallback is required for custom interior/renovation scopes such as kitchen cabinet, TV cabinet, bedroom cabinet, shoe cabinet, plaster ceiling, wiring, plumbing relocation, mirror/fluted/wainscoting, flooring, painting and other itemized works.

Workflow:

1. Read customer request and floor plan/drawing in the active job folder, not directly in `ActiveBOQ/` root.
2. Split job into S01, S02, S03 scopes by actual construction sequence.
3. Produce SPEC A:C first according to `README - BOQ.txt`.
4. Use exact descriptions from `1.2 Materials.txt` and `1.3 Labour.txt` where available.
5. If a required item is missing from master lists, AI may create an ActiveBOQ provisional rate assumption file when the owner allows logical estimates.
6. Keep customer quotation separate from internal cost build-up.

## Sequential SXX costing, wastage, buffer and MH productivity rule

For any BOQ or quotation job that uses S01-SXX, GPT must cost one SXX at a time in construction sequence. Do not open the next SXX costing file until the current SXX is either `COMPLETE FOR NEXT SXX` or `RESERVED WITH REASON`.

Each SXX cost file must complete these gates before moving to the next SXX:

1. read the active workspace files and the relevant drawing/source evidence;
2. confirm SPEC A:C is takeoff-ready for that SXX;
3. extract and show raw measured quantity, deduction, net quantity and UOM;
4. map material lines to exact `1.2 Materials.txt` Description and UOM where available;
5. map labour, plant, rental and service lines to exact `1.3 Labour.txt` Description and UOM where available;
6. separate Block 1 material, Block 2 labour/plant and Block 3 subcontract/specialist/service;
7. apply wastage explicitly by item or trade, not hidden inside a lump sum;
8. apply buffer/contingency separately from wastage and state whether it is included or only shown as an option;
9. round purchase quantities to practical supplier stock units after wastage, for example full bag, full sheet, full length, full box, full roll, full trip, full m3 or full piece;
10. record manpower-hour/productivity basis where labour is not a fixed master-list package rate, including crew size, expected output per day/hour or total man-hours;
11. mark missing master-list items, missing rates, missing specifications and supplier-needed items in the SXX file, not by inventing final rates silently;
12. state whether the SXX total is `WORKING COST`, `PROVISIONAL COST`, `SELLING RATE USED`, or `CUSTOMER SELLING PRICE`.

For large construction projects such as Surau Nilai, the default order is:

`Deep Read Register -> Scope Sequence -> S01 SPEC + Cost -> S01 Check -> S02 SPEC + Cost -> S02 Check -> continue until final Summary`.

A total project price may be reported only from completed SXX totals plus clearly labelled reserved/provisional allowances. Do not claim a final overall price while major SXX scopes remain unread, unmeasured or unpriced.

## MISC product-reference folder rule

New material/product references for flooring should be kept under:

`MISC/Nii Flooring SPC, Vinyl/`

This MISC folder is the preferred reference location for NII flooring products, SPC, Vinyl, Carpet, foam/underlay, glue, profile, skirting and future separated product folders.

Older `AdditionalMaterials/` files may remain as legacy references, but future flooring takeoff should check `MISC/Nii Flooring SPC, Vinyl/` first when the owner says updated materials are there.

When the owner separates product folders inside MISC, use the most specific product folder first, for example:

- SPC product folder;
- Vinyl product folder;
- Carpet product folder;
- Foam / underlay folder;
- Glue folder;
- Profile / trims folder;
- Skirting folder.

Do not treat MISC references as public selling prices by default. They are product/cost references unless the owner labels them as selling/package rates.

If a MISC price reference may be old but is still usable for rough costing, apply a logical 5% to 10% uplift and show the base, +5%, and +10% options.

## Floor covering stock-size calculation rule

This rule applies to Carpet, Vinyl, SPC, foam/underlay, glue, skirting, profile and other flooring accessories.

Calculate by supplier stock size, not by loose tiny quantities.

Standard method when customer provides only total floor area:

1. If no room dimension is available, use square-root method as a quick perimeter estimate: `side = sqrt(area sqft)`.
2. If actual rectangular dimensions are available, use actual area and actual perimeter instead of square-root estimate.
3. Floor material: add 10% wastage to floor area, divide by box/roll coverage, and round up to the next full box/roll/stock unit.
4. Skirting: use actual perimeter where available. If door/opening count is known and the openings break the skirting line, deduct door/opening width before wastage. Then add 10% wastage and round up to full stock length.
5. Profile/trims at doorways and edges: use actual door count/opening count if known. If not known, use a logical default for the house size. For a 1044 sqft house, use up to 8 door openings as a safe standard estimate unless the floor plan indicates otherwise.
6. Door profile default: use 3ft per door/opening, add 10% wastage, divide by profile stock length, and round up to full pieces.
7. Glue: use tub/stock-size allowance. Do not price a tiny loose amount if supplier sells by full tub.
8. Foam/underlay: use full roll/box/stock-size allowance if it is separate. Do not price loose sqft unless supplier sells by sqft.
9. Accessories must be rounded by stock unit: full box, full piece, full tub or full roll.
10. Record whether the calculation is Carpet, Vinyl, SPC, ground floor, upper floor, foam-backed, separate foam, glue-down, click system, or provisional.

Floor covering notes:

- SPC: Ground floor normally uses foam-backed / foam-included SPC when product reference has that option. If SPC product already includes foam/underlay, record `FOAM INCLUDED IN PRODUCT SPEC` and do not add separate foam cost by default. Upper floor normally does not add separate foam unless product spec, acoustic requirement, or site requirement says so.
- Vinyl: Usually follows its system requirement. Glue-down vinyl should include glue unless product/system says otherwise. Foam is not added unless product/system specifically requires underlay.
- Carpet: Usually needs profile/trims at edges and door transitions. Carpet usually does not use skirting by default unless the product/system or owner request says so. Carpet accessories must still be rounded to stock size.
- If exact floor plan is available, replace the square-root method with actual room perimeter, actual doorway count, and actual edge/profile lengths.
- If customer asks for SPC, do not substitute Vinyl or Carpet just because cheaper unless owner approves substitution.

Example reference calculation:

`MISC/Nii Flooring SPC, Vinyl/1044sqft_Flooring_Calculation_Template_V1.md`

Legacy example reference:

`AdditionalMaterials/SPC & Vynil/1044sqft_SPC_Vinyl_Calculation_V1.md`

## SPC flooring rule for ActiveBOQ

For this ActiveBOQ customer job, owner confirmed the existing living hall floor is tile.

SPC pricing assumptions for this job:

- No floor levelling by default because existing tile floor is assumed usable.
- No removal of existing tile; SPC is installed over existing tile.
- Use SPC installation labour at RM2/sqft unless owner gives another rate for the job.
- Delivery is treated as included in the SPC installation labour for this ActiveBOQ scope unless later owner says otherwise.
- Skirting and profile/trims can use listed product-reference prices.
- Glue is optional only if selected system/profile needs it.
- Final colour/model selection is chosen later and does not block early budgeting.
- `NII FLOOR PRODUCT PRICELIST 2023 - updated 311222.pdf` must be checked for SPC product numbers 7-12 because owner identified those as foam-backed/foam-included references.
- If the selected SPC product already states foam/underlay is included or attached, do not add a separate foam line by default. Record it as `FOAM INCLUDED IN PRODUCT SPEC` and confirm exact model later.
- If selected product does not include foam, add separate foam/underlay only when a price source exists; do not invent a foam rate.
- If SPC material/skirting/profile/glue prices are old, calculate base, +5% and +10% material uplift; use +10% for safer cost estimate.

These confirmations apply to this ActiveBOQ SPC scope unless owner reuses them in another job.

## Cost versus selling price rule

Every ActiveBOQ estimate must clearly state whether the amount is:

- internal cost / working cost;
- cost with contingency only;
- customer selling price with markup;
- customer selling price with target gross margin.

Do not call a number customer-ready if markup or margin has not been explicitly calculated. Rounding a cost number to the nearest customer figure is not a markup.

When preparing a customer quotation from internal cost, create a separate upgrade file showing at least:

- base working cost;
- markup on cost options, normally 10%, 15%, and 20%;
- optional/add-on impact;
- recommended customer figure;
- whether SST, management fee, delivery, access cost, or authority cost is included or excluded.

If a rate is already a selling/package rate, mark it as `SELLING RATE USED`. If it is only cost/provisional, mark it as `WORKING COST` or `PROVISIONAL COST`.

## Immutable source and cumulative upgrade-file rule

Do not edit original customer files, old catalog versions, PDFs, DOCX, Materials, Labour, README or Deep Research unless owner explicitly asks to revise that exact file.

Customer originals such as `Customer Request.txt`, floor plans, drawings, photos and uploaded PDFs are source evidence and must remain unchanged.

Every correction, audit, BOQ, SPEC, measurement extraction or quotation draft must be saved as a new upgrade file inside the active customer/site workspace, not directly under `ActiveBOQ/` root.

Use a clear version suffix, for example:

- `Customer_Request_Audit_V1.md`
- `Customer_Request_SPEC_V1.tsv`
- `ActiveBOQ_Takeoff_V1.tsv`
- `Customer_Quotation_Draft_V1.md`
- later corrections as V2, V3 and so on.

If V1 exists and needs updating, create V2 with V1 useful/current content included. If V2 needs updating, create V3 with V1 and V2 useful/current content included. Do not create a V2/V3 that contains only the new small correction and loses the earlier work trail.

If V5 catalog needs correction, create V6. Do not edit V5 directly unless owner explicitly instructs direct V5 correction.

## Current source files

Current V4 source names:

- `SingleStoreyExtentionNRenovationV4.md`
- `DoubleStoreyExtentionNRenovationV4.md`

Current V5 source names:

- `SingleStoreyExtentionNRenovationV5.md`
- `DoubleStoreyExtentionNRenovationV5.md`
