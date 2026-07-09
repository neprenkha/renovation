# GPT Header Amendment — Authorised Allowance + Mandatory Header Update Rule

Generated MYT: 2026-07-10 05:50

Repository:

```text
neprenkha/renovation
```

This file records a permanent governance correction that must be merged into:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt full owner-copy replacement when next produced
```

## Why this amendment exists

Owner corrected GPT after S08 because GPT wrongly treated all `allowance`, `basis`, `supplier/site verification`, `may refine`, `average`, or similar wording as automatic failure for 100% SXX completion.

That was too broad.

The correct rule is:

```text
Authorised allowance / customer-given allowance / drawing-derived allowance / README-compliant full allowance / owner-confirmed working basis can be a 100% current BOQ cost basis when it is recorded as final for the current BOQ stage.

Random unsupported allowance cannot be treated as 100% drawing/spec completion.
```

## Mandatory rule to add to Section 13D or a new Section 13E

When owner says `100%`, `siap sepenuhnya`, `ikut spec/drawing pelanggan`, or `99.9% means fail`, GPT must distinguish between:

```text
A) Unsupported/random allowance = FAIL / HOLD.
B) Authorised/customer/drawing/README/owner-confirmed allowance = CAN BE FINAL current BOQ cost basis.
```

An authorised allowance may be used when:

- it comes from customer instruction, drawing/spec note, README - BOQ.txt, owner-confirmed decision, or a clearly documented drawing-derived full allowance;
- the SPEC A:C explains that the allowance is intentionally adopted as the current BOQ cost basis;
- Block 1-3 use the full allowance quantity, not a minimum quantity;
- Wastage/Buffer follows README format, including `0` where the Usage Qty is already a full purchase/full allowance quantity;
- the row note says `CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS - CLOSED FOR CURRENT BOQ COST` or equivalent;
- the line has no hanging wording such as `may refine later` as the active final gate;
- undercost/overprice/double-count/markup checks are recorded.

## SXX proceeding rule after this correction

If a SXX uses authorised allowance correctly, GPT may mark:

```text
COMPLETE FOR NEXT SXX - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS
```

and proceed to the next SXX.

If a SXX uses unsupported/random allowance, GPT must mark:

```text
HOLD - DRAWING SPEC / AUTHORISED ALLOWANCE VERIFICATION REQUIRED
```

and must not proceed.

## Mandatory header-update-after-mistake rule

If GPT makes a governance-level mistake and then fixes only a tracker, addendum, or job file, that is still incomplete.

When the mistake proves the header did not prevent the failure, GPT must update the canonical header in the same session when GitHub is accessible:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTEditable/README_GPTEDITABLE.md if governance/header workflow is affected
GPTRenovationHeader.txt full owner-copy replacement when next produced or requested
```

Do not wait for the owner to ask again.

## S08 application

S08 V2 corrected the gate using the authorised allowance rule:

```text
ActiveBOQ/Surau Nilai/BOQ/S08_ALLOWANCE_AUTHORITY_CORRECTION_V3.md
ActiveBOQ/Surau Nilai/BOQ/S08_RCFrame_Columns_RoofBeams_Takeoff_Audit_V2.txt
ActiveBOQ/Surau Nilai/BOQ/S08_BOQXLSM_PASTE_READY_V2.txt
ActiveBOQ/Surau Nilai/BOQ/20_SXX_COSTING_TRACKER_V20.md
```

S08 V2 supersedes the overly strict S08 hold in:

```text
ActiveBOQ/Surau Nilai/BOQ/S08_STRICT_100_PERCENT_GATE_REVIEW_V2.md
ActiveBOQ/Surau Nilai/BOQ/19_SXX_COSTING_TRACKER_V19.md
```

## Status

```text
HEADER AMENDMENT CREATED
MAIN CANONICAL HEADER STILL MUST BE MERGED SAFELY WITHOUT SHORTENING OR OVERWRITING VALID OLD RULES
```