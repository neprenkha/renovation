# README BOQ Block Compliance Audit V1

## Audit question

Owner asked whether the current estimate already includes Block 1, Block 2 and Block 3 according to `README - BOQ.txt`.

## Result

No. `ActiveBOQ_Full_Estimate_V1.tsv` is a provisional quotation / summary estimate, not a full README-BOQ workbook block output.

It priced S01-S12 at scope-summary level, but it did not yet convert every priced SXX into the required three BOQ input blocks.

## README - BOQ requirement

According to `README - BOQ.txt`, after SPEC A:C is final, every priced SXX must output exactly three TSV blocks:

1. Block 1 / Materials, paste to `SXX!E:K`.
2. Block 2 / Labour, paste to `SXX!P:V`.
3. Block 3 / Service, paste to `SXX!AA:AG`.

Each block must use these input columns only:

`Note | Spec | Description | UOM | Usage Qty | Wastage/Buffer | Price/Unit or Rate (RM)`

The README also says not to output Total columns into block 1-3 paste blocks.

## Current files status

| File | Status |
|---|---|
| `Customer_Request_SPEC_V2.tsv` | SPEC stage exists but needs V3 repair to become fully takeoff-ready for all S01-S12. |
| `ActiveBOQ_Full_Estimate_V1.tsv` | Quotation summary / provisional pricing only. Not README block 1-3. |
| `Customer_Quotation_Draft_V2.md` | Customer-facing budget draft only. Not README block 1-3. |

## Why current estimate is not enough for workbook BOQ

`ActiveBOQ_Full_Estimate_V1.tsv` includes amount and total rows. README block paste output must not include Total columns or summary total rows.

The current estimate also combines several internal material/labour/service elements into one scope line, for example cabinet, plaster ceiling and feature wall rates. That is acceptable for customer rough budget, but not yet correct for workbook BOQ block 1-3.

## Required correction

Next proper step is to create upgraded files:

1. `Customer_Request_SPEC_V3.tsv` - repaired SPEC A:C with all S01-S12 takeoff logic locked.
2. `ActiveBOQ_Block_1_Materials_V1.tsv` - materials blocks for each priced SXX.
3. `ActiveBOQ_Block_2_Labour_V1.tsv` - labour blocks for each priced SXX.
4. `ActiveBOQ_Block_3_Service_V1.tsv` - service blocks for each priced SXX.
5. `ActiveBOQ_README_BOQ_Output_V1.md` - paste target headers for each SXX block.

## Working decision

The current RM39,000 figure can still be used as customer provisional quotation range.

But it must not be called a completed README-BOQ workbook output until block 1-3 files are produced and each SXX has its materials, labour and service rows separated according to README.
