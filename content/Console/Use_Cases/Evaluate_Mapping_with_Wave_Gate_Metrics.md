+++
title = 'Evaluate Mapping with Wave Gate Metrics'
solution = 'Migration'
+++

# Evaluate Mapping with Wave Gate Metrics

There are two types of gate metrics for Map:

  - [Value mapping](#Gate), which is set up at the Wave level in Console

  - [Field mapping](#Gate2) which is set up at the Wave-process level in
    Console

A gate, with a gate date and a percentage complete, which allows a user
to evaluate current mapping status against a customizable goal. Use the
Snap Shot process in Map to get current mapping statistics to measure
against the Gate Wave metrics.

**NOTE:** The process for setting up Wave Gate metrics for value mapping
and field mapping is the same. Wave Gate metrics for value mapping are
set up on the *[Wave Gate Metrics (Value
Mapping)](../Page_Desc/Wave_Gate_Metrics_Value_Mapping_H.htm)* page.
Wave Gate metrics for field mapping are set up on the *[Wave Gate
Metrics (Field
Mapping)](../../Map/Page_Desc/Wave_Proc_Area_Gate_Metrics_Field_Mapping.htm)*
page.

The process for using Wave Gate metrics is:

1.  Enter the **GATE NAME**, the **GATE DATE** and the **GATE
    PERCENTAGE** for value mapping and field mapping in Console.
2.  Run the Snap Shot process in Map to gather current mapping status.
    The Snap Shot process captures mapping metrics at a specific point
    in time. Refer to [Capture Statistics for Wave Gate
    Metrics](../../Map/Use_Cases/Capture_Statistics_for_Wave_Gate_Metrics.htm)
    for more information.
3.  View the current mapping status in relation to the gate metrics on
    the *Wave Gate Metrics (Value Mapping)* page and the *Wave Gate
    Metrics (Field Mapping)* page. View details for a gate by clicking
    **Vertical View** for the gate on the *Wave Gate Metrics (Value
    Mapping)* page or the *Wave Gate Metrics (Field Mapping)* page.

**NOTE:** These pages can be viewed in Map by clicking **Metrics** on
the *[Process Area
Launch](../../Transform/Page_Desc/Process_Area_Launch.htm)* page. Click
the **Gate Value Metrics** icon or the **Gate Field Metrics** icon.
These pages open as display only when accessed in Map. Wave Gate metrics
can only be edited in Console.

## <span id="Gate"></span>Gate Metrics for Value Mapping

To set up Gate metrics for value mapping in Console:

1.  Click **Waves** icon on the *Navigation* pane.

2.  Click the **Metrics** icon for a Wave.

3.  Click **Add**.
    
    *[View the field descriptions for the Wave Gate Metrics (Value
    Mapping) page](../Page_Desc/Wave_Gate_Metrics_Value_Mapping_H.htm)*

4.  Enter a name in the **GATE NAME** field.

5.  Enter a date or click the calendar to select a date in the **GATE
    DATE** field.

6.  Enter a value in the **GATE PERCENTAGE** field.

7.  **NOTE**: This percent should be complete for value mapping by the
    date entered in the **GATE DATE** field.

8.  Click **Save.**

**NOTE:** A service page runs daily to update the gate percentage. A
user can also run the Snap Shot process in Map to update the current
mapping statistics visible on the *Wave Gate Metrics (Value Mapping)*
page’s *Horizontal* View with details provided on the *Vertical* View.
The LAST UPDATE DATE field is updated with the date the service page
ran, or the last date the Snap Shot process was run.

**NOTE:** If the current date is later than the date in the **GATE
DATE** field, the statistics on the page will not update.

## <span id="Gate2"></span>Gate Metrics for Field Mapping

To set up Gate metrics for field mapping in Console:

1.  Click **Waves** on the *Navigation* pane.

2.  Click the **Process Areas** icon for a Wave.

3.  Click the **Metrics** icon for a Process Area.

4.  Click **Add**
    
    [View the field descriptions for the Wave Process Area Gate Metrics
    (Field Mapping)
    page](../../Map/Page_Desc/Wave_Proc_Area_Gate_Metrics_Field_Mapping.htm)

5.  Enter a name in the **GATE NAME** field.

6.  Enter a date or click the calendar to select a date in the **GATE
    DATE** field.
    
    **NOTE:** This is the date by which the percentage of the field
    mapping entered in the GATE PERCENTAGE field should be completed.

7.  Enter a value in the **GATE PERCENTAGE** field.
    
    **NOTE:** This percent should be complete for field mapping by the
    date entered in the GATE DATE field.

8.  Click **Save**.

**NOTE:** A service page runs daily to update the gate percentage. A
user can also run the Snap Shot process in Map to update the current
mapping statistics visible on the *Wave Process Area Gate Metrics (Field
Mapping)* page’s *Horizontal* View, with details provided on the
*Vertical* View. The LAST UPDATE DATE field is updated with the date the
service page ran or the last date the Snap Shot process was run.

**NOTE:** If the current date is later than the date in the GATE DATE
field, the statistics on the page will not update.
