# GPTEditable

This folder contains GPT-editable governance files and approved editable reference addendum files for `neprenkha/renovation`.

## Editable governance file

```text
GPTEditable/GPT Header Renovation.md
```

This is the canonical editable copy of the renovation GPT header. When a permanent general workflow rule changes, update this header and keep the root visible header aligned:

```text
GPT Header Renovation.md
```

## Owner local header

The owner also uses a local/pasted start-work header:

```text
GPTRenovationHeader.txt
```

When GPT is asked to provide this file for download, GPT must provide the full cumulative replacement header, not a short summary and not a patch-only update.

The downloadable owner header must preserve the useful current rules from the prior header and add the new rule cleanly. Do not remove unrelated valid sections just to shorten the file.

## Editable reference addendum

Root master files are read-only unless owner explicitly asks direct edit:

```text
README - BOQ.txt
1.2 Materials.txt
1.3 Labour.txt
```

If a BOQ/SXX item is not available in those root master lists, work must not stop. GPT must create or update editable supplemental reference files under:

```text
GPTEditable/Reference_Addendum/
```

Approved addendum files may include:

```text
GPTEditable/Reference_Addendum/README_REFERENCE_ADDENDUM.md
GPTEditable/Reference_Addendum/1.2_AdditionalMaterials_OnlineReference.txt
GPTEditable/Reference_Addendum/1.3_AdditionalLabourServices_OnlineReference.txt
```

The addendum files must follow the same tab-delimited column style as the root master lists where applicable:

```text
No	Category	Subcategory	Description	Qty	UOM	Price/Unit (RM)	Total (RM)	Update Date	Supplier	Note
```

Each online/provisional reference must record update date, supplier/source, status and note. If online search does not produce a reliable exact source, GPT may use a logical working-cost reference but must mark it clearly as `CURRENT WORKING COST BASIS`, `MARKET CHECKED - INTERNAL COST BASIS`, `SUPPLIER QUOTE NEEDED`, or `SELLING RATE USED` where applicable. Do not leave any required SXX line as NIL/blank only because a root master item is missing.

## SXX finality / no-hanging-cost rule

For each SXX, GPT must complete the SXX as a muktamad working-cost basis before moving to the next SXX.

`PROVISIONAL` must not be used merely because GPT has not found a material/labour price. If a root master item is missing, GPT must use web/current search, approved addendum reference, logical working-cost basis, or supplier-needed remark and still fill the SXX line.

A line may be marked `SUPPLIER QUOTE NEEDED` for later commercial confirmation, but the SXX cannot be left hanging: quantity, UOM, working rate basis, amount, markup status and audit note must still be filled.

Use `PROVISIONAL` only for real unresolved design/source conflicts, drawing unreadability, or owner scope decisions that cannot be resolved from existing material. The exact reason must be written.

## Markup / selling-rate rule

Root master files `1.2 Materials.txt` and `1.3 Labour.txt` are treated as cost / unmarked-up working rates unless the line itself states otherwise.

Every SXX rate line must state its markup status:

- `NO MARKUP - ROOT COST`;
- `NO MARKUP - ADDENDUM COST BASIS`;
- `MARKET CHECKED - NO MARKUP WORKING COST`;
- `SELLING RATE USED`;
- `MARKUP INCLUDED / DO NOT MARK UP AGAIN`;
- `SUPPLIER QUOTE NEEDED BEFORE CUSTOMER PRICE`.

If a rate appears to be a retail package, subcontract complete rate, selling rate, or already-marked-up rate, GPT must remark it clearly to avoid double markup, underquote or overprice.

## Cross-SXX contradiction / double-count rule

When working on any later SXX, if GPT finds a contradiction, overlap, duplicate scope, missing scope, undercost risk or overprice risk affecting a previous SXX, GPT must stop and revise the affected SXX first.

Required correction workflow:

1. create the next cumulative version of the affected SXX file;
2. preserve useful content from the previous version;
3. correct the double count / undercount / rate status / markup note;
4. update the SXX tracker;
5. update any overall summary if it already exists;
6. only then continue to the current SXX.

Do not wait until the end of the project to fix a known contradiction.

## BOQ.xlsm paste-ready output rule

Audit/takeoff files are not the same as owner paste files.

For every SXX that must be pasted into `*BOQ.xlsm`, GPT must produce a separate paste-ready `.txt` file or copy block that follows `README - BOQ.txt` exactly.

The valid paste targets are:

```text
Paste to SXX!A:C - SPEC
Paste to SXX!E:K - Materials Block
Paste to SXX!P:V - Labour Block
Paste to SXX!AA:AG - Service Block
```

The target header must be outside and immediately above each TSV block. The target header must not be included inside the TSV data.

The TSV data must contain only the workbook input columns:

```text
SPEC A:C:
Spec	Description	Note

Block 1 E:K:
Note	Spec	Description	UOM	Usage Qty	Wastage/Buffer	Price/Unit (RM)

Block 2 P:V:
Note	Spec	Description	UOM	Usage Qty	Wastage/Buffer	Rate (RM)

Block 3 AA:AG:
Note	Spec	Description	UOM	Usage Qty	Wastage/Buffer	Rate (RM)
```

GPT must not include audit-only columns, total columns, formula columns, GitHub status columns, source-drawing columns, raw/deduction/net columns, or long review tables inside BOQ.xlsm paste blocks.

If an audit/takeoff file has those extra columns, GPT must clearly say it is for audit/reference only and must also provide the separate `BOQXLSM_PASTE_READY` file for owner paste.

## Drawing/spec source rule

Active job `Drawing/` folders contain customer/source specifications and are not optional background material.

For Surau Nilai, the drawing/spec source folder is:

```text
ActiveBOQ/Surau Nilai/Drawing/
```

Drawing files are read-only. GPT must use them as source evidence for takeoff and must not edit, rename, move, overwrite or delete them.

Before finalising any SXX or overall BOQ, GPT must show which drawing/source files were checked for that SXX. If a drawing cannot be read/rendered, mark it clearly as `UNREADABLE / NEEDS REVIEW`; do not silently ignore it.

## Auditable takeoff rule

Takeoff must be understandable by owner, QS, contractor, future GPT sessions and future reviewers. It is not only a private understanding for the current chat.

Every takeoff line must record enough detail to be rechecked later:

- SXX/trade;
- source drawing filename;
- sheet/title/revision/page where visible;
- measured element/location;
- dimension source;
- formula;
- raw quantity;
- deductions;
- net quantity;
- UOM;
- wastage;
- buffer/contingency if any;
- material/labour/addendum reference;
- status such as measured, drawing-derived, owner-corrected, muktamad working-cost basis, supplier quote needed, selling rate used or conflict.

If a line cannot be audited later, it is not a complete takeoff line.

## Previous-session / owner-correction rule

Before asking the owner a question or saying an item is unknown, GPT must check previous discussion/context, current header, GitHub governance, active workspace files, drawings, README, material/labour lists and addendum files.

For Surau Nilai, use owner-corrected `Lot 20093` as the governing working lot unless a later owner instruction changes it. If a drawing or older source shows another lot number, record it as a conflict; do not silently revert to the wrong lot.

## SXX copy-paste output rule

For BOQ costing, every SXX output intended for spreadsheet use must be produced as `.txt` tab-delimited content that can be copied into `.xls` / Excel in the exact `README - BOQ.txt` paste target format.

Markdown files may be used for notes/control and audit files may include extra columns, but the actual owner paste output must be a separate BOQ.xlsm paste-ready `.txt` file or block using only the workbook input columns.

## Correction-triggered updates

If the owner corrects GPT because GPT violated a workflow rule, shortened a required header, failed to update governance, touched the wrong scope, mixed projects, or repeated a preventable mistake, GPT must treat the correction as a possible governance failure.

If the correction is general/permanent, GPT must update the relevant governance files in the same session when GitHub is accessible:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTEditable/README_GPTEDITABLE.md   (if GPTEditable usage is affected)
```

If GitHub is not accessible, GPT must mark the change as `PENDING GITHUB UPDATE`, provide the full updated owner-copy header when asked, and then update GitHub as soon as access is available later.

A chat apology alone is not enough when the mistake shows the header or workflow guard failed.

## Not a project workspace

`GPTEditable/` is not an ActiveBOQ customer/site folder. Do not put BOQ, quotation, takeoff, drawing, original file or customer work output here.

Only governance files and approved reusable editable reference addendum files belong here.

## ActiveBOQ rule

Customer/site work must stay inside its own folder, for example:

```text
ActiveBOQ/Surau Nilai/
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/
```

Read-only source folders such as `Drawing/` and `OriginalFile/` must not be edited.
