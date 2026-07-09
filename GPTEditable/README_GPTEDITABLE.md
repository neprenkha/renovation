# GPTEditable

This folder contains GPT-editable governance files for `neprenkha/renovation`.

## Editable file

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

## ActiveBOQ rule

Customer/site work must stay inside its own folder, for example:

```text
ActiveBOQ/Surau Nilai/
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/
```

Read-only source folders such as `Drawing/` and `OriginalFile/` must not be edited.
