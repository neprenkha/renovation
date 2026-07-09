# Surau Nilai — Cursor Work Rules

## Absolute rule

The `Drawing/` folder is source reference only.

```text
ActiveBOQ/Surau Nilai/Drawing/
```

Do not modify anything in that folder.

## Allowed work area

All generated notes, extracted text, takeoff tables, working markdown, CSV, or BOQ draft files must be placed only under:

```text
ActiveBOQ/Surau Nilai/Takeoff_Work/
```

## Disallowed actions

Cursor must not perform any of the following:

- delete files or folders;
- run cleanup commands;
- run recursive remove commands;
- move source drawings;
- rename source drawings;
- overwrite source drawings;
- write outside `Takeoff_Work/` unless explicitly approved by owner;
- touch unrelated projects or folders.

## Shell restriction

Do not use shell delete commands. This includes but is not limited to:

```text
Remove-Item
rmdir
rd
del
erase
shutil.rmtree
git clean
robocopy /MIR
```

## Correct workflow

1. Read drawing filenames from `Drawing/`.
2. Create notes/tables in `Takeoff_Work/`.
3. Make takeoff detail first.
4. Keep all assumptions and unresolved questions visible.
5. Do not price until quantity takeoff is checked.

## Prompt discipline

Every future Cursor prompt for this project must say:

```text
Do not modify ActiveBOQ/Surau Nilai/Drawing/. Use it as read-only reference only. Write all work outputs only inside ActiveBOQ/Surau Nilai/Takeoff_Work/. Do not delete, clean up, move, rename, or overwrite any source file.
```

## Recovery/context note

This rule file exists because previous destructive cleanup behavior caused data loss. The safe default for Surau Nilai is read-only reference drawings and separated working output.