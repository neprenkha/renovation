# File Relocation Plan — +60 13-731 9262 - fahrurrazy fr

## Purpose

Loose files currently stored directly under `ActiveBOQ/` should not remain mixed with other projects. This client/site should use its own workspace:

```text
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/
```

## Target folders

```text
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/GPT_CONTROL/
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/Takeoff_Work/
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/BOQ/
ActiveBOQ/+60 13-731 9262 - fahrurrazy fr/BOQ_work/
```

## Known loose ActiveBOQ root files from repository history

### Proposed target: `BOQ/`

```text
ActiveBOQ/ActiveBOQ_Full_Estimate_V3.tsv
ActiveBOQ/ActiveBOQ_Full_Estimate_V4.md
ActiveBOQ/ActiveBOQ_Full_Estimate_V5.md
ActiveBOQ/ActiveBOQ_Full_Estimate_V6.md
ActiveBOQ/ActiveBOQ_Full_Estimate_V7.md
ActiveBOQ/Customer_10_Item_Cost_Breakdown_V1.md
ActiveBOQ/Customer_10_Item_Size_Rate_Breakdown_V2.md
ActiveBOQ/Customer_Estimate_Answer_V2.md
ActiveBOQ/Customer_Estimate_Answer_V3.md
ActiveBOQ/Customer_Estimate_Answer_V4.md
ActiveBOQ/Customer_Estimate_Answer_V5.md
ActiveBOQ/Customer_Estimate_Answer_V6.md
ActiveBOQ/Customer_Estimate_Answer_V7.md
ActiveBOQ/Customer_Quotation_Draft_V5.md
ActiveBOQ/Customer_Quotation_Draft_V6.md
ActiveBOQ/Customer_Quotation_Draft_V7.md
```

### Proposed target: `Takeoff_Work/`

```text
ActiveBOQ/Ceiling_Dimension_Correction_V1.md
ActiveBOQ/Dimension_Correction_V3.md
ActiveBOQ/Painting_Building_Area_Correction_V2.md
ActiveBOQ/Painting_Dimension_Correction_V1.md
ActiveBOQ/Painting_Product_Material_Check_V1.md
```

## Relocation rule

Move only loose files directly under `ActiveBOQ/` that belong to this client/site. Do not move:

```text
ActiveBOQ/Surau Nilai/
```

or any file/folder inside another project folder.

## Status

Workspace folders and control files are created. Actual file relocation should be done only against a confirmed file list so unrelated project files are not moved by mistake.
