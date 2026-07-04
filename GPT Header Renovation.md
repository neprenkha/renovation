# GPT Header Renovation

## Purpose and audience

Repository: `neprenkha/renovation`

This header is a standalone handover and governance file for ACTIVEBOQ / Mix BOQ renovation catalog, BOQ and quotation work.

It must be understandable by:

- the owner;
- a new AI session;
- a human quantity surveyor;
- an interior designer;
- a contractor;
- a future reviewer preparing quotation or checking scope.

This header is not only for the AI that created it. When the owner pastes this header into another AI session or gives it with the latest catalog PDF, that reader must understand the versioning rule, source order, customer-facing catalog intent, quotation test method and safety boundaries.

## Browser reply timestamp rule

Every browser/chat reply for this renovation project must show Malaysia date/time near the top in this format:

`MYT: YYYY-MM-DD HH:mm`

Use Malaysia timezone `Asia/Kuala_Lumpur`. Do not rely on UTC or server local time when stating the time.

## Project identity guard

This header belongs only to `neprenkha/renovation`.

Before every reply, prompt, audit or GitHub edit, confirm the work belongs to `neprenkha/renovation`. If the request, permission screen, repository, file names or task point to `neprenkha/BOQ`, LBHub, Enginuity, ONEBOT, ACCOUNT or another project, stop first and warn the owner. Do not silently mix headers, files, rules, branches or project authority.

General governance style may be adapted from other projects only for safety, preservation, evidence, versioning and anti-drift. Do not copy another project's scope, paths, modules, engines, workbooks, runtime rules or business objectives.

## ActiveBOQ active work folder

The current active customer-pricing work is under:

`ActiveBOQ/`

The `ActiveBOQ/` folder is for the current extension and renovation job where the customer has supplied a floor plan and the owner needs to calculate price and prepare a customer-facing quotation.

The wider repository root `neprenkha/renovation` remains the reference source for catalog, material, labour, BOQ and quotation rules. ActiveBOQ must use the root reference files, but it must not overwrite root catalog versions or reference files.

Before doing quotation work in ActiveBOQ, check whether the folder contains enough evidence for:

- customer/project identity or job label;
- floor plan or drawing;
- work area and scope;
- single-storey or double-storey status;
- measurements or scale basis;
- selected package tier or intended finish level;
- add-ons such as bathroom, wet kitchen, laundry, electrical, plumbing, aluminium/glass, cabinet or structure;
- site risk notes;
- required output format for customer quotation.

If any required detail is missing, mark it as missing and ask only for the exact missing item. Do not invent final quotation price from an unclear drawing.

## Floorplan estimate rule

When a customer has supplied a floor plan but exact sizes are not written or are not readable, AI may use reasonable floorplan-based estimates for early budgeting.

Allowed estimate methods:

- derive approximate size from visible room proportions in the floor plan;
- use typical Malaysian terrace-house proportions when the drawing is clearly a normal terrace-style layout;
- use practical built-in cabinet depths and heights where not specified;
- apply `+/-` tolerance and mark the line as `FLOORPLAN ESTIMATE`;
- choose a reasonable size that does not look illogical for the room type;
- keep assumptions visible in the audit/spec/quotation file.

Do not present floorplan estimates as final measured quantities. Final quotation must still say subject to site measurement, final cabinet drawing, material confirmation and route verification.

If the floor plan cannot be read at all, state that limitation and use only request-based provisional scope until the readable drawing is available.

## Catalog fallback and manual BOQ rule

If the requested work is not fully covered by a completed catalog package, do not force it into the catalog.

Use the latest catalog only for matching guide items and customer-facing inclusion wording. For items not covered by the catalog, use `README - BOQ.txt` workflow and the master lists to build a manual BOQ/spec calculation.

Manual BOQ fallback is required for custom interior or renovation scopes such as kitchen cabinet, TV cabinet, bedroom cabinet, shoe cabinet, plaster ceiling, wiring points, plumbing relocation, mirror/fluted/wainscoting, SPC flooring, painting or other itemized work that is not priced as a ready catalog package.

The workflow is:

1. Read the customer request and floor plan/drawing in `ActiveBOQ/`.
2. Split the job into logical S01, S02, S03 scopes following actual construction sequence.
3. Produce SPEC A:C first according to `README - BOQ.txt`.
4. Use exact master-list descriptions from `1.2 Materials.txt` and `1.3 Labour.txt` for takeoff rows where available.
5. If a required material/labour item is missing from the master list, record `INPUT NEEDED` or create a new upgraded working file/report first; do not invent a master item silently.
6. Keep customer-facing quotation separate from internal BOQ cost build-up.

## AdditionalMaterials reference rule

`AdditionalMaterials/` is a supplemental price-reference area. It may contain supplier catalogs, screenshots, PDFs or price notes that are useful for active pricing before an item is fully added to the master lists.

For ActiveBOQ, AdditionalMaterials may be used to choose a provisional material price when the owner explicitly points to it, such as `AdditionalMaterials/SPC & Vynil` for SPC/Vinyl flooring.

Rules:

- Use the cheapest suitable option only when the owner asks for the cheaper option and the material still matches the customer request.
- If customer asked for SPC, choose the cheapest SPC item, not vinyl, unless owner accepts vinyl substitution.
- Record the selected item, rate, coverage, source folder and limitation in a new ActiveBOQ upgrade file.
- Mark it as provisional if it is not yet an exact `1.2 Materials.txt` master item.
- Do not silently treat AdditionalMaterials as the master list.
- Before final BOQ, either map the item to an existing master item, add/update the master list through a controlled file update, or keep it as an owner-approved provisional quotation line.

## Immutable source and upgrade-file rule

Do not edit original customer files, old catalog versions, PDFs, DOCX, Materials, Labour, README or Deep Research unless the owner explicitly asks to revise that exact file.

Customer originals such as `Customer Request.txt`, floor plans, drawings, photos and uploaded PDFs are source evidence. They must remain unchanged.

Every working correction, audit, BOQ, SPEC, measurement extraction or quotation draft must be saved as a new upgrade file in `ActiveBOQ/` with a clear version suffix, for example:

- `Customer_Request_Audit_V1.md`
- `Customer_Request_SPEC_V1.tsv`
- `ActiveBOQ_Takeoff_V1.tsv`
- `Customer_Quotation_Draft_V1.md`
- future corrections as V2, V3 and later.

If V5 catalog needs correction, create V6. Do not edit V5 directly unless the owner explicitly instructs a direct V5 correction.

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

The actual current repository overrides memory.

## Source order

Use sources in this order:

1. Latest explicit owner instruction.
2. This header for workflow rules.
3. ActiveBOQ current job files for customer-specific scope, drawings, floor plan, measurements and site notes.
4. Latest versioned catalog for matching guide prices, public wording and exclusions only where applicable.
5. `README - BOQ.txt` when catalog does not fully cover the requested scope or manual takeoff is required.
6. `1.2 Materials.txt` for material references.
7. `1.3 Labour.txt` for labour and installation references.
8. `AdditionalMaterials/` for owner-pointed supplemental material pricing where master-list item is missing or needs comparison.
9. README quotation rules for output discipline.
10. Deep Research only where it does not conflict.
11. PDF/DOCX as rendered reference.
12. Older drafts or stale branches.

## Versioning rule

Do not overwrite, delete, rename or move old catalog versions.

Old versions are references. Every meaningful public catalog update must create a new versioned file using the same front name and the next version number.

Current naming pattern:

- `SingleStoreyExtentionNRenovationV4.md`
- `DoubleStoreyExtentionNRenovationV4.md`
- `SingleStoreyExtentionNRenovationV5.md`
- `DoubleStoreyExtentionNRenovationV5.md`

Future versions continue as V6, V7 and later.

The latest V number is the current combined version. Older versions remain for audit, correction and rollback reference.

## Catalog and PDF delivery rule

A version is not customer-ready until the matching downloadable files exist or the owner has explicitly accepted Markdown-only use.

For each completed public version, provide at minimum:

- Markdown source for single-storey catalog;
- Markdown source for double-storey catalog;
- PDF render for single-storey catalog;
- PDF render for double-storey catalog;
- change report;
- customer answer sheet.

The PDF must be based on the matching same-version catalog source. If the PDF is not yet created, state that the catalog source exists but PDF delivery is still pending.

## Public catalog rule

Public catalog files must be customer-facing.

Do not place internal raw costing, profit, supplier names, GPT/Cursor/Codex notes, source-file notes or audit notes inside public catalog files.

Do not mention brand names unless the official quotation intentionally lists a brand/model.

Describe items by specification: material type, size allowance, finish tier, included quantity, route or site limitation, exclusions and quote-only items.

## Package scope rule

Catalog packages should read like normal homeowner renovation scope.

Basic, Standard and Better Finish should mainly differ by finish level, material tier, electrical/plumbing allowance, wet-area treatment and accessory allowance.

The catalog must let staff answer customer questions about tiles, skirting, ceiling, door/window allowance, electrical points, plumbing points, WC type, bathroom items, wet kitchen items, paint and exclusions.

## Price rule

Do not change catalog prices, size bands, thresholds or add-on guide prices unless the owner explicitly asks.

Material and labour files are internal support. They are not public selling prices.

## Header update rule

When the owner creates a permanent workflow rule, corrects a recurring mistake, changes source authority, or explicitly asks for header update, update this header in the same work session.

A chat apology or acknowledgement alone is not enough.

Do not update this header for routine progress.

## Work continuation rule

When the owner asks to update GitHub or create the next catalog version, ActiveBOQ file, BOQ, audit or quotation, do not stop at explanation if the safe next action is known.

Proceed with the smallest complete safe task. If blocked, state the exact block and exact owner action required.

## ActiveBOQ quotation test rule

For customer quotation work under `ActiveBOQ/`, use:

1. customer location and job label;
2. house type and storey type;
3. floor plan/drawing evidence;
4. work area and measured/assumed size;
5. package tier or finish level;
6. add-ons;
7. site risk notes;
8. catalog version used;
9. inclusions;
10. exclusions;
11. assumptions;
12. questions still required before final quotation.

Do not promise a brand/model unless written in the quotation.

## Known mistakes to avoid

- Do not make a new version by changing only the title.
- Do not copy vague V4 wording into a new version without clearer scope.
- Do not leave wording such as `Basic floor finish`, `Higher allowance`, `where stated` or `Better finish allowance` without explanation.
- Do not edit V4, V5, PDF, DOCX, Materials, Labour, README or Deep Research when creating a new version or working file.
- Do not edit customer originals such as `Customer Request.txt`, drawings, floor plans, photos or uploaded PDFs.
- Do not invent brands or exact models.
- Do not present floorplan estimates as final measured quantities.
- Do not treat AdditionalMaterials as master list unless it is formally added or mapped.
- Do not choose vinyl when customer asked for SPC unless owner approves substitution.
- Do not promise cabinets, premium glass, water heater, shower screen, DB upgrade, sewer/manhole work, authority fees or structural strengthening unless listed.
- Do not work in a hidden branch when the owner expects visible files in `main`, unless branch workflow is explicitly agreed.
- Do not request or use permission for `neprenkha/BOQ` when current work is `neprenkha/renovation`.
- Do not tell the owner V5 is fully ready if the PDF render is not yet created.
- Do not treat the root catalog as the active customer job; the active customer job is under `ActiveBOQ/`.
- Do not force custom renovation items into catalog package pricing when manual BOQ based on `README - BOQ.txt` is more suitable.
