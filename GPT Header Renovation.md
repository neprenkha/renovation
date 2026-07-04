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

## Floorplan estimate rule

When customer supplied a floor plan but exact sizes are missing or unreadable, AI may use reasonable floorplan-based estimates for early budgeting:

- derive size from visible room proportions;
- use typical Malaysian terrace-house proportions if applicable;
- use practical built-in cabinet depths/heights where not specified;
- apply `+/-` tolerance;
- mark every estimated line as `FLOORPLAN ESTIMATE`;
- keep assumptions visible.

Do not present estimates as final measured quantities. Final quotation remains subject to site measurement, final cabinet drawing, material confirmation and route verification.

## Catalog fallback and manual BOQ rule

If requested work is not fully covered by a completed catalog package, do not force it into the catalog.

Use latest catalog only for matching guide items and customer-facing inclusion wording. For non-catalog items, use `README - BOQ.txt` workflow and master lists to build manual BOQ/spec calculation.

Manual BOQ fallback is required for custom interior/renovation scopes such as kitchen cabinet, TV cabinet, bedroom cabinet, shoe cabinet, plaster ceiling, wiring, plumbing relocation, mirror/fluted/wainscoting, SPC flooring, painting and other itemized works.

Workflow:

1. Read customer request and floor plan/drawing in `ActiveBOQ/`.
2. Split job into S01, S02, S03 scopes by actual construction sequence.
3. Produce SPEC A:C first according to `README - BOQ.txt`.
4. Use exact descriptions from `1.2 Materials.txt` and `1.3 Labour.txt` where available.
5. If a required item is missing, record `INPUT NEEDED` or create a new upgrade file/report first.
6. Keep customer quotation separate from internal cost build-up.

## AdditionalMaterials reference and old-price uplift rule

`AdditionalMaterials/` is a supplemental price-reference area. It may be used when owner explicitly points to it, such as `AdditionalMaterials/SPC & Vynil` for SPC/Vinyl flooring.

Rules:

- Use the cheapest suitable option only when owner asks for cheaper option and material still matches customer request.
- If customer asked for SPC, choose the cheapest SPC item, not vinyl, unless owner accepts vinyl substitution.
- Record selected item, rate, coverage, source folder and limitation in a new ActiveBOQ upgrade file.
- Mark as provisional if not yet an exact `1.2 Materials.txt` master item.
- Do not silently treat AdditionalMaterials as master list.
- If the price reference may be old but is still usable for cost estimate, apply an age/inflation allowance of 5% to 10% where logical.
- For early budgeting, show base price, +5% and +10% option, then use the prudent +10% cost unless owner instructs otherwise.
- Do not apply annual uplift to owner-confirmed current labour rates unless owner says the labour rate is old.

## SPC flooring rule for ActiveBOQ

For this ActiveBOQ customer job, owner confirmed the existing living hall floor is tile.

SPC pricing assumptions for this job:

- No floor levelling by default because existing tile floor is assumed usable.
- No hacking/removal of existing tile; SPC is installed over existing tile.
- Use SPC installation labour at RM2/sqft.
- Skirting and profile/trims can use listed AdditionalMaterials prices.
- Glue is optional only if selected system/profile needs it.
- Foam/underlay is normally expected for ground-floor use, but if price is not found in the provided price reference, list it as missing rather than inventing a rate.
- Final colour/model selection is chosen later and does not block early budgeting.
- If SPC material/skirting/profile/glue prices are old, calculate base, +5% and +10% material uplift; use +10% for safer cost estimate.

These confirmations apply to this ActiveBOQ SPC scope unless owner reuses them in another job.

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
- `AdditionalMaterials/`
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
8. `AdditionalMaterials/` for owner-pointed supplemental material pricing.
9. README quotation rules.
10. Deep Research only where not conflicting.
11. PDF/DOCX rendered reference.
12. Older drafts or stale branches.

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
- Do not invent brands, exact models, or missing rates.
- Do not present floorplan estimates as final measured quantities.
- Do not treat AdditionalMaterials as master list unless formally mapped/approved.
- Do not choose vinyl when customer asked for SPC unless owner approves substitution.
- Do not include floor levelling or existing tile hacking/removal for this ActiveBOQ SPC scope unless later evidence requires it.
- Do not invent foam/underlay price if not found in provided price reference.
- Do not use old AdditionalMaterials prices without marking uplift/age allowance when owner says the reference may be old.
- Do not work in hidden branch when owner expects `main`, unless branch workflow is explicitly agreed.
- Do not request or use permission for `neprenkha/BOQ` when current work is `neprenkha/renovation`.
- Do not treat root catalog as active customer job; active customer job is under `ActiveBOQ/`.
- Do not force custom renovation items into catalog package pricing when manual BOQ is more suitable.
