# GPT HEADER — ACTIVEBOQ GENERAL WORK RULES

## Parent folder rule

`ActiveBOQ/` is a parent folder for many separate jobs.

It is not safe to treat `ActiveBOQ/` itself as one project workspace.

## Active workspace rule

The active workspace is always the exact folder named by the owner.

Examples:

```text
ActiveBOQ/Surau Nilai/
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/
```

GPT must write only inside the active workspace.

## Standard folder roles

Inside each project folder:

```text
GPT_CONTROL/
Takeoff_Work/
BOQ/
BOQ_work/
Drawing/
OriginalFile/
```

Use:

- `GPT_CONTROL/` for GPT rules, header, README, governance and file maps.
- `Takeoff_Work/` for measurements, takeoff notes, corrections and assumptions.
- `BOQ/` for customer estimate, quotation, BOQ, supplier files and final outputs.
- `BOQ_work/` for temporary/intermediate generated work.
- `Drawing/` only as read-only drawing/PDF reference.
- `OriginalFile/` only as read-only owner source/original reference.

## Read-only default

The following are read-only unless owner explicitly says otherwise:

- any `Drawing/` folder;
- any `OriginalFile/` folder;
- shared reference files such as Materials, Labour, README-BOQ, quotation README or price reference files.

## Write prohibition

GPT must not write generated files directly under:

```text
ActiveBOQ/
```

Generated files must go under the active project folder and suitable subfolder.

## Movement rule

If loose files already exist directly under `ActiveBOQ/`, move them only after identifying the correct project owner/site.

A controlled GitHub relocation is allowed when the owner instructs it.

Do not move files from one project folder to another unless explicitly told.

## Safety rule

Do not perform broad cleanup, recursive delete, overwrite-all, mirror sync or uncontrolled file movement.

For GitHub work, relocation must be old path to new path only.

## Current known project folders

```text
ActiveBOQ/Surau Nilai/
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/
```

## Current instruction lock

For `+60 13-731 9262 - fahrurrazy fr`, loose root files under `ActiveBOQ/` that belong to that client/site should be relocated into that project folder, not left scattered at `ActiveBOQ/` root.
