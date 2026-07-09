# README — ActiveBOQ GPT Workspace

## Purpose

`ActiveBOQ/` is the parent folder for multiple customers, sites and BOQ jobs. It is not itself a single project workspace.

Every job must live in its own folder under:

```text
ActiveBOQ/<customer-or-site-name>/
```

Examples:

```text
ActiveBOQ/Surau Nilai/
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/
```

## Core rule

When the owner tells GPT to work in a folder, that folder becomes the hard boundary.

GPT must not write outside the named folder.

Example:

```text
Work area: ActiveBOQ/Surau Nilai/
```

means GPT may only create or edit files under:

```text
ActiveBOQ/Surau Nilai/
```

and must not write in:

```text
ActiveBOQ/
```

or any other client/site folder.

## Standard project folder layout

Each job folder should use this structure where applicable:

```text
GPT_CONTROL/
Takeoff_Work/
BOQ/
BOQ_work/
Drawing/
OriginalFile/
```

| Folder | Purpose | GPT write rule |
|---|---|---|
| `GPT_CONTROL/` | Header, README, guardrails, work instructions | Can write |
| `Takeoff_Work/` | Takeoff notes, measurements, correction logs | Can write |
| `BOQ/` | Estimate, quotation, BOQ, supplier files | Can write |
| `BOQ_work/` | Intermediate work files | Can write, but do not auto-delete |
| `Drawing/` | Uploaded PDFs/drawings | Read-only |
| `OriginalFile/` | Owner original/source files | Read-only |

## Repository-level references

Files at repository root or parent folders may be shared references. Examples may include:

```text
README - BOQ.txt
README Quotation
Materials.txt
Labour.txt
```

Shared reference files are read-only unless owner explicitly says to edit that exact file.

## No loose project files in ActiveBOQ root

Generated project files must not be placed directly under:

```text
ActiveBOQ/
```

Loose files directly under `ActiveBOQ/` must be moved into the correct client/site workspace.

## No destructive operations

GPT must not perform broad cleanup, recursive delete, mirror sync, overwrite-all or uncontrolled file movement.

Moving a file in GitHub must be a controlled relocation from a known old path to a known new path, within the correct project folder.

## Owner instruction law

If owner says a folder is read-only, GPT cannot write there.

If owner says a folder is the workspace, GPT must not go outside it.

If owner says to create new work files, GPT must create them inside the appropriate subfolder of the active workspace, not scattered in the parent folder.
