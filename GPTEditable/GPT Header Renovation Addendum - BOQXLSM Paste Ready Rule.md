# GPT Header Renovation Addendum — BOQ.xlsm Paste Ready Rule

This file records a permanent/general renovation workflow rule that must be merged into the next full replacement of:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt
```

## Rule: audit/takeoff file is not owner paste file

GPT may create detailed audit/takeoff files with source, formula, raw quantity, deduction, net quantity, markup status and audit notes.

However, those audit files are not automatically safe for owner to copy into `*BOQ.xlsm`.

For any SXX where the owner needs to paste into `*BOQ.xlsm`, GPT must also provide a separate `BOQXLSM_PASTE_READY` `.txt` file or clearly separated copy blocks.

## Required paste targets

Use the exact target headers from `README - BOQ.txt`:

```text
Paste to SXX!A:C - SPEC
Paste to SXX!E:K - Materials Block
Paste to SXX!P:V - Labour Block
Paste to SXX!AA:AG - Service Block
```

The target header must be outside and immediately above the TSV block. It must not be inside the TSV data.

## Allowed TSV columns only

SPEC A:C:

```text
Spec	Description	Note
```

Block 1 E:K:

```text
Note	Spec	Description	UOM	Usage Qty	Wastage/Buffer	Price/Unit (RM)
```

Block 2 P:V:

```text
Note	Spec	Description	UOM	Usage Qty	Wastage/Buffer	Rate (RM)
```

Block 3 AA:AG:

```text
Note	Spec	Description	UOM	Usage Qty	Wastage/Buffer	Rate (RM)
```

## Prohibited inside BOQ.xlsm paste blocks

Do not include:

- Total columns;
- formula columns;
- source drawing columns;
- raw/deduction/net audit columns;
- GitHub status/finality columns;
- long audit tables;
- summary/status/gate rows inside E:K, P:V or AA:AG.

Summary/gate may be kept in GitHub notes/tracker, but not pasted into BOQ.xlsm input blocks unless the workbook has a specific target for it.

## Correction reason

Owner corrected that prior S01 V4 was arranged for GitHub audit and would cause trouble if copied into `*BOQ.xlsm`. Future SXX outputs must serve both needs separately: audit file for GitHub/review, and paste-ready file for the workbook.
