# ActiveBOQ Workflow Checklist

## Purpose

This folder is the active customer-pricing workspace for the current extension and renovation job.

Use this folder to solve the current customer request: read the supplied floor plan/drawing, identify the renovation or extension scope, calculate price using the repository references, and prepare a customer-facing quotation.

The root repository remains the reference source:

- `GPT Header Renovation.md`
- `SingleStoreyExtentionNRenovationV5.md`
- `DoubleStoreyExtentionNRenovationV5.md`
- `V5_CUSTOMER_ANSWER.md`
- `V5_CHANGE_REPORT.md`
- `1.2 Materials.txt`
- `1.3 Labour.txt`
- `README - BOQ.txt`
- `README - QUOTATION.txt`

## ActiveBOQ evidence to check

Before pricing, confirm whether this folder contains:

| Check | Required detail | Status |
|---|---|---|
| 1 | Customer/project name or job label | To check from ActiveBOQ files |
| 2 | Floor plan/drawing supplied by customer | To check from ActiveBOQ files |
| 3 | Work area marked or described | To check from ActiveBOQ files |
| 4 | Single-storey/double-storey status | To check from ActiveBOQ files |
| 5 | Measurements or usable scale | To check from ActiveBOQ files |
| 6 | Extension/renovation scope | To check from ActiveBOQ files |
| 7 | Package tier or finish expectation | To check from ActiveBOQ files |
| 8 | Add-ons such as toilet, wet kitchen, laundry, M&E, aluminium/glass, cabinet or structure | To check from ActiveBOQ files |
| 9 | Site risk notes or assumptions | To check from ActiveBOQ files |
| 10 | Required quotation output format | To check from ActiveBOQ files |

If a detail is not available, mark it as `MISSING` and ask only for that exact missing detail.

## Pricing source order

Use this order:

1. ActiveBOQ customer floor plan/drawing and owner instructions.
2. Latest catalog version V5 for public guide prices and package scope.
3. `V5_CUSTOMER_ANSWER.md` for how to explain inclusions to customer.
4. `1.2 Materials.txt` for material reference.
5. `1.3 Labour.txt` for labour and installation reference.
6. README BOQ/quotation files for output discipline.

## Quotation output structure

Every customer quotation draft should include:

1. Customer/project label.
2. Work area.
3. Drawing/floor plan reference used.
4. Measurement basis.
5. Package/tier used.
6. Scope included.
7. Add-ons included.
8. Exclusions.
9. Assumptions.
10. Site questions before final confirmation.
11. Price range or quotation amount.
12. Catalog/reference version used.

## Safety rule

Do not overwrite root catalog versions from this folder.

Do not invent dimensions from a unclear drawing.

Do not promise brand/model unless the final quotation lists it.

Do not publish internal costing, profit, raw labour or supplier names to the customer quotation unless the owner explicitly asks for internal BOQ/costing output.
