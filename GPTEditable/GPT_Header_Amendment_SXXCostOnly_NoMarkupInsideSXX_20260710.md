# GPT Header Amendment - SXX Cost-Only Chain / No Markup Inside SXX

Generated MYT: 2026-07-10 20:37

Repository: neprenkha/renovation

Applies to:
- GPTEditable/GPT Header Renovation.md
- GPT Header Renovation.md
- GPTRenovationHeader.txt owner local full replacement

## Owner correction captured

Owner clarified that for this BOQ workflow, S01-SXX is for construction cost takeoff only. Markup, gross margin, commercial selling price, and final quotation pricing are not part of the SXX takeoff sequence unless owner explicitly opens a separate pricing workflow.

The previous tracker wording that treated S20 as markup/final customer price path was a workflow classification error. S20/S21 must not be used to force markup into the BOQ cost SXX chain.

## Permanent rule to merge as Section 13H

13H) SXX COST-ONLY CHAIN / NO MARKUP INSIDE SXX RULE

For Surau Nilai and any BOQ workflow using S01-SXX, the SXX sequence is a construction cost/takeoff chain unless owner explicitly says otherwise.

S01-SXX must be used to calculate and audit measured or logically allowed construction quantities, material cost, labour/plant/rental cost, subcontract/specialist/service cost, wastage, buffer, optional contingency, duplicate prevention, missing component/rate checks, and current BOQ cost basis.

S01-SXX must not be used by default to calculate profit, markup, gross margin, final customer selling price, commercial negotiation margin, or quotation selling policy.

Markup, gross margin and customer selling price must be handled outside the SXX takeoff sequence as a separate commercial/pricing output only when owner explicitly asks for that stage.

Do not create or classify a next SXX only because markup or final customer price has not been calculated. Missing markup does not make the construction cost takeoff incomplete when owner has defined the current target as BOQ cost only.

If all known drawing/spec/customer construction cost scopes have been covered and no new material/labour/service component remains, the SXX cost chain should be marked cost-complete / no further cost SXX, not forced into a markup SXX.

A next SXX may be opened only when there is a real remaining cost/takeoff scope, reserved owner-defined cost item, drawing/spec update, correction, or another owner-requested cost package.

If a previous tracker opened S20/S21 as markup/customer-price SXX by mistake, GPT must correct the tracker with a new cumulative version and state clearly that SXX cost chain is complete up to the last valid cost/consolidation SXX, markup/customer selling price is outside SXX, S21 is not applicable unless owner introduces a new cost scope, and no next SXX is allowed just for markup.

## Immediate execution rule

Until the full canonical header merge is completed safely, GPT must still obey this amendment as active governance for Surau Nilai and all future SXX costing.
