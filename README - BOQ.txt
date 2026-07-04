README - BOQ.xlsx WORKFLOW (S01-S100 + SUMMARY + SEARCH/PURCHASE)
Version: V2.2 (Simple Sections, No Sub-Headings)
Last update: 2026-02-16

============================================================
1) AUTHORITATIVE SOURCES (STRICT)
============================================================
- This README / tracker workflow (layout + rules)
- 1.2 Materials.txt (exact item names + UOM + rates if any)
- 1.3 Labour.txt (exact labour/rental/service names + UOM + rates if any)

Hard rules:
- Description MUST match master list text exactly (case/spaces).
- UOM MUST follow master list UOM for that Description.
- If required item does not exist in master list:
  - Do not invent a new name in BOQ.
  - Add item to Materials.txt or Labour.txt first, then use it.
- If SPEC is truly missing a required input, use NOTE prefix: INPUT NEEDED.
- Output format: Copy Code Tab Delimited only. No exceptions, no excuses. Unless User state otherwise, do not provide any other format

============================================================
2) CHANGE CONTROL (DO NOT LET AI REWRITE README)
============================================================
- AI MUST update ONLY the requested section(s).
- AI MUST NOT rewrite, reformat, reorder, renumber, or replace the entire README unless user explicitly requests full README replacement.
- AI MUST keep existing section numbers stable.
- AI MUST preserve unrelated sections exactly as they are.

- Section replacement rule:
  - When a correction changes, clarifies, or overrides an existing rule, AI MUST replace the whole affected section.
  - AI MUST NOT append overlapping bullets under old wording when the old wording can conflict, confuse, or create duplicate instructions.
  - Replacement section must remove the old conflicting wording and contain one clean final rule set.
  - Replacement section must keep the same section number and title unless user instructs otherwise.

- Sub-section / bullet replacement rule:
  - AI may replace a smaller bullet group only when the rest of the section has no conflict with the new rule.
  - If multiple bullets inside the same section are affected, replace the whole section.

- Exception:
  - If user explicitly requests "full README replacement", AI may output the full README once.

============================================================
3) MASTER LISTS (WHAT THEY CONTAIN)
============================================================
- Materials.txt:
  - Approved material item names (Description) and their allowed UOM (and optional rate).
  - This is the ONLY allowed source for material Description text.
- Labour.txt:
  - Approved labour / service / rental item names (Description) and their allowed UOM (and optional rate).
  - This is the ONLY allowed source for labour/service/rental Description text.
- Impact:
  - BOQ consolidation and summary grouping depends on identical Description text.
  - If the same function is needed across scopes, ALWAYS reuse the same master item.
- If the same approved Description appears multiple times with the same UOM, apply the Duplicate Rate Selection Rule in Section 12.

============================================================
4) WORKFLOW PHASES (CHATGPT MODE)
============================================================
- Phase 1: SPEC FIRST (A:C only)
  - Discuss and finalize SPEC in A:C until confirmed complete.
  - Do NOT fill any block values until SPEC is finalized.
- Phase 2: TAKEOFF + FILL BLOCKS
  - After SPEC is final, fill block values using master list exact names.
  - Output must be paste-ready TSV for INPUT columns only (formula columns are not pasted).
- Phase 3: REVIEW + SUMMARY + OVERRIDE
  - Check consistency across scopes (same items use same exact Description).
  - Use Search/Purchase override workflow for packaging and price overrides.
- Translation duty rule:
  - AI MUST NOT treat user explanations as informal chat only.
  - AI MUST translate the user's explanations, decisions, corrections, dimensions, structural logic, room use logic, service logic, and cost-saving method into detailed SPEC A:C rows before takeoff.
  - AI MUST convert user input into project-ready scope language so the sheet can function as a working BOQ/spec reference, not just a memory aid for the current session.
  - AI MUST assume that a future session may continue using SPEC A:C only, without access to the original conversation, so all critical user intent must be preserved in SPEC.

============================================================
5) SCOPE PLANNING + WORK SEQUENCE (CRITICAL)
============================================================
- When user provides multiple works in one message, AI MUST:
  - identify all distinct work scopes first
  - produce a Scope List in logical construction order
  - then map each scope to S01, S02, S03... in that same order
- AI MUST NOT reorder works randomly.
- If one project contains multiple building parts, AI MUST split the work by construction logic and structural dependency, not by random room names only.
- For extension / renovation / multi-zone jobs, AI MUST first identify whether the works belong to:
  - one shared structural system, or
  - separate structural systems / separate building blocks / separate add-on zones.
- If separate areas have different footing pad / ground beam / RC column / roof beam logic, AI MUST treat them as separate scopes or separate sub-scopes in sequence.
- For residential extension works, preferred structural sequence is:
  - footing pad + excavation + base formation
  - ground beam
  - RC column
  - roof beam / upper beam / tank support beam
  - roof frame / roof covering
  - wall / opening / finishing / services as relevant
- AI MUST distinguish clearly between:
  - wall line
  - beam line without wall
  - RC column point
  - footing pad point
- Beam lines without wall are still structural scope and must not be omitted from the relevant structural sheet.
- Structural correction rule:
  - If a correction affects footing pad or ground beam only, update the footing/ground beam scope only.
  - If a correction affects RC column, roof beam, tank support, or upper structural support only, update the upper structural scope only.
  - AI MUST NOT rewrite unrelated SXX sheets when the correction is local to one structural layer.
- Rule of thumb sequence (example):
  - Setting out / protection
  - Hacking / demolition / disposal
  - Structural / base / concrete / rebar / formwork
  - Drainage / plumbing rough-in
  - Waterproofing
  - Screed / leveling / plaster / skim
  - Tiling
  - Metal/roofing installation
  - Sealant / finishing
  - Final cleaning
- If scope order is unclear, AI must write CONFLICT note in SPEC A:C and stop before filling sheets.
- AI MUST ensure the proposed S01..SXX scope breakdown matches the real construction sequence and actual trade dependency of the project, not a generic or random grouping.
- AI MUST avoid both under-splitting and over-splitting. Each SXX must be small enough that a local correction can be made in that same sheet only, but large enough to remain a practical work package.
- AI MUST NOT use one oversized generic scope such as "finishing" to absorb unrelated trades.
- Finishing-stage works MUST be split by actual construction package where relevant, such as plaster/skim, ceiling, waterproofing, tiling, painting/final fittings, or equivalent project-specific trade sequence.
- Plumbing / internal cold water / sanitary, external drainage / longkang, roofing / rainwater goods, and electrical MUST be assigned to their correct trade scopes and must not be mixed randomly.
- For renovation and extension works, scope grouping MUST follow how the work will actually be built on site, so later corrections can be updated in the affected SXX only without reopening unrelated sheets.

============================================================
6) WHEN TO USE S01 ONLY VS SPLIT INTO S02..SXX
============================================================
- Option A (Small job, single scope):
  - Use S01 only for the entire job.

- Option B (Large job OR multiple scopes):
  - MUST split by scope into S01..SXX in construction sequence order.

- S01 numbering rule:
  - S01 is the first scope sheet in the project sequence.
  - S01 may be preliminaries only when the project has a confirmed preliminaries scope.
  - When the project has no separate preliminaries scope, S01 may be the first measured trade work.
  - AI MUST NOT force S01 to become preliminaries when the user has already mapped S01 to a measured work scope.
  - AI MUST follow the user-confirmed S01..SXX scope mapping for the current project.

- 45-row rule (SPEC length control):
  - If job has multiple scopes AND the combined SPEC A:C would exceed ~45 rows:
    - MUST split scopes into separate sheets (S01, S02, S03...) to keep each scope readable.
  - If job is ONE scope only:
    - Keep it in S01 even if SPEC exceeds 45 rows.
    - Do NOT split one single scope into multiple sheets merely to reduce row count.

- Naming rule:
  - Each sheet SXX SPEC A:C must clearly state the scope title and key measurements for that scope.

- Additional structural split rule:
  - If the project contains multiple structural layers, AI MUST split by structural layer even if the physical area is small.
  - Minimum recommended split for extension works with structure:
    - one sheet for footing pad + ground beam
    - one sheet for RC column + roof beam / upper structural support

- Special support rule:
  - If a special supported item exists, such as overhead water tank support zone, AI MUST place that work under the relevant structural sheet only, not create a duplicate random scope unless the support system is truly independent.
  - If the tank/platform/support uses the same new structural system, AI MUST keep it inside the same structural sheet and note the correction in SPEC.
  - If the tank/platform/support requires a fully separate support frame or separate foundation system, AI may split it into a new SXX structural sub-scope.

- Sequence reservation rule:
  - AI may prepare SXX sheets in sequence order even when some intermediate scopes are not yet priced.
  - If a scope exists in sequence but has no confirmed chargeable work, keep the sheet/SPEC reserved and do not force block filling.
  - AI MUST NOT skip an earlier sequence just because a later structural or service scope is easier to price first.

- Scope size rule:
  - AI MUST avoid both under-splitting and over-splitting.
  - Each SXX must be small enough that a local correction can be made in that same sheet only.
  - Each SXX must be large enough to remain a practical work package.
  - If one proposed SXX still mixes too many unrelated trades or prevents local correction, AI MUST split it further into smaller sequence-based work packages.

============================================================
7) SPEC A:C FORMAT (HEADER + HOW TO WRITE)
============================================================
- Columns A:C are SPEC only (editable). They are for discussion, scope definition and takeoff preparation.
- Use this header in Row 1 (or the first SPEC row for each SXX):
  A = Spec
  B = Description
  C = Note

- Every SXX sheet MUST start with at least 2 SPEC rows:
  1) SXX-TITLE
  2) SXX-OVERVIEW

- Mandatory structure in every SXX:
  - A (Spec): SXX-TITLE
  - B (Description): Scope Title (short, clear)
  - C (Note): One-line objective and location
  - A (Spec): SXX-OVERVIEW
  - B (Description): Work description (what is included / excluded)
  - C (Note): Assumptions, constraints, access, working hours, protection needs

- SPEC output finality rule:
  - AI MUST NOT output SPEC A:C as a loose draft.
  - AI MUST output SPEC A:C only when it is complete enough to support accurate takeoff for that same SXX.
  - AI MUST NOT output repeated full SPEC A:C just to restate unchanged information.
  - AI may output SPEC A:C only when:
    - the user requests SPEC A:C
    - a confirmed input changed
    - a missing line was repaired
    - a conflict was resolved
    - the sheet was not previously produced in the current finalized form
    - a prior SPEC A:C output was wrong and must be superseded

- SPEC replacement rule:
  - When SPEC A:C needs replacement, AI MUST output the full affected SXX SPEC A:C, not only edited rows.
  - The replacement SPEC A:C must supersede the previous affected SPEC A:C.
  - AI MUST NOT output partial SPEC row edits unless the user explicitly requests partial rows only.
  - AI MUST preserve all unrelated valid SPEC/USER-INPUT content inside the full replacement output.
  - AI MUST remove or correct the wrong/conflicting rows inside the full replacement output.

- Before asking user rule:
  - Before asking the user for information, AI MUST first check:
    - current conversation input
    - previous user-confirmed input
    - existing SPEC A:C
    - USER-INPUT row
    - uploaded README / Materials / Labour files
    - prior handover tracker or saved project memory
  - AI MUST NOT ask the user to repeat information that already exists in those sources.
  - AI may ask only for information that is truly missing, contradictory, or impossible to infer from existing project context.
  - Such question must be recorded with NOTE prefix: INPUT NEEDED in SPEC A:C.

- After the first 2 mandatory rows, write SPEC items in the same sheet, grouped logically.
- Each line should describe ONE measurable, verifiable, or rule-setting input.
- Avoid mixing unrelated inputs in one row.

- For structural scopes, SPEC A:C MUST record support logic clearly before takeoff.
- Structural SPEC must state, where relevant:
  - footing pad points
  - RC column points
  - ground beam lines
  - roof beam / upper beam lines
  - beam lines without wall
  - wall lines
  - special support zones
- AI MUST record whether a support point is:
  - new structural point, or
  - existing structural support point used as tie-in/reference
- AI MUST NOT use vague wording such as:
  - near existing footing
  - use nearby support
- AI MUST state load-path logic clearly where relevant.
- If the user corrects the structural layout, AI MUST update only the affected structural logic inside the full affected SPEC A:C replacement and preserve unrelated valid SPEC/USER-INPUT content.

- Examples of SPEC line types:
  - Dimensions/quantities:
    - A: SXX-DIM
    - B: Area/length/height/qty description
    - C: Values with units (mm, m, sqm, pcs) and references (drawing/photo/onsite)
  - Method/sequence requirement:
    - A: SXX-METHOD
    - B: Key method requirement
    - C: Constraints / conditions / limits
  - Material/brand rule:
    - A: SXX-MATERIAL-STD
    - B: Standardize item
    - C: Use same Description as Materials.txt item: <Exact Name>

- Detailed translation rule:
  - AI MUST expand and translate user instructions into sufficiently detailed SPEC A:C language in the style of working BOQ/spec notes.
  - AI MUST NOT leave critical user explanations only in short vague phrases if those explanations affect:
    - level logic
    - structural logic
    - wall vs beam distinction
    - opening logic
    - roof type and fall direction
    - plumbing logic
    - electrical logic
    - tank limitation
    - room usage
    - finish scope
    - cost-saving construction method
  - If the user gives practical construction logic in plain language, AI MUST restate that logic clearly in SPEC A:C as technical scope notes.
  - AI MUST write SPEC in a way that another AI or estimator can continue the BOQ later without repeatedly asking for the same floor plan explanation, support-point explanation, or room-use explanation.
  - AI MUST NOT over-shorten important user decisions into generic wording such as "follow plan" or "as discussed" when the logic can be stated directly in SPEC.
  - If dimensions, support points, beam lines, opening sizes, tank limits, floor drops, or service routes are already explained by the user, AI MUST capture them explicitly in SPEC A:C.

- Takeoff-ready completion test:
  - A sheet is considered complete only when, using:
    - that same SXX SPEC A:C
    - Materials.txt
    - Labour.txt
    AI can fill block 1-3 accurately, or leave them accurately empty when the sheet is intentionally reserved/nil.
  - If AI cannot determine exact quantity logic, exact nil status, or exact chargeable scope for that sheet, the sheet is not complete.
  - A non-complete sheet must be repaired in SPEC first.
  - AI MUST NOT call a sheet complete or takeoff-ready unless it passes this test.

- Spec completion rule:
  - If pasted SPEC lacks required takeoff details:
    - AI MUST first check previous input and project context.
    - AI MUST add the missing SPEC lines that can be derived from existing context.
    - AI MUST mark derived/default values using NOTE prefix: DEFAULT USED.
  - If there is a contradiction:
    - AI MUST flag it using NOTE prefix: CONFLICT.
    - AI MUST stop before filling SXX blocks until conflict is resolved.
  - If required input is truly missing and cannot be derived:
    - AI MUST write NOTE prefix: INPUT NEEDED and list the exact question needed.

- Important:
  - SPEC A:C is where the real discussion happens.
  - AI must not jump into takeoff blocks until SPEC A:C is coherent, complete and takeoff-ready.
  - AI must not ask again for input that is already provided in current context, previous user input, SPEC, USER-INPUT, project memory, or uploaded files.

============================================================
8) WHAT AI MUST OUTPUT AFTER SPEC IS FINAL
============================================================
- AI must output paste-ready TSV for INPUT columns only.
- The TSV copy-code block must contain tab-delimited table data only.
- Target headers must be written outside the copy-code block.

- Target header placement rule:
  - Every copy-code TSV block MUST have a plain-text target header outside and immediately above the copy-code block.
  - The target header MUST NOT be placed inside the TSV copy-code block.
  - The target header MUST use the actual sheet number and exact paste range.
  - AI MUST NOT output a TSV block without its target header.

- SPEC header format:
  - Paste to SXX!A:C - SPEC

- Block 1 header format:
  - Paste to SXX!E:K - Materials Block

- Block 2 header format:
  - Paste to SXX!P:V - Labour Block

- Block 3 header format:
  - Paste to SXX!AA:AG - Service Block

- Example target headers:
  - Paste to S01!A:C - SPEC
  - Paste to S01!E:K - Materials Block
  - Paste to S01!P:V - Labour Block
  - Paste to S01!AA:AG - Service Block

- After SPEC A:C is final, AI must output EXACTLY 3 TSV blocks per priced SXX:
  - Block 1 / Materials (paste into E:K):
    Note | Spec | Description | UOM | Usage Qty | Wastage/Buffer | Price/Unit (RM)
  - Block 2 / Labour (paste into P:V):
    Note | Spec | Description | UOM | Usage Qty | Wastage/Buffer | Rate (RM)
  - Block 3 / Service (paste into AA:AG):
    Note | Spec | Description | UOM | Usage Qty | Wastage/Buffer | Rate (RM)

- No-repeat block rule:
  - AI MUST NOT output the same SXX block 1-3 repeatedly when there is no change.
  - AI may re-output a block only when:
    - user requests a fresh paste block
    - a confirmed value changes
    - an item is added, corrected, or made obsolete
    - a formula/error audit requires replacement
    - a prior block was wrong and must be replaced in full
  - When replacing a wrong block, AI MUST clearly state that the new block replaces the previous block.
  - AI MUST NOT keep giving alternate partial versions that cause duplicate paste work.

- AI must not output any Total (RM) columns.
- AI must not paste into formula columns:
  - Materials formula columns: L:M:N
  - Labour formula columns: W:X:Y
  - Service formula columns: AH:AI:AJ

- Wastage/Buffer column rule:
  - Wastage/Buffer MUST be entered as a ratio multiplier only.
  - For 10% wastage, enter 0.10.
  - For 5% wastage, enter 0.05.
  - For 0% wastage, enter 0.
  - AI MUST NOT enter absolute waste quantity in Wastage/Buffer.
  - Wrong: Usage Qty 267.08 and Wastage/Buffer 26.71.
  - Correct: Usage Qty 267.08 and Wastage/Buffer 0.10.
  - For standalone, full purchase, full pack, full allowance, or already-rounded purchase quantities, enter the final full quantity in Usage Qty and enter Wastage/Buffer as 0.
  - AI MUST verify that Usage Qty x (1 + Wastage/Buffer) produces the intended workbook quantity before outputting the block.

- Block fill rule:
  - AI must fill block 1-3 only for scopes with confirmed chargeable work supported by the same sheet's SPEC A:C.
  - Reserved or nil SXX scopes must keep block 1-3 empty.
  - AI MUST NOT duplicate preliminaries, labour, rental, or service items across different SXX sheets.
  - AI MUST ensure block 1-3 follows the same SXX logic already locked in SPEC A:C.

- Accurate takeoff rule:
  - AI MUST NOT fill block 1-3 from Materials.txt and Labour.txt alone when the same sheet's SPEC A:C is not takeoff-ready.
  - Master lists provide approved item names, UOM, and rates only; they do NOT provide project quantities by themselves.
  - The same SXX sheet must already explain:
    - what work belongs to that sheet
    - where the work is
    - what quantity logic applies
    - what key sizes, counts, routes, or limits are locked
    - whether the correct result is priced work or nil work
  - AI MUST NOT guess quantities, MH, rental, or service requirements just because a sheet exists.

- Readiness test before output:
  - AI MUST internally verify that this exact SXX A:C + Materials.txt + Labour.txt can produce an accurate block result.
  - Failing that test means AI must repair SPEC first.
  - Passing that test permits final paste-ready block output only.

============================================================
9) NOTE PREFIX STANDARD (FOR AUDIT)
============================================================
- Notes are text-only and must stay in the Note column.
- Allowed prefixes:
  - CALC NOTE: derived from SPEC A:C geometry, user-locked input, or calculation logic
  - DEFAULT USED: used a project default value that is final for the current paste block
  - CONFLICT: spec contradiction or mismatch; block output stops until resolved
  - INPUT NEEDED: blocked because SPEC truly lacks critical input OR master item is missing

- Do NOT use INPUT NEEDED when the value can be derived from SPEC A:C, USER-INPUT, master lists, or user-locked decisions.

- Finality rule:
  - Notes must explain the final calculation basis only.
  - Notes must not contain uncertain acceptance wording.
  - Prohibited note wording includes:
    - acceptable
    - tentative
    - maybe
    - approximate
    - unclear
    - needs clearer note
    - can be accepted
    - partially correct
  - Prohibited Malay wording includes:
    - kurang tepat
    - boleh diterima
    - note kena jelas
    - belum
    - kalau
  - A finalized value must be output as final.
  - A non-final value must not be output in block 1-3.
  - The correct action for non-final data is SPEC repair first, then final TSV output.

============================================================
10) UPDATE-ONLY RULE (NEVER DELETE)
============================================================
- Never delete old useful lines.
- If a line becomes obsolete:
  - Set Usage Qty = 0
  - Explain why in Note
- Add new lines below existing ones.

============================================================
11) CONSISTENCY RULE (CRITICAL FOR CONSOLIDATION)
============================================================
- If S01 uses a specific master item (brand/type), S02..S100 MUST use the SAME exact item for the same purpose.
- Reason: consolidation by Description requires identical text.
- If you intentionally change an item (brand/type) in later scopes:
  - Write the reason in SPEC (A:C) and in the row Note.
  - Keep the old row (update-only) and set Usage Qty = 0 for obsolete line.

============================================================
12) SUMMARY + SEARCH/PURCHASE OVERRIDE (PACKAGING + PRICE)
============================================================
- Goal:
  - Keep takeoff sheets (S01..S100) as "auto/mapping" quantities.
  - Do packaging rounding and vendor pricing decisions in Purchase override flow.
- Summary:
  - Consolidates items by exact Description across selected sheets.
- Purchase:
  - Stores override records (manual edits) for packaging and price.
- Search:
  - UI sheet to search Summary items and manage Purchase overrides.
- Override use cases:
  - Convert small packaging to bulk (example: sand bags -> truck/trip).
  - Round up to supplier pack size (example: need 15 pcs but supplier sells 16 pcs).
  - Force one brand/type across scopes by overriding and zeroing obsolete lines (update-only rule).
- Duplicate rate selection rule:
  - If the same Description appears more than once in Materials.txt or Labour.txt with the same UOM and the same practical function/purpose, AI MUST use the highest Price/Unit (RM) or Rate (RM) as the default takeoff rate.
  - This rule applies only when:
    - Description is the same
    - UOM is the same
    - the item is clearly the same practical item/function
  - AI MUST NOT average the rates.
  - AI MUST NOT randomly choose a lower duplicate rate.
  - If a lower rate is intentionally chosen later, that decision must be handled through Purchase/Search override and the reason must be recorded.
  - Example:
    - If Coarse Sand (10-Wheel Truck) appears at RM850 and RM860, use RM860.
    - If 3/4" Aggregate (10-Wheel Truck) appears at RM830 and RM850, use RM850.
    - If the same item appears with different UOM or clearly different variants/specs, AI MUST NOT treat them as the same duplicate item.

============================================================
13) LABOUR PRODUCTIVITY RULES
============================================================
- All Man-Hour (MH) outputs must be final workbook labour quantities.
- Labour Description and UOM must match Labour.txt exactly.
- Labour rows must use the approved master Labour rate from Labour.txt.

- Standard labour master rates:
  - Labour - General Helper (Per MH): use Labour.txt rate.
  - Labour - Skilled Worker (Per MH): use Labour.txt rate.
  - Tukang, wireman, fabricator, installer, mason, plasterer, painter, and skilled trade work use Labour - Skilled Worker (Per MH) unless a more specific approved Labour.txt item exists.

- Productivity-based MH rule:
  - MH must use realistic productivity, not ideal productivity.
  - Standard efficiency factor: 0.65.
  - When an ideal/base MH is used, realistic MH = ideal/base MH / 0.65.
  - Logistics & handling allowance: +20%.
  - Sequence & interruption allowance: +15%.
  - Complexity guidance:
    - Light work (paint/clean): 0.80
    - Medium work (brick/plaster/tile): 0.65
    - Heavy/structural (hacking/G25 infill/rebar): 0.55

- User-locked labour cost conversion rule:
  - When the user has locked labour by m2, sqft, point, set, lump sum, or other project rate, AI must convert that approved labour cost into MH using the relevant master Labour rate.
  - Formula:
    - Final MH = Approved Labour Cost / Master Labour Rate
  - Example:
    - User locked RM24/m2 for 32.05m2.
    - Approved labour cost = 32.05 x 24 = RM769.20.
    - Master skilled worker rate = RM22.50/MH.
    - Final MH = 769.20 / 22.50 = 34.1867 MH.
  - This converted MH is the final workbook quantity for that user-locked labour basis.

- Labour Wastage/Buffer rule:
  - Labour Wastage/Buffer must be 0 unless the user explicitly locked a separate labour buffer.
  - AI MUST NOT add extra labour buffer to a user-locked labour cost.
  - AI MUST NOT double-count productivity allowance after converting a user-locked final labour cost into MH.

- Labour output rule:
  - AI must output final MH only.
  - AI must not output labour rows with tentative language, partial confidence, or status commentary.
  - AI must verify that Usage Qty x Rate equals the intended approved labour cost before outputting the block.

============================================================
14) USER-INPUT ROW TEMPLATE (FOR EVERY SXX SHEET)
============================================================
- All user instructions, clarifications, agreed details, and technical decisions relevant to the scope/block generation must be recorded directly in SPEC A:C after the last SPEC line (e.g. SXX-USER-INPUT).
- The USER-INPUT row is the single authoritative reference for all user inputs for block 1-3 generation in that sheet/scope.
- User inputs need only be written once in the USER-INPUT row when there are no changes.

- Authority rule:
  - The user's own inputs, corrections, confirmations, and locked decisions are authoritative.
  - GPT commentary from older sessions is context only.
  - GPT commentary is not authoritative when it conflicts with the user's confirmed input.
  - If old GPT commentary conflicts with user-confirmed input, AI MUST follow the user-confirmed input and flag the conflict.

- Before asking user rule:
  - Before asking any question, AI MUST check:
    - current chat
    - previous user-confirmed input
    - uploaded file contents
    - saved project memory
    - existing SPEC A:C
    - USER-INPUT row
    - Materials.txt
    - Labour.txt
  - AI MUST NOT ask the user to repeat a measurement, decision, rate, scope boundary, or correction that was already provided.
  - AI may ask only for a truly missing or conflicting input.
  - The exact missing/conflicting input must be recorded with NOTE prefix: INPUT NEEDED or CONFLICT.

- Update rule:
  - Specification lines (SPEC A:C) may be updated or added as scope changes or information is refined.
  - When user input changes, AI must update the technical meaning inside the affected SPEC A:C.
  - As long as the USER-INPUT row remains up to date and unchanged, it does not need to be re-written for each revision.

- Full replacement rule for paste outputs:
  - AI MUST NOT output row-only edits for workbook paste replacement unless the user explicitly requests partial rows only.
  - When SPEC A:C is wrong, incomplete, contradicted, or affected by a confirmed change, AI MUST output the full affected SXX SPEC A:C replacement.
  - When Block 1 / Materials is wrong, incomplete, contradicted, or affected by a confirmed change, AI MUST output the full affected SXX Block 1 replacement.
  - When Block 2 / Labour is wrong, incomplete, contradicted, or affected by a confirmed change, AI MUST output the full affected SXX Block 2 replacement.
  - When Block 3 / Service is wrong, incomplete, contradicted, or affected by a confirmed change, AI MUST output the full affected SXX Block 3 replacement.
  - A replacement must be complete, paste-ready, and must supersede the previous affected output.
  - AI MUST preserve valid unchanged content inside the full replacement output.
  - AI MUST remove, zero, or correct only the wrong/obsolete content according to the relevant rule.

- No-repeat rule:
  - AI MUST NOT repeatedly output the same A:C or block 1-3 content when no input changed.
  - AI MUST NOT create repeated versions that force the user to compare multiple nearly identical outputs.
  - AI MUST output a replacement only when a previous output is wrong, incomplete, contradicted, or affected by a confirmed change.
  - AI MUST clearly identify that the replacement supersedes the previous affected output.

- Omission rule:
  - AI is strictly forbidden from disregarding, prompting again, or omitting any input that remains recorded in the USER-INPUT row.
  - Any omission, overwriting, or unnecessary rewriting of USER-INPUT or unrelated SPEC lines is a workflow violation.

- Structural correction decisions from the user MUST be stored in USER-INPUT, especially:
  - support point corrections
  - footing pad additions/removals
  - beam line corrections
  - wall-line vs beam-line clarification
  - tank support limitation / tank class limitation
- If the user confirms that a change is local to one structural layer only, AI MUST not reopen or rewrite unrelated SXX sheets.

- Session continuity rule:
  - USER-INPUT is not a dumping row only.
  - AI MUST also translate the same confirmed information into the relevant SPEC rows where it affects actual scope, method, dimension, or limitation.
  - AI MUST NOT rely on USER-INPUT alone if the information is important for takeoff or scope understanding.
  - USER-INPUT stores the decision history; SPEC rows must store the working technical meaning of that decision.

============================================================
15) HANDOVER (PASTE THIS TO NEW SESSION)
============================================================
- We use BOQ.xlsx with S01..S100 + SUMMARY + Search/Purchase override.
- SPEC is A:C only; D is blank spacer.
- Each SXX has 3 blocks only:
  - Block 1 / Materials: E:N, paste E:K only
  - Block 2 / Labour: P:Y, paste P:V only
  - Block 3 / Service: AA:AJ, paste AA:AG only

- Paste target header rule:
  - Every paste block must show the target header outside and immediately above the copy-code TSV block.
  - The target header must use the actual sheet number and exact paste range.
  - The target header must not be included inside the TSV data.
  - The TSV copy-code block must contain tab-delimited table data only.

- Paste target headers:
  - SPEC:
    - Paste to SXX!A:C - SPEC
  - Block 1 / Materials:
    - Paste to SXX!E:K - Materials Block
  - Block 2 / Labour:
    - Paste to SXX!P:V - Labour Block
  - Block 3 / Service:
    - Paste to SXX!AA:AG - Service Block

- Description + UOM must match master lists exactly.
- Multiple scopes must be mapped to S01..SXX in construction sequence order.
- SPEC A:C must be finalized before Materials/Labour/Service blocks.
- After SPEC is final, AI must output 3 TSV blocks for input columns only.
- AI must not touch formula columns.
- AI must not output Total columns.
- A sheet may exist in sequence with empty block 1-3 when the scope is reserved or nil.
- AI must not jump sequence logic.
- AI must not force pricing into a sheet that does not own that scope.

- Paste-ready audit rule:
  - Before outputting any TSV block, AI must verify:
    - The correct target header is outside and immediately above the copy-code block.
    - The block is not a repeated output of unchanged data.
    - Description exactly matches Materials.txt or Labour.txt.
    - UOM exactly matches Materials.txt or Labour.txt.
    - Wastage/Buffer uses ratio format, not absolute quantity.
    - Standalone/full purchase quantities use Usage Qty as final full quantity and Wastage/Buffer as 0.
    - Labour MH follows the approved user-locked costing basis or realistic productivity basis.
    - Labour Wastage/Buffer is 0 unless user locked a separate labour buffer.
    - No formula columns are included.
    - No Total columns are included.
    - The resulting workbook formula total matches the intended cost logic.
  - AI must not output workbook blocks with tentative language or partial confidence.
  - Output must be final paste-ready TSV only.

- No-repeat handover rule:
  - AI must not repeatedly hand over the same A:C or block 1-3 content when no confirmed value changed.
  - A handover must identify the latest valid output and mark wrong earlier output as superseded when applicable.
  - The next session must continue from the latest valid user-confirmed data, not from old GPT commentary.

- Future-session continuity rule:
  - SPEC A:C must be detailed enough that a new AI session can continue scope review and block 1-3 takeoff with minimal repeated questioning.
  - Each priced SXX must be takeoff-ready on its own.
  - USER-INPUT must preserve the user's confirmed decisions.
  - GPT commentary from old sessions is not authoritative unless it matches the user's confirmed input.
  - AI must check prior user-confirmed input before asking the user to repeat details.

- Acceptance test:
  - A sheet is complete only when the next AI can use:
    - that same SXX A:C
    - Materials.txt
    - Labour.txt
    to fill block 1-3 accurately, or leave them accurately empty when the sheet is nil/reserved.
  - A sheet that still requires basic quantity logic repair is not complete and must not proceed to block pricing.
END.
