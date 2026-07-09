# GPT Header Renovation Addendum — One-Pass SXX Preflight Rule

This file records a permanent/general renovation workflow rule that must be merged into the next full replacement of:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt
```

## Rule: complete each SXX once with preflight before writing output

Before creating any SXX audit/takeoff file or BOQ.xlsm paste-ready file, GPT must perform a preflight check in the same turn:

1. read the latest SXX tracker;
2. confirm the active SXX and previous SXX gate;
3. read the relevant drawing/source list for that SXX;
4. read `README - BOQ.txt` format rules;
5. read matching material/labour/root/addendum references;
6. check cross-SXX overlap/double-count risks;
7. only then create the audit/takeoff file, BOQ.xlsm paste-ready file and tracker update.

## Rule: do not repeat the S02 pattern

GPT must not create a SXX as complete, then hold it, then close it again with no quantity/rate change unless the owner explicitly changes the decision.

Separate statuses must remain clear:

```text
WORKING-COST BASIS
BOQ.XLSM PASTE READY
CUSTOMER SELLING PRICE
CORRECTION REQUIRED BY LATER CONTRADICTION
```

When the owner directs that a SXX must be completed now, GPT must complete the current working-cost basis and keep the later contradiction rule active instead of leaving the SXX hanging.

## Correction reason

Owner corrected the S02 workflow because GPT created repeated S02 versions and status changes. Future SXX outputs must be prepared with a stricter preflight so each SXX can be completed in one pass wherever possible.
