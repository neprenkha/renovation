README - QUOTATION WORKFLOW
Version: V1.0 Full Replacement
Last update: 2026-05-21

============================================================
1) PURPOSE
============================================================
This README controls how ChatGPT prepares customer-facing quotation text from BOQ/costing work.

Quotation is NOT the same as BOQ.

BOQ / takeoff / costing is internal.
Quotation is customer-facing.

The quotation must be clear enough for customer approval, but must not expose internal costing logic, MH, productivity, wastage, buffer, purchase strategy, supplier costing, or BOQ calculation notes.

============================================================
2) AUTHORITATIVE SOURCES
============================================================
Use these sources in this order:

1. User's latest confirmed instruction in the current job.
2. User-approved quotation price / revised price / final total.
3. Latest accepted BOQ / takeoff / costing numbers.
4. Uploaded quotation PDF if user asks to check issued quotation.
5. 1.2 Materials.txt and 1.3 Labour.txt for internal costing only.
6. README - BOQ.txt / BOQ workflow rules for takeoff and cost validation.

Do not use older GPT estimates if user has corrected or locked a newer price.

If uploaded quotation PDF conflicts with user instruction:
- Flag the conflict.
- Follow the latest user-approved instruction unless user asks to preserve the PDF exactly.

============================================================
3) STRICT SEPARATION BETWEEN BOQ AND QUOTATION
============================================================
BOQ may contain:
- material item names
- labour item names
- service/rental item names
- Usage Qty
- Wastage/Buffer
- MH productivity
- material rates
- labour rates
- service rates
- markup calculation
- supplier UOM
- purchase rounding
- formula logic
- takeoff notes

Quotation must NOT contain those internal details unless user specifically asks.

Customer quotation must only contain:
- clear work description
- location or affected area
- visible quantity and size where relevant
- included work scope
- reasonable exclusions or limitations where needed
- final selling price outside copy-code
- UOM outside copy-code

============================================================
4) MAIN OUTPUT RULE
============================================================
For normal customer quotation wording:

PRICE OUTSIDE COPY CODE.
UOM OUTSIDE COPY CODE.
DESCRIPTION INSIDE COPY CODE ONLY.

The copy-code block must contain customer-facing description only.

Do not put price inside the description copy-code.

Do not put UOM inside the description copy-code unless user specifically asks for table format.

============================================================
5) STANDARD CHAT OUTPUT FORMAT
============================================================
Use this format unless user instructs otherwise:

QUOTATION SXX

Kos: RMX,XXX.XX
Markup sesuai: XX%
Harga jual cadangan: RMX,XXX.XX
Harga bulat cadangan: RMX,XXX

UOM: 1 LOT
Harga: RMX,XXX

```text
Supply labour and material for <customer-facing scope description>.

- <included item 1>
- <included item 2>
- <included item 3>
```

Rules:
- Cost, markup, selling price and UOM are outside the copy-code.
- Description only is inside the copy-code.
- If user already locked final selling price, do not recalculate unless asked.
- If user only asks wording, do not include cost/markup unless useful or requested.

============================================================
6) FINAL QUOTATION CHECK FORMAT
============================================================
When user asks to check issued quotation PDFs, answer in this format:

Semakan quotation:

Quotation No / Scope:
- Value: RMX,XXX.XX
- Key wording present / missing
- Any spelling or scope issue

Total:
- S01 = RMX,XXX
- S02 = RMX,XXX
- S03 = RMX,XXX
- TOTAL = RMX,XXX

Decision:
- Betul / Salah
- If wrong, state exact correction.

Do not over-explain if the user asks "check betul tak".

============================================================
7) CUSTOMER-FACING DESCRIPTION RULES
============================================================
Quotation description must be written for the customer.

Use wording like:
- Supply labour and material for...
- Complete with...
- Including...
- To affected area...
- Existing item to be removed and reinstated where applicable...
- Debris clearing and disposal included...

Avoid internal wording like:
- MH
- productivity
- wastage
- buffer
- takeoff
- Usage Qty
- formula
- supplier UOM
- purchase qty
- cost price
- margin
- markup
- material uplift
- BOQ block
- Block 1 / Block 2 / Block 3
- SPEC A:C
- Materials.txt
- Labour.txt

============================================================
8) PRICE AND UOM RULE
============================================================
Price must be shown outside the copy-code.

Example:

S02: RM3,900
UOM: 1 LOT

```text id="fb352l"
Supply labour and material for waterproofing rectification, hacking, tile reinstatement, existing sanitary reinstatement and lower slab make-good works to 1 No existing bathroom not yet hacked.

- 1 No existing bathroom temporary remove and reinstall existing toilet
- 1 No upper-floor leak tracing, hacking and opening to affected floor and 300mm wall band
- 1 No concealed waterproofing system complete with primer, 2-coat waterproofing and full-area fiberglass mesh to affected floor and 300mm wall upturn
- 1 No curing, drying and water ponding / floor test
- 1 No floor screed / fall correction and tile reinstatement to floor and 300mm wall band only
- 1 Lot lower slab scrape / skim / sealer / repaint make-good to affected underside leak zone
- 1 Lot debris clearing, removal and disposal
```

Do not write:
"Price RM3,900 included..." inside the copy-code.

============================================================
9) VISIBLE ITEM RULE
============================================================
If an item is visible to the customer, do not hide it as vague lump sum.

Visible items must show quantity and size where available.

Good examples:
- 1 No x 30in x 84in Bathroom Door
- 3 Nos x 1200mm x 600mm Top Hung Window
- 1 Lot Car Porch 22ft x 20ft
- 2 Nos existing bathrooms
- 1 No additional separate bathroom wall area repair
- 1 Lot small laundry area

Bad examples:
- 1 Lot door works
- 1 Lot window works
- repair works
- complete works
- as discussed

Use "1 Lot" only when the work is genuinely a combined service/package and not a visible countable product.

============================================================
10) BRAND AND MATERIAL DISCLOSURE RULE
============================================================
Do not put brand names in customer quotation unless:
- user asks to show brand
- brand is a selling point
- supplier/system warranty requires it
- customer needs to approve exact brand/system

For internal BOQ, use exact master list names.
For quotation, use customer-facing scope wording.

Example:
Internal:
Pentens T-100 Water-Based PU Bituminous Waterproofing Membrane 20kg

Customer-facing:
concealed waterproofing system complete with primer, 2-coat waterproofing and fiberglass mesh reinforcement

============================================================
11) WATERPROOFING QUOTATION RULE
============================================================
For bathroom/wet-area waterproofing quotation, customer wording may include:
- surface preparation
- leak tracing / rectification
- primer
- waterproof coating
- fiberglass mesh reinforcement
- curing / drying
- ponding test
- protective screed / fall correction
- tile reinstatement
- grout / final finish
- sanitary reinstatement where relevant
- lower slab make-good where relevant
- debris clearing and disposal

Do not expose:
- kg/m2 rate
- number of pails
- mesh roll quantity
- media sand quantity
- MH
- wastage
- supplier package quantity

============================================================
12) HACKING / ALREADY HACKED RULE
============================================================
If area is already hacked/opened, quotation must not say hacking is included unless additional hacking remains.

Correct:
2 Nos existing bathrooms already opened for leak-rectification works

Wrong:
2 Nos bathroom hacking works

If only S02 requires hacking, do not copy S02 wording into S01.

S01 and S02 must remain distinct if their site condition differs.

============================================================
13) LOWER SLAB REPAIR RULE
============================================================
If leakage affects underside/lower slab, customer quotation must include lower slab make-good if user has stated it.

Use wording:
- 1 Lot lower slab scrape / skim / sealer / repaint make-good to affected underside leak zone

For multiple zones:
- 1 Lot lower slab scrape / skim / sealer / repaint make-good to affected underside leak zones

Do not omit lower slab repair if user already mentioned it.

============================================================
14) ADDITIONAL WORK INSIDE EXISTING QUOTATION
============================================================
If customer asks to reduce total but add extra small work into one quotation line, revise the description clearly.

Example:
- 1 No additional separate bathroom wall area repair complete with waterproofing rectification and 1ft x 2ft tile reinstatement to affected area

If it is a separate room, say "separate bathroom" or "separate room".

Do not leave it vague as:
- additional wall repair
- extra repair
- tile repair

============================================================
15) FINAL TOTAL / DISCOUNT RULE
============================================================
When customer asks to reduce total package price:
- keep scope wording clear
- revise per-quotation price if needed
- show total calculation
- ensure final total equals agreed total exactly

Example:

S01 = RM6,500
S02 = RM3,900
S03 = RM3,500

TOTAL = RM13,900

If numbers do not add up exactly, stop and correct before saying "betul".

============================================================
16) MARKUP RULE
============================================================
Markup is internal.

Use markup only for discussion with user, not inside customer description.

When user asks "berapa markup sesuai", answer outside copy-code.

Suggested markup must consider:
- rectification risk
- comeback risk
- waterproofing risk
- small-job mobilization
- labour uncertainty
- material purchase rounding
- disposal
- warranty exposure
- site difficulty
- customer discount pressure

Do not underprice rectification work as if it is simple new work.

============================================================
17) COST VS SELLING PRICE RULE
============================================================
Cost is not quotation price.

Cost may include:
- material cost
- labour cost
- service/rental/disposal
- subcontractor labour
- transport
- hidden risk allowance
- material uplift if locked
- wastage/buffer if locked

Selling price must include profit and risk.

If user asks for "cost", answer cost.
If user asks for "harga jual", answer selling price.
If user asks for "upah tukang luar", answer labour/subcontract cost only.

Do not answer a labour-only question with full project cost.

============================================================
18) SUBCONTRACTOR / TUKANG LUAR RULE
============================================================
If user asks "upah tukang luar", answer labour/subcontract price only.

Do not include:
- material
- RORO
- company margin
- supplier purchase
- markup

Unless user asks for all-in subcontractor package.

State clearly:
- labour only
- material excluded
- RORO excluded
- tools/comeback included or excluded if known

============================================================
19) SMALL JOB PURCHASE ROUNDING RULE
============================================================
For internal cost:
- calculate raw usage first
- add wastage/buffer
- then round up to supplier UOM

Do not:
- round raw usage first
- then add wastage
because that double-counts.

For customer quotation:
- never show raw decimal material quantity.
- never show supplier purchase quantity unless user asks for supplier order list.

============================================================
20) FULL UNIT PURCHASE RULE
============================================================
For supplier order list:
- use full supplier UOM
- no impossible decimal purchase quantities for items sold by pail, bag, roll, pack, tin, pcs, set

Example:
Wrong:
Pentens T-007 Primer 20kg - 0.1268 PAIL

Correct:
Pentens T-007 Primer 20kg - 1 PAIL

For BOQ usage sheet:
- decimal usage may exist if workbook requires usage logic.
For purchase list:
- full supplier unit only.

============================================================
21) QUOTATION DESCRIPTION MUST NOT USE BOQ NOTES
============================================================
Do not paste BOQ note lines directly into quotation.

Bad:
DEFAULT USED: primer basis 0.20kg/m2 over treated area; 20kg pail

Good:
concealed waterproofing system complete with primer and 2-coat waterproofing to affected area

BOQ notes are for calculation.
Quotation text is for customer.

============================================================
22) SCOPE-SPECIFIC QUOTATION HEADING RULE
============================================================
Each quotation scope should start with a clear heading or first sentence:

Supply labour and material for <work description>.

Examples:
- Supply labour and material for waterproofing rectification, tile reinstatement, sanitary reinstatement and lower slab make-good works to 2 Nos existing bathrooms already hacked/opened.
- Supply labour and material for waterproofing rectification, hacking, tile reinstatement, existing sanitary reinstatement and lower slab make-good works to 1 No existing bathroom not yet hacked.
- Supply labour and material for waterproofing rectification, hacking, tile reinstatement and lower slab make-good works to 1 Lot small laundry area.
- Supply labour and material for vinyl flooring installation complete with skirting.
- Supply labour and material for aluminium and glass sliding door with upper fixed panel works.

============================================================
23) CUSTOMER WORDING STYLE
============================================================
Use professional and direct wording.

Avoid:
- maybe
- roughly
- if needed
- depend
- probably
- should be
- I think
- internal assumption wording

Use:
- including
- complete with
- to affected area
- existing item to be reinstated
- final site measurement subject to verification
only if that condition is truly needed.

Do not overpromise.
Do not hide exclusions that can cause dispute.

============================================================
24) QUOTATION REVISION RULE
============================================================
If rewriting a quotation:
- write the full revised wording again
- do not give partial patches unless user asks for edit-only
- do not say "add this line" when user asks "tulis semula"
- do not leave the user to assemble fragments

If user says "tulis semula", output the full revised block.

============================================================
25) MULTIPLE QUOTATION PDF CHECK RULE
============================================================
If user uploads old and new quotation PDFs together:
- identify old vs revised version
- use latest revised numbers
- check total
- check key wording
- flag typo if any
- do not treat old price as current

If there are duplicate quote numbers with different prices:
- flag both
- state which one should be used based on latest user-approved price.

============================================================
26) SPELLING / CUSTOMER NAME CHECK RULE
============================================================
When checking final quotation PDF:
- check amount
- check total
- check scope wording
- check customer/project spelling
- check deliver-to spelling
- check obvious typo

If typo does not affect price, still flag it.

Example:
"Urban Inn Salak Tinggii" has extra "i".

============================================================
27) ACCEPTED TOTAL CHECK RULE
============================================================
When user says customer accepted a total and wants revision:
- do not change total
- rebalance line prices only if needed
- make sure total exactly equals accepted total
- do not add unapproved extra price

Example:
Customer requests total RM13,900.
Final must equal RM13,900 exactly.

============================================================
28) PACKAGE PRICING RULE
============================================================
If multiple quotations are part of one accepted package, price can be balanced across scopes.

However:
- each scope wording must still match actual work
- do not hide a bigger scope inside a smaller description
- if one quotation includes an added extra area, write it clearly
- final total must match agreed package total

============================================================
29) S01 / S02 / S03 NAMING RULE
============================================================
Use S01, S02, S03 when the user is working from BOQ scopes.

Do not mix descriptions between scopes.

Example:
S01 = bathrooms already hacked/opened
S02 = bathroom not yet hacked
S03 = laundry area
S04 = larger laundry/full room if user has separated it

If user corrects scope identity, rewrite the correct SXX only.

============================================================
30) QUOTATION AND BOQ SEQUENCE
============================================================
Normal workflow:
1. Build or confirm BOQ cost.
2. Confirm scope.
3. Confirm selling price.
4. Draft customer-facing quotation description.
5. Check total.
6. Check issued quotation PDF if uploaded.

Do not write customer quotation before understanding the actual scope.

Do not continue to next SXX if the current SXX is still wrong.

============================================================
31) COPY-CODE RULE
============================================================
Use copy-code only for text the user may paste.

Do not put commentary inside copy-code.

Do not put "Kos", "Markup", "Harga", or explanation inside copy-code unless user asks for a full quotation table.

For description copy-code, use plain text.

Example:

```text id="scf2co"
Supply labour and material for waterproofing rectification, tile reinstatement, sanitary reinstatement and lower slab make-good works to 2 Nos existing bathrooms already hacked/opened.

- 2 Nos existing bathrooms already opened for leak-rectification works
- 2 Nos upper-floor leak tracing and rectification to opened wet-area zones
- 2 Nos concealed waterproofing system complete with primer, 2-coat waterproofing and full-area fiberglass mesh to affected floor and 300mm wall upturn
- 2 Nos curing, drying and water ponding / floor test
- 2 Nos floor screed / fall correction and tile reinstatement to floor and 300mm wall band only
- 2 Nos existing toilet bowls reinstall back to usable condition
- 1 No damaged 4in waste fitting replacement
- 1 No additional separate bathroom wall area repair complete with waterproofing rectification and 1ft x 2ft tile reinstatement to affected area
- 1 Lot lower slab scrape / skim / sealer / repaint make-good to affected underside leak zones
- 1 Lot debris clearing, removal and disposal
```

============================================================
32) TABLE QUOTATION RULE
============================================================
If user asks for a table quotation, use table only when suitable.

Standard customer table may use:
No
Description
Qty
UOM
Unit Price (RM)
Amount (RM)

But for normal user workflow, use description copy-code with price outside copy-code.

Do not force table format if user asks for "prompt copy code".

============================================================
33) QUOTATION HEADER FOR DISCUSSION
============================================================
When user asks for markup suggestion, use this header style outside copy-code:

QUOTATION S01

Kos: RMX,XXX.XX
Markup sesuai: XX%
Harga jual cadangan: RMX,XXX.XX
Harga bulat cadangan: RMX,XXX

Then put customer-facing description in copy-code.

If user has already decided the price:
Harga revise: RMX,XXX

Do not reargue the markup unless asked.

============================================================
34) CUSTOMER-FACING EXCLUSION RULE
============================================================
Only include exclusions if they prevent future dispute.

Examples:
- Excluding concealed pipe replacement unless separately instructed.
- Excluding electrical works unless separately instructed.
- Excluding full-height wall tile if only 300mm wall band is included.
- Excluding new sanitary ware if existing sanitary is to be reused.

Do not add exclusions that scare the customer if not needed.

============================================================
35) REUSE ITEM RULE
============================================================
If electrical or sanitary items are reuse only, do not turn them into chargeable quotation items.

Use wording:
- existing item to be removed and reinstalled
- existing item to be reused
- minor disconnect/reinstall only

Do not list reuse items as new supply unless user confirms.

============================================================
36) FULL-HEIGHT TILE VS PARTIAL TILE RULE
============================================================
If user confirms floor tile and 300mm wall band only:
- do not describe full-height tile
- do not price as full-height tile
- do not imply wall tiling beyond affected 300mm band

Use:
floor and 300mm wall band only

============================================================
37) WATERPROOFING METHOD STATEMENT RULE
============================================================
If user asks for method statement, separate it from quotation.

Method statement may include:
1. Surface preparation
2. Primer
3. First coat
4. Mesh
5. Second coat
6. Sand splash / broadcast sand
7. Cure
8. Ponding test
9. Screed
10. Tiles / finish

But customer quotation should summarize only unless detailed method is required.

============================================================
38) PONDING / CURING WORDING RULE
============================================================
For customer quotation, use:
- curing, drying and water ponding / floor test

Do not put exact technical timing unless user wants:
- 8 hours
- 12 hours
- 24 hours
- 5 days
- 7 days

For site instruction, timing can be stated separately.

============================================================
39) MATERIAL ORDER LIST RULE
============================================================
If user asks "barang kena beli", output supplier purchase list.

For supplier purchase list:
- use exact item names where available
- use full supplier UOM
- no decimal purchase qty
- include only items needed
- separate confirmed quantity and optional additional quantity if needed

Example:
For 4 bathrooms confirmed:
Pentens T-007 Primer 20kg - 1 PAIL
Pentens T-100 Water-Based PU Bituminous Waterproofing Membrane 20kg - 3 PAIL
Pentens ACW-015 High Performance Fiberglass Mesh 1m x 100m - 1 ROLL
Silica Sand Filter Media Fine 0.6mm - 1.2mm 25kg Bag - 1 BAG
Cement 50kg Bag - 4 BAG
Fine Sand 20kg/Bag - 28 BAG
Sika Tile Adhesive 88 25kg - 8 BAG
Weber Weberfill Fine Grout Coloured Grout For Narrow Tile Joint (3.5kg) - 3 BAG
Tile 300mm x 600mm - 176 PCS
PVC Tile Spacer 2mm - 3 PACK

============================================================
40) SUPPLIER ORDER VS CUSTOMER QUOTATION RULE
============================================================
Supplier order list is not customer quotation.

Do not send supplier order list to customer unless user specifically asks.

Customer does not need to see:
- how many pails
- how many bags
- how many rolls
- how many kg
- purchase rounding
- leftover material
- wastage logic

============================================================
41) INTERNAL NOTE HANDLING
============================================================
Internal notes must stay outside customer quotation.

Internal examples:
- S01 already hacked
- S02 still requires hacking
- lower slab must be included
- tile only floor + 300mm wall band
- mesh full area
- T-100 selected by supplier
- 3 pail T-100 enough for 5 same-size bathrooms
- 1 scoop sand likely over
- media sand actual use small but purchase 1 bag

These may guide the quotation but must not appear as internal notes.

============================================================
42) EXACTNESS RULE WHEN USER ASKS "CHECK BETUL TAK"
============================================================
When user asks "check betul tak":
- check actual numbers
- check scope line
- check final total
- answer directly

Do not introduce new unrelated assumptions.

If correct:
Betul.

If wrong:
Salah pada <exact item>. Betulkan kepada <exact correction>.

============================================================
43) DO NOT REPEAT ALREADY SETTLED ISSUES
============================================================
If user has already locked a decision, do not ask again or reopen it.

Examples:
- mesh full area if user locked full area
- T-100 instead of T-100 Pro if supplier/user locked T-100
- price RM13,900 if customer accepted total
- S01 already hacked if user confirmed
- lower slab repair included if user already said so

If later evidence conflicts, flag conflict once.

============================================================
44) DO NOT GIVE PARTIAL PATCH WHEN FULL REWRITE IS ASKED
============================================================
If user says:
- tulis semula
- bagi penuh
- full
- jangan suruh tambah
- jangan bagi sekerat

Then output the full revised text.

Do not answer with:
- tambah line ini
- edit bahagian ini
- replace this bullet only

============================================================
45) LANGUAGE STYLE
============================================================
Discussion may be in Malay.
Quotation description may be in English if user uses English quotation system.
Keep wording professional, direct, and copy-ready.

Do not use casual insults, jokes, emojis, or unnecessary explanation inside quotation output.

============================================================
46) COMMON CUSTOMER QUOTATION WORDING BLOCKS
============================================================

Bathroom already hacked/opened:

Supply labour and material for waterproofing rectification, tile reinstatement, sanitary reinstatement and lower slab make-good works to 2 Nos existing bathrooms already hacked/opened.

- 2 Nos existing bathrooms already opened for leak-rectification works
- 2 Nos upper-floor leak tracing and rectification to opened wet-area zones
- 2 Nos concealed waterproofing system complete with primer, 2-coat waterproofing and full-area fiberglass mesh to affected floor and 300mm wall upturn
- 2 Nos curing, drying and water ponding / floor test
- 2 Nos floor screed / fall correction and tile reinstatement to floor and 300mm wall band only
- 2 Nos existing toilet bowls reinstall back to usable condition
- 1 No damaged 4in waste fitting replacement
- 1 No additional separate bathroom wall area repair complete with waterproofing rectification and 1ft x 2ft tile reinstatement to affected area
- 1 Lot lower slab scrape / skim / sealer / repaint make-good to affected underside leak zones
- 1 Lot debris clearing, removal and disposal

Bathroom not yet hacked:

Supply labour and material for waterproofing rectification, hacking, tile reinstatement, existing sanitary reinstatement and lower slab make-good works to 1 No existing bathroom not yet hacked.

- 1 No existing bathroom temporary remove and reinstall existing toilet
- 1 No upper-floor leak tracing, hacking and opening to affected floor and 300mm wall band
- 1 No concealed waterproofing system complete with primer, 2-coat waterproofing and full-area fiberglass mesh to affected floor and 300mm wall upturn
- 1 No curing, drying and water ponding / floor test
- 1 No floor screed / fall correction and tile reinstatement to floor and 300mm wall band only
- 1 Lot lower slab scrape / skim / sealer / repaint make-good to affected underside leak zone
- 1 Lot debris clearing, removal and disposal

Laundry small area:

Supply labour and material for waterproofing rectification, hacking, tile reinstatement and lower slab make-good works to 1 Lot small laundry area.

- 1 Lot upper-floor leak tracing, hacking and opening to affected laundry floor and 300mm wall band
- 1 Lot concealed waterproofing system complete with primer, 2-coat waterproofing and full-area fiberglass mesh to affected floor and 300mm wall upturn
- 1 Lot curing, drying and water ponding / floor test
- 1 Lot floor screed / fall correction and tile reinstatement to floor and 300mm wall band only
- 1 Lot lower slab scrape / skim / sealer / repaint make-good to affected underside leak zone
- 1 Lot debris clearing, removal and disposal

============================================================
47) FINAL DECISION WORDING
============================================================
Use:
- Betul.
- Salah.
- Boleh guna.
- Jangan guna versi lama.
- Total betul.
- Total salah.
- Harga dan wording betul.
- Ada typo sahaja.
- Perlu revise wording.
- Perlu revise price.

Avoid long defensive explanation unless user asks why.

============================================================
48) END OF README
============================================================
This README controls customer-facing quotation output only.

For BOQ/takeoff/building-cost workflow, follow README - BOQ.txt.
For supplier material list, follow 1.2 Materials.txt.
For labour/service/rental list, follow 1.3 Labour.txt.
For customer quotation wording, follow this README - QUOTATION.
