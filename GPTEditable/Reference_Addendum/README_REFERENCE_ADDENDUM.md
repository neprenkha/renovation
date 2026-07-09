# Renovation Reference Addendum

This folder stores approved editable supplemental reference files for `neprenkha/renovation`.

Root files remain read-only unless owner explicitly asks to edit that exact file:

```text
README - BOQ.txt
1.2 Materials.txt
1.3 Labour.txt
```

If a BOQ/SXX item is missing from root master files, work must not stop. GPT must create/update reference addendum files here and mark the rate/source status clearly.

## Approved files

```text
GPTEditable/Reference_Addendum/1.2_AdditionalMaterials_OnlineReference.txt
GPTEditable/Reference_Addendum/1.3_AdditionalLabourServices_OnlineReference.txt
```

## Required tab-delimited schema

Use the same column style as root master lists:

```text
No	Category	Subcategory	Description	Qty	UOM	Price/Unit (RM)	Total (RM)	Update Date	Supplier	Note
```

## Rate status rules

Use clear notes:

- `ROOT MASTER MATCH` = already exists in root master list;
- `ONLINE SOURCE` = supported by online/public source;
- `PROVISIONAL ONLINE / MARKET SURVEY` = online search performed but exact local item/source is not reliable enough for final quotation;
- `LOGICAL PROVISIONAL RATE` = owner permits continuity and item is needed for SXX progression;
- `SUPPLIER QUOTE NEEDED` = final quote still required.

## Use in SXX costing

SXX costing may use these addendum descriptions when the root master files do not contain the required item.

Every SXX line using this folder must keep the price status visible and must not pretend that provisional references are final customer selling rates.
