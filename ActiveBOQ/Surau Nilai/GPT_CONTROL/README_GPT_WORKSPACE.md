# README — GPT Workspace for Surau Nilai

## Purpose

This README tells GPT how to work when GitHub is attached for the Surau Nilai BOQ/takeoff project.

The working space is exactly:

```text
ActiveBOQ/Surau Nilai/
```

`ActiveBOQ/` is only a parent folder containing many different project folders. It is not the work boundary for this task.

## Current protected source folders

Read-only source/reference folders:

```text
ActiveBOQ/Surau Nilai/Drawing/
ActiveBOQ/Surau Nilai/OriginalFile/
```

`Drawing/` already exists and contains the uploaded PDFs. `OriginalFile/` may be created by owner later. Both are read-only.

Do not write generated work into these folders.

## GPT-created folders

Current GPT-created/control folders:

```text
ActiveBOQ/Surau Nilai/GPT_CONTROL/
ActiveBOQ/Surau Nilai/Takeoff_Work/
```

BOQ output folder from the uploaded BOQ README:

```text
ActiveBOQ/Surau Nilai/BOQ/
```

Temporary/intermediate folder, if needed:

```text
ActiveBOQ/Surau Nilai/BOQ_work/
```

Do not auto-clean or remove temporary folders. Leave them for owner review.

## Files in this folder

| File | Role |
|---|---|
| `GPT_HEADER_SURAU_NILAI.md` | Mandatory GPT header and boundary rule |
| `README_GPT_WORKSPACE.md` | Workspace explanation and folder map |

## Existing takeoff work files

The current takeoff working folder is:

```text
ActiveBOQ/Surau Nilai/Takeoff_Work/
```

Existing files there include:

```text
00_TAKEOFF_DETAIL.md
01_DISCUSSION_CAPTURE.md
02_TAKEOFF_METHOD.md
03_CURSOR_WORK_RULES.md
```

Those files hold the earlier takeoff capture and safety rules.

## What GPT must do next

Before generating BOQ foundation files, GPT should:

1. read this README;
2. read `GPT_HEADER_SURAU_NILAI.md`;
3. inspect the uploaded PDF drawing list from `Drawing/` as read-only;
4. build a drawing register;
5. create takeoff details in `Takeoff_Work/` or BOQ foundation outputs in `BOQ/`, depending on owner instruction;
6. keep all assumptions and queries visible;
7. never modify drawings or original source files.

## What GPT must not do

GPT must not:

- treat wider `ActiveBOQ/` as the work area;
- use local-drive paths as the active GitHub workspace;
- edit `Drawing/`;
- edit `OriginalFile/`;
- alter uploaded PDFs;
- create files randomly in unrelated folders;
- perform destructive cleanup;
- create pricing or block work before the foundation/takeoff is checked.

## Captured BOQ foundation requirement

The uploaded BOQ README says the previous foundation output is rejected. GPT must not patch isolated rows. It must rebuild affected foundation files only after reading and checking all sources.

The foundation rebuild includes:

- all 24 PDFs visually inspected;
- structural drawings 01–07 visually extracted;
- door/window/opening register corrected;
- exact TSV schemas preserved;
- S01 to S25 AC files rebuilt as full takeoff-ready specs;
- premix area recomputed from actual tarmac/premix boundary or labelled project-provisional;
- supplier files kept short with resolved quantities only;
- master coverage rebuilt against Materials and Labour references;
- deterministic validation performed before PASS.

## Working rule summary

The owner instruction is:

```text
Ruang kerja ialah ActiveBOQ/Surau Nilai.
Drawing atau OriginalFile hanyalah rujukan.
Kalau nak buat kerja, buat folder/fail baru dalam ActiveBOQ/Surau Nilai.
Jangan keluar dari ActiveBOQ/Surau Nilai.
```

GPT must obey this as the top-level project law for this GitHub task.
