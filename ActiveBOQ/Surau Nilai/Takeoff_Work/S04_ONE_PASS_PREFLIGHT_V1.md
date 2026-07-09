# Surau Nilai — S04 One-Pass Preflight V1

## Objective

Prepare S04 once, fully and cleanly, without repeating the S02 open/hold/close pattern.

## Active sequence confirmed

Latest tracker before S04:

```text
ActiveBOQ/Surau Nilai/BOQ/09_SXX_COSTING_TRACKER_V9.md
```

Gate from V9:

```text
CURRENT ACTIVE SXX: S04
S03 COMPLETE FOR NEXT SXX: YES - 100% MUKTAMAD WORKING-COST BASIS
S03 BOQ.XLSM PASTE FILE: READY
S04 START ALLOWED: YES
```

## S04 scope

```text
S04 = Crossing bridge and permanent site entrance
```

## S04 source drawings / source files

Primary S04 drawing from deep-read register and tracker:

```text
ActiveBOQ/Surau Nilai/Drawing/CROSSING BRIDGE.pdf
```

Supporting source as needed:

```text
ActiveBOQ/Surau Nilai/Drawing/Surau Site Plan Tender_Constn.pdf
ActiveBOQ/Surau Nilai/Drawing/Survey Tapak Surau Juassewh Sentosa.pdf
```

GitHub source check:

```text
CROSSING BRIDGE.pdf exists in GitHub with blob SHA fc6723eb5dd6b70c697cc69a3577a4a3946ba00c.
```

## Root/reference checked

```text
README - BOQ.txt
1.2 Materials.txt
1.3 Labour.txt
GPTEditable/Reference_Addendum/
```

Relevant material/root rates:

```text
Ready Mix Concrete G25 (Per m3) - M3 - RM365.00
Crusher Run (10-Wheel Truck) - TRIP - RM850.00 selected by duplicate highest-rate rule
Reinforcement Steel Bar Supply Allowance (Current Working Cost Per kg) - KG - RM3.80 addendum
Formwork Plywood Timber and Release Oil Material Allowance (Current Working Cost Per m2) - M2 - RM35.00 addendum
```

Relevant labour/plant root rates:

```text
Labour - Skilled Worker (Per MH) - MH - RM22.50
Labour - General Helper (Per MH) - MH - RM16.25
Backhoe Hire - Standard (Per Day) - DAY - RM750.00
```

## Cross-SXX checks

S04 must not duplicate:

```text
S01 mobilisation / hoarding / signboard / site setup
S02 ESCP silt fence / sandbag / temporary ESCP controls
S03 general earthwork / platform formation / imported fill allowance
S05 building substructure footing / ground beam
S07 slab and apron works
S22 permanent drainage
S24 road base / premix / parking works
```

## Final current S04 basis

Owner requires SXX to be completed now and not left hanging.

Current S04 working-cost basis is locked as:

```text
Ready Mix Concrete G25: 3.20 m3 + 5% wastage
Reinforcement steel: 320 kg + 5% wastage
Formwork material: 22 m2 + 10% wastage
Crusher Run: 1 trip
Skilled worker: 48 MH
General helper: 32 MH
Backhoe hire: 1 day
```

This is the muktamad working-cost basis for S04 sequence. Later contradiction, drawing refinement or supplier quote must create a correction version before affected summary/customer total is used.

## Completion target

Create:

```text
ActiveBOQ/Surau Nilai/BOQ/S04_CrossingBridge_Entrance_Takeoff_Audit_V1.txt
ActiveBOQ/Surau Nilai/BOQ/S04_BOQXLSM_PASTE_READY_V1.txt
ActiveBOQ/Surau Nilai/BOQ/10_SXX_COSTING_TRACKER_V10.md
```
