# S08 Allowance Authority Correction V3

Generated MYT: 2026-07-10 05:40

## Correction

Owner corrected the S08 strict gate decision:

```text
If customer/drawing/README/owner gives an allowance or accepted working basis, use that allowance.
The requirement is not to use the minimum quantity.
Use the customer/authority-derived allowance so excess risk is already costed.
Do not treat an authorised allowance as a failure merely because it is called allowance.
```

## README basis

`README - BOQ.txt` is an authoritative source for the BOQ workflow. It states that the README/tracker workflow, Materials list and Labour list are authoritative sources. It also states that standalone/full purchase/full allowance/already-rounded purchase quantities can be entered as the final full quantity with Wastage/Buffer = 0.

For S08, this means the following can be closed as final cost basis when clearly recorded:

```text
- RF beam length basis from rendered RF roof beam drawing and roof layout.
- IRB beam length basis from rendered internal roof beam drawing and roof layout.
- Column count/height basis from rendered layout/column schedule and adopted working height.
- Rebar BBS working quantity where the internal calculation is deliberately set as a full cost allowance, not a minimum.
- Scaffold bay and jack/U-head allowance where the allowance covers the S08 column/roof beam work period and is recorded as the final full usage quantity.
- Pump/access allowance where a fixed lot allowance is used as the final cost basis for the current BOQ stage.
```

## Updated interpretation

The earlier S08 strict review V2 was too strict because it treated every `allowance`, `basis`, or `can refine` phrase as an automatic 100% failure.

That interpretation is now superseded.

Correct rule for this project:

```text
Authorised allowance / customer-given allowance / README-compliant full allowance = can be final cost basis.
Random unsupported allowance = cannot be final cost basis.
```

## Required wording cleanup

S08 V2 must remove hanging/tentative wording from the workbook paste file and audit gate. It must record the allowance as:

```text
CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS - CLOSED FOR CURRENT BOQ COST
```

not as:

```text
supplier verification item
may refine later
exact design can refine
```

## Gate decision

```text
S08 V1 strict hold is superseded.
Create S08 V2 audit and paste-ready files with final allowance basis.
Then open S09.
```
