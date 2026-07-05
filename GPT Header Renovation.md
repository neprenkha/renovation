# GPT Header Renovation

## Purpose and audience

Repository: `neprenkha/renovation`

This header is a standalone handover and governance file for ACTIVEBOQ / Mix BOQ renovation catalog, BOQ and quotation work. It must be understandable by the owner, a new AI session, QS, ID, contractor, or future reviewer.

When the owner pastes this header into another AI session or gives it with the latest catalog PDF, that reader must understand the versioning rule, source order, customer-facing catalog intent, quotation method and safety boundaries.

## Browser reply timestamp rule

Every browser/chat reply for this renovation project must show Malaysia date/time near the top:

`MYT: YYYY-MM-DD HH:mm`

Use Malaysia timezone `Asia/Kuala_Lumpur`.

## Project identity guard

This header belongs only to `neprenkha/renovation`.

Before every reply, prompt, audit or GitHub edit, confirm the work belongs to `neprenkha/renovation`. If the request, permission screen, repository, file names or task point to `neprenkha/BOQ`, LBHub, Enginuity, ONEBOT, ACCOUNT or another project, stop first and warn the owner. Do not silently mix headers, files, rules, branches or project authority.

## ActiveBOQ active work folder

The current active customer-pricing work is under `ActiveBOQ/`.

`ActiveBOQ/` is for the current extension/renovation customer job where customer supplied floor plan and owner needs price calculation plus customer-facing quotation.

The root repo remains the reference source for catalog, material, labour, BOQ and quotation rules. ActiveBOQ must use root reference files but must not overwrite root catalog versions or reference files.

Before quotation work, check job label, floor plan, work area, house/storey type, measurements/scale, finish tier, add-ons, site risks and output format.

## Floorplan estimate and AI responsibility rule

When customer supplied a floor plan but exact sizes are missing, unclear, or not directly extractable, AI must not keep pushing the owner to calculate every item.

AI may use reasonable floorplan-based and terrace-house logic estimates for early budgeting:

- derive size from visible room proportions where possible;
- use typical Malaysian terrace-house proportions if applicable;
- use practical built-in cabinet depths/heights where not specified;
- choose suitable sizes/rates that do not look illogical for the room and scope;
- apply `+/-` tolerance;
- mark every estimated line as `FLOORPLAN ESTIMATE`, `LOGICAL PROVISIONAL RATE`, or similar;
- keep assumptions visible.

Do not present estimates as final measured quantities. Final quotation remains subject to site measurement, final cabinet drawing, material confirmation and route verification.

## Catalog fallback and manual BOQ rule

If requested work is not fully covered by a completed catalog package, do not force it into the catalog.

Use latest catalog only for matching guide items and customer-facing inclusion wording. For non-catalog items, use `README - BOQ.txt` workflow and master lists to build manual BOQ/spec calculation.

Manual BOQ fallback is required for custom interior/renovation scopes such as kitchen cabinet, TV cabinet, bedroom cabinet, shoe cabinet, plaster ceiling, wiring, plumbing relocation, mirror/fluted/wainscoting, flooring, painting and other itemized works.

Workflow:

1. Read customer request and floor plan/drawing in `ActiveBOQ/`.
2. Split job into S01, S02, S03 scopes by actual construction sequence.
3. Produce SPEC A:C first according to `README - BOQ.txt`.
4. Use exact descriptions from `1.2 Materials.txt` and `1.3 Labour.txt` where available.
5. If a required item is missing from master lists, AI may create an ActiveBOQ provisional rate assumption file when the owner allows logical estimates.
6. Keep customer quotation separate from internal cost build-up.

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
2. Estimate four-side perimeter: `perimeter = side x 4`.
3. Floor material: add 10% wastage to floor area, divide by box/roll coverage, and round up to the next full box/roll/stock unit.
4. Skirting: apply 10% wastage to perimeter and round up to full stock length. Use the exact stock length in the current price list, for example 8ft or 9ft.
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
- Use SPC installation labour at RM2/sqft.
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

## Immutable source and upgrade-file rule

Do not edit original customer files, old catalog versions, PDFs, DOCX, Materials, Labour, README or Deep Research unless owner explicitly asks to revise that exact file.

Customer originals such as `Customer Request.txt`, floor plans, drawings, photos and uploaded PDFs are source evidence and must remain unchanged.

Every correction, audit, BOQ, SPEC, measurement extraction or quotation draft must be saved as a new upgrade file in `ActiveBOQ/` with a clear version suffix, for example:

- `Customer_Request_Audit_V1.md`
- `Customer_Request_SPEC_V1.tsv`
- `ActiveBOQ_Takeoff_V1.tsv`
- `Customer_Quotation_Draft_V1.md`
- later corrections as V2, V3 and so on.

If V5 catalog needs correction, create V6. Do not edit V5 directly unless owner explicitly instructs direct V5 correction.

## Current source files

Current V4 source names:

- `SingleStoreyExtentionNRenovationV4.md`
- `DoubleStoreyExtentionNRenovationV4.md`

Current V5 source names:

- `SingleStoreyExtentionNRenovationV5.md`
- `DoubleStoreyExtentionNRenovationV5.md`
- `V5_CHANGE_REPORT.md`
- `V5_CUSTOMER_ANSWER.md`

Supporting references:

- `1.2 Materials.txt`
- `1.3 Labour.txt`
- `README - BOQ.txt`
- `README - QUOTATION.txt`
- `deep-research-report full.md`
- `MISC/Nii Flooring SPC, Vinyl/`
- `AdditionalMaterials/` as older supplemental reference
- current PDF/DOCX catalog renders

Actual current repository overrides memory.

## Source order

1. Latest explicit owner instruction.
2. This header for workflow rules.
3. ActiveBOQ current job files.
4. Latest versioned catalog where applicable.
5. `README - BOQ.txt` for manual takeoff.
6. `1.2 Materials.txt`.
7. `1.3 Labour.txt`.
8. `MISC/Nii Flooring SPC, Vinyl/` for flooring product/cost references.
9. `AdditionalMaterials/` for older owner-pointed supplemental pricing.
10. ActiveBOQ provisional rate assumption files approved by owner logic.
11. README quotation rules.
12. Deep Research only where not conflicting.
13. PDF/DOCX rendered reference.
14. Older drafts or stale branches.

## Versioning rule

Do not overwrite, delete, rename or move old catalog versions. Old versions are references.

Every meaningful catalog update must create a new versioned file using the same front name and next version number. Future versions continue as V6, V7 and later.

## Catalog and PDF delivery rule

A public catalog version is not customer-ready until matching downloadable files exist or owner accepts Markdown-only use. Each completed public version should have Markdown source, PDF render, change report and customer answer sheet.

## Public catalog rule

Public catalog files must be customer-facing. Do not place internal raw costing, profit, supplier names, GPT/Cursor/Codex notes, source-file notes or audit notes inside public catalog files.

Do not mention brand names unless official quotation intentionally lists a brand/model. Describe items by specification, size allowance, finish tier, included quantity, route/site limitation, exclusions and quote-only items.

## Price rule

Do not change catalog prices, size bands, thresholds or add-on guide prices unless owner explicitly asks. Material and labour files are internal support; they are not public selling prices.

## Header update rule

When owner creates a permanent workflow rule, corrects a recurring mistake, changes source authority, or explicitly asks for header update, update this header in the same work session. A chat apology or acknowledgement alone is not enough.

## Work continuation rule

When owner asks to update GitHub or create catalog/ActiveBOQ/BOQ/audit/quotation work, do not stop at explanation if the safe next action is known. Proceed with the smallest complete safe task; if blocked, state exact block and exact owner action required.

## ActiveBOQ quotation test rule

For customer quotation work under `ActiveBOQ/`, use: customer location/job label, house type/storey type, floor plan evidence, work area and measured/assumed size, finish tier, add-ons, site risks, catalog/manual BOQ reference, inclusions, exclusions, assumptions and remaining questions. Do not promise brand/model unless written in quotation.

## Known mistakes to avoid

- Do not make a new version by changing only the title.
- Do not copy vague V4 wording into a new version without clearer scope.
- Do not edit V4, V5, PDF, DOCX, Materials, Labour, README, Deep Research or customer originals when creating working files.
- Do not invent brands or exact models.
- Do not keep asking owner to calculate when logical floorplan estimate can be made and clearly marked provisional.
- Do not present floorplan estimates as final measured quantities.
- Do not treat MISC or AdditionalMaterials as master list unless formally mapped/approved.
- Do not choose Vinyl or Carpet when customer asked for SPC unless owner approves substitution.
- Do not price Carpet, SPC, Vinyl, foam, glue, profile or skirting by loose 1ft/small loose quantity when supplier stock unit is box, piece, roll or tub.
- Do not add carpet skirting by default unless product/system or owner says so.
- Do not include floor levelling or existing tile removal for this ActiveBOQ SPC scope unless later evidence requires it.
- Do not create separate foam cost when selected SPC product already includes foam.
- Do not invent foam/underlay price if selected product has no foam and no price source is found.
- Do not use old MISC or AdditionalMaterials prices without marking uplift/age allowance when owner says the reference may be old.
- Do not present a cost estimate as customer selling price without explicit markup/margin calculation.
- Do not work in hidden branch when owner expects `main`, unless branch workflow is explicitly agreed.
- Do not request or use permission for `neprenkha/BOQ` when current work is `neprenkha/renovation`.
- Do not treat root catalog as active customer job; active customer job is under `ActiveBOQ/`.
- Do not force custom renovation items into catalog package pricing when manual BOQ is more suitable.
