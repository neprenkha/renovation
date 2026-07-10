# Surau Nilai — SXX Costing Tracker V41

Supersedes:

```text
ActiveBOQ/Surau Nilai/BOQ/40_SXX_COSTING_TRACKER_V40.md
```

Active workspace:

```text
ActiveBOQ/Surau Nilai/
```

## V41 note — owner scope correction for tile supply and S11 inclusion

Owner corrected that:

```text
Tile supply should be counted in the BOQ working cost.
Door/window/glazing should be counted in the BOQ working cost.
S01-SXX remains cost-only; markup/customer selling price is outside SXX.
```

## Header/governance correction

New governance amendment created:

```text
GPTEditable/GPT_Header_Amendment_OwnerRequiredSupplyItemsIncluded_20260710.md
Commit: 85d5969c2905a7cbed5326957b8a5239cee23464
```

Active added rule:

```text
SXX OWNER-REQUIRED SUPPLY-INCLUDED RULE
```

## S12 V2 active files

```text
Rate reference:
ActiveBOQ/Surau Nilai/BOQ/S12_Finishes_Sanitary_RateReference_V2.txt

Audit/reference file:
ActiveBOQ/Surau Nilai/BOQ/S12_InternalFinishes_SanitaryFixtures_OwnerScopeCorrection_Takeoff_Audit_V2.txt

Owner workbook paste file:
ActiveBOQ/Surau Nilai/BOQ/S12_BOQXLSM_PASTE_READY_V2.txt
```

## S12 V2 correction decision

```text
S12 TILE SUPPLY PREVIOUSLY EXCLUDED: ERROR - SUPERSEDED
S12 V2 TILE SUPPLY: INCLUDED BY OWNER CORRECTION
S12 V2 CURRENT BOQ COST BASIS: PASS
S11 DOOR/WINDOW/GLAZING: INCLUDED IN S11 COST; FUTURE ACTUAL PRICE REPLACEMENT ONLY
```

## S12 V2 tile supply added

```text
PT porcelain floor tile supply: 100m2 x RM55.00/m2 = RM5,500.00
CT ceramic wall/floor tile supply: 175m2 x RM40.00/m2 = RM7,000.00
Total tile supply added: RM12,500.00
```

## S12 V2 corrected cost

```text
Block 1 material/product/consumable: RM44,490.35
Block 2 labour: RM34,520.05
Block 3 service: RM3,400.00
Base working cost: RM82,410.40
Optional 10% contingency: RM8,241.04
Working cost with optional contingency: RM90,651.44
Customer selling price / markup: OUTSIDE SXX
```

## S12 V2 delta

```text
S12 V1 base working cost: RM69,910.40
S12 V2 added tile supply: RM12,500.00
S12 V2 base working cost: RM82,410.40
Delta with optional 10% contingency: RM13,750.00
```

## S11 inclusion confirmation

S11 remains included in the BOQ cost chain. It already includes:

```text
D1 solid timber doors: 4 nos
D2 aluminium sliding doors: 3 nos
D3 solid timber doors: 3 nos
W1 aluminium top hung windows: 2 nos
W2 Breezeway Altair adjustable glass louvres: 5 nos
W3 Breezeway Altair adjustable glass louvres: 2 nos
S11 base working cost: RM54,771.60
```

Future actual supplier price may replace S11 rates later, but S11 is not zero and not excluded.

## Corrected current BOQ total after S12 V2

```text
Previous corrected base working cost: RM748,244.00
Add S12 V2 tile supply delta: RM12,500.00
Corrected base working cost after S12 V2: RM760,744.00
Optional 10% contingency: RM76,074.40
Corrected working cost with optional contingency: RM836,818.40
Customer selling price / markup: OUTSIDE SXX
```

## Correct active paste/summary chain after V41

```text
S01_BOQXLSM_PASTE_READY_V1.txt
S02_BOQXLSM_PASTE_READY_V2.txt
S03_BOQXLSM_PASTE_READY_V2.txt
S04_BOQXLSM_PASTE_READY_V2.txt
S05_BOQXLSM_PASTE_READY_V1.txt
S06_BOQXLSM_PASTE_READY_V2.txt
S07_BOQXLSM_PASTE_READY_V1.txt
S08_BOQXLSM_PASTE_READY_V2.txt
S09_BOQXLSM_PASTE_READY_V1.txt
S10_BOQXLSM_PASTE_READY_V1.txt
S11_BOQXLSM_PASTE_READY_V2.txt
S12_BOQXLSM_PASTE_READY_V2.txt
S13_BOQXLSM_PASTE_READY_V2.txt
S14_BOQXLSM_PASTE_READY_V1.txt
S15_BOQXLSM_PASTE_READY_V1.txt
S16_BOQXLSM_PASTE_READY_V1.txt
S17_BOQXLSM_PASTE_READY_OR_SUMMARY_V3.txt
S18_BOQXLSM_PASTE_READY_OR_SUMMARY_V1.txt
S19_BOQXLSM_PASTE_READY_OR_SUMMARY_V2.txt
S20_BOQXLSM_PASTE_READY_OR_SUMMARY_V2.txt
```

## V41 strict checklist

```text
Owner correction checked: PASS
S12 tile supply added: PASS
S12 tile supply rate basis documented as logical provisional: PASS
S12 tile consumables/labour retained: PASS
S12 sanitary fixture count retained: PASS
S11 door/window/glazing included: PASS
Future actual supplier price recorded as replacement only: PASS
No missing material/product/labour/service line after correction: PASS
No customer markup inserted into SXX: PASS
Overall cost total corrected: PASS
```

## Current gate

```text
CURRENT ACTIVE SXX: COST CHAIN CORRECTED THROUGH S12 V2 / S19 / S20 CORRECTION CHECKPOINT
S01 DRAWING/SPEC RESCAN: PASS FOR CURRENT BOQ COST BASIS - USE V1
S02 DRAWING/SPEC RESCAN: PASS FOR CURRENT BOQ COST BASIS - USE V2
S03 DRAWING/SPEC RESCAN: PASS AND COST REVISED - USE V2
S04 WORKING-COST DRAWING/SPEC BASIS: COMPLETE - USE V2
S05 WORKING-COST DRAWING/SPEC BASIS: COMPLETE - USE V1
S06 WORKING-COST DRAWING/SPEC BASIS: COMPLETE AFTER RECHECK - USE V2
S07 WORKING-COST DRAWING/SPEC BASIS: COMPLETE AFTER RECHECK - USE V1
S08 COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS - USE V2
S09 COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS - USE V1
S10 COMPLETE - CUSTOMER/README ACCEPTED FULL ALLOWANCE BASIS - USE V1
S11 STRICT 100% CURRENT BOQ COST BASIS: PASS - USE AUDIT V3 / PASTE V2
S12 OWNER SCOPE CORRECTION V2: PASS - TILE SUPPLY INCLUDED - USE V2
S13 WORKING-COST ESTIMATE COMPLETE - OWNER ACCEPTED PREMIUM-SENSIBLE SIZE-BASED PROVISIONAL PATH - USE V2
S14 STRICT 100% CURRENT BOQ COST BASIS: PASS - USE V1
S15 STRICT 100% CURRENT BOQ COST BASIS: PASS - USE V1
S16 STRICT 100% CURRENT BOQ COST BASIS: PASS - USE V1
S17 STRICT 100% RECHECK V3: PASS FOR CURRENT BOQ COST BASIS
S18 FINAL RESERVED SCOPE / PROJECT CLOSEOUT REVIEW: PASS FOR CURRENT BOQ COST BASIS
S19 13G STRICT 100% RECHECK V2: PASS FOR CURRENT BOQ COST BASIS
S20 SXX COST-ONLY CORRECTION / CLOSURE CHECKPOINT: PASS
S21 START ALLOWED: NO - NO ADDITIONAL CURRENT COST SCOPE AFTER THIS CORRECTION
CORRECTED BASE WORKING COST: RM760,744.00
CORRECTED WORKING COST WITH OPTIONAL 10% CONTINGENCY: RM836,818.40
CUSTOMER SELLING PRICE / MARKUP: OUTSIDE SXX
```
