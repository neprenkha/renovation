# Surau Nilai — Discussion Capture

This file captures the project discussion so the work can continue without re-explaining the same points.

## Hard boundary

- Reference drawings are located in:

```text
ActiveBOQ/Surau Nilai/Drawing/
```

- The `Drawing/` folder is reference-only.
- Do not edit, rename, move, replace, delete, clean up, or reorganize anything inside `Drawing/`.
- All working material must be created inside:

```text
ActiveBOQ/Surau Nilai/Takeoff_Work/
```

## Current objective

Prepare a detailed takeoff first before final BOQ pricing.

The next work must focus on:

1. checking all uploaded drawing PDFs;
2. listing every drawing sheet/file used as source;
3. extracting measurable items;
4. recording dimensions, assumptions, and queries;
5. preparing a quantity takeoff table;
6. only then converting the takeoff into BOQ lines.

## Earlier geometry discussion captured

A roof geometry item was discussed before the file incident:

- Roof pitch: `35 degrees`.
- Roof type: `A roof / gable-type roof`.
- Total horizontal projection/span from edge to edge: `6150 mm`.
- Ridge is at the centre:

```text
3075 mm + 3075 mm
```

- Rise from eaves/projection edge line to ridge:

```text
rise = tan(35°) × 3075 mm
rise ≈ 2153 mm
```

- Therefore, if the 6150 mm is the total horizontal projection/span and the ridge is exactly centred, the ridge height above the eaves/projection line is approximately:

```text
2150 mm to 2153 mm
```

This calculation is geometry-only. It must still be checked against the actual drawing section/elevation before being used in final BOQ.

## Important working interpretation

- Do not assume drawing dimensions silently.
- If a dimension is missing, unclear, cropped, or depends on scale, record it under `Queries / Assumptions`.
- The work must produce a transparent takeoff trail so the owner can see how every quantity was derived.

## Data-loss incident safeguard for this project

Because a previous Cursor cleanup/delete instruction caused serious data loss risk, this project must follow stricter rules:

- No delete commands.
- No recursive cleanup.
- No shell-based removal.
- No moving or modifying reference drawings.
- No work outside the Surau Nilai project folder.
- No changes to `Drawing/`.
- Any temporary or extracted working file must stay under `Takeoff_Work/`.

## Status

This file is the discussion lock/capture for Surau Nilai takeoff continuation.