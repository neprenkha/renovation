# GPT Header Renovation Addendum — SXX Visual Scan Gate Rule

This file records a permanent/general renovation workflow rule that must be merged into the next full replacement of:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt
```

## Rule: PDF existence is not a drawing scan

Do not mark any SXX as 100% customer-spec complete merely because:

- the drawing filename exists;
- GitHub fetched the PDF/base64;
- the source path was listed;
- a default working-cost basis was created;
- a BOQ.xlsm paste-ready file was generated.

Customer-spec complete requires actual drawing/source scan. For PDFs, this means render/screenshot/visual inspection or a reliable extraction that proves the relevant notes, dimensions and symbols were checked.

## Rule: two completion states must be separated

Every SXX may have these separate states:

```text
WORKING-COST BASIS COMPLETE
BOQ.XLSM PASTE FILE READY
CUSTOMER-SPEC VISUAL SCAN COMPLETE
CUSTOMER SELLING PRICE COMPLETE
```

GPT must not collapse these into one word such as `complete`.

A SXX may be paste-ready for working-cost input but still held for customer-spec visual scan.

## Rule: if drawing cannot be rendered/read

If a relevant drawing cannot be rendered or read in the current tool/session:

- mark the SXX as `HOLD - VISUAL SCAN REQUIRED` or `UNREADABLE / NEEDS REVIEW`;
- do not start the next SXX as if the current one is 100% complete;
- create a rescan gate note under the active job `Takeoff_Work/` folder;
- update the SXX tracker before continuing.

## Reason

Owner corrected S02 because it was marked complete too quickly even though `SJ_01ESCP-LP-01-S0-00.pdf` had not been visually scanned/rendered. Future SXX work must not repeat this mistake.
