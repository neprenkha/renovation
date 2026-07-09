# GPT Header Renovation Addendum — SXX Reference Rule

This file records a permanent/general renovation workflow rule that must be merged into the next full replacement of:

```text
GPTEditable/GPT Header Renovation.md
GPT Header Renovation.md
GPTRenovationHeader.txt
```

## Rule

Root master/reference files remain read-only unless owner explicitly asks to edit that exact file:

```text
README - BOQ.txt
1.2 Materials.txt
1.3 Labour.txt
```

If a BOQ/SXX item is missing from root master lists, work must not stop.

GPT must create or update approved editable supplemental reference files under:

```text
GPTEditable/Reference_Addendum/
```

Approved files:

```text
GPTEditable/Reference_Addendum/README_REFERENCE_ADDENDUM.md
GPTEditable/Reference_Addendum/1.2_AdditionalMaterials_OnlineReference.txt
GPTEditable/Reference_Addendum/1.3_AdditionalLabourServices_OnlineReference.txt
```

Addendum files must use root-master style tab-delimited schema where applicable:

```text
No	Category	Subcategory	Description	Qty	UOM	Price/Unit (RM)	Total (RM)	Update Date	Supplier	Note
```

Every rate must record update date, supplier/source and status. If online search does not produce a reliable exact source, GPT may use a logical provisional rate only when it is clearly marked as provisional and not presented as final customer selling price.

SXX BOQ output intended for Excel/XLS must be `.txt` tab-delimited and copy-paste ready in this order:

```text
SPEC A:C
Block 1 material/product/consumable
Block 2 labour/plant/rental
Block 3 subcontract/specialist/service
summary/status/gate
```

## Reason

Owner corrected that S01 must not stop only because `1.2 Materials.txt` or `1.3 Labour.txt` lacks a required item. Missing items should become editable reference addendum entries, while root master files remain read-only.
