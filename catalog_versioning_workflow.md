# Catalog Versioning Workflow

This workflow keeps old catalog references intact and creates a new catalog file set for every meaningful update.

## Main rule

Do not overwrite, delete, rename or move old catalog versions.

Every major customer-facing update must create a new versioned file set. Older versions remain as historical reference.

## Version naming

Use clear version suffixes:

- `_v4` = existing repaired public catalog source/reference.
- `_v5` = first detailed public catalog draft/spec version.
- `_v6` = next merged revision after V5 scope lock and latest Materials/Labour review.
- `_v7`, `_v8` and later = future updates.

Recommended file names:

- `single_storey_house_extension_public_catalog_v6.md`
- `double_storey_house_extension_public_catalog_v6.md`
- `catalog_v6_change_report.md`
- `catalog_v6_owner_decisions_required.md`

For later updates, increment the number only.

## Source hierarchy

Use this order when creating a new version:

1. Existing older catalog version for prices, customer wording and exclusions.
2. `catalog_v5_customer_scope_lock.md` for brandless customer-facing scope rules.
3. `1.2 Materials.txt` for approved material descriptions, UOM and rates.
4. `1.3 Labour.txt` for approved labour, service, rental and installation descriptions, UOM and rates.
5. Deep Research file for intended package logic only where it does not conflict with Materials/Labour/source catalog.
6. PDF/DOCX only as rendered layout/reference, not as the editing source unless no Markdown source exists.

## Brand rule

Public catalog files must describe item specification, material tier, size allowance, quantity and exclusions. Do not mention brand names unless the final official quotation intentionally lists that brand/model.

## Customer-answer rule

The catalog should let staff answer customer questions by specification:

- what type of tile is included;
- whether skirting is included;
- what ceiling board and design level is included;
- how many electrical points are included;
- what plumbing points are included;
- what WC type and bathroom items are included;
- what wet-kitchen items are included;
- what is excluded or quoted separately.

## Merge rule

Only merge a version branch when:

- all new versioned files are present;
- old versions remain unchanged;
- Materials/Labour references have been checked;
- public catalog wording does not expose internal cost, labour hours, supplier names or profit assumptions;
- change report confirms price preservation and file-scope safety.
