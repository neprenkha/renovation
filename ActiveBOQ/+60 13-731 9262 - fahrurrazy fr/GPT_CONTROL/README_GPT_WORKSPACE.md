# README — GPT Workspace for +60 13-731 9262 - fahrurrazy fr

## Workspace boundary

This client/site workspace is:

```text
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/
```

The parent folder `ActiveBOQ/` stores multiple separate jobs. It is not the working folder for this client/site.

## Folder purpose

| Folder | Purpose |
|---|---|
| `GPT_CONTROL/` | GPT header, workspace rules, relocation notes |
| `Takeoff_Work/` | Measurement notes, dimension checks, correction logs |
| `BOQ/` | Customer estimate, quotation draft, cost/rate breakdown, final BOQ outputs |
| `BOQ_work/` | Intermediate drafts and temporary work notes; do not auto-delete |
| `Drawing/` | If owner later uploads drawings/original PDFs, read-only source |
| `OriginalFile/` | If owner later uploads original files, read-only source |

## Read-only rule

If `Drawing/` or `OriginalFile/` exists, GPT must treat it as read-only. Do not edit, rename, move, replace, overwrite, or delete source files.

## Output rule

All GPT-generated or reorganized files for this client/site must remain inside this workspace and should be placed in the appropriate subfolder.

## No destructive cleanup

Do not run or recommend cleanup/delete/mirror operations. GitHub moves should be handled as controlled relocation only after file list and destination are clear.