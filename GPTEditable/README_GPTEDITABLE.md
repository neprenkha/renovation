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

Each online/provisional reference must record update date, supplier/source, status and note. If online search does not produce a reliable exact source, GPT may use a logical provisional reference but must mark it clearly as `PROVISIONAL ONLINE / MARKET SURVEY` or `LOGICAL PROVISIONAL RATE`.

## SXX copy-paste output rule

For BOQ costing, every SXX output intended for spreadsheet use must be produced as `.txt` tab-delimited content that can be copied into `.xls` / Excel in sequence:

```text
SPEC A:C
Block 1 material/product
Block 2 labour/plant/rental
Block 3 subcontract/specialist/service
summary/status/gate
```

Markdown files may be used for notes/control, but the actual BOQ paste output must be `.txt` when owner is preparing workbook-style costing.

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
