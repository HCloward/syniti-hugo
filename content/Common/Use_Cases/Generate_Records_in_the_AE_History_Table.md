# Generate Records in the AE History Table

The **AE Insert History** check box is a troubleshooting tool for any
user that encounters issues with AE processing. Users will be able to
review the AE history processing with the flag turned on. A
pre-requisite to inserting into the History table is ensuring that there
are Targets in Target Design. Refer to [Add a
Target](../../../Migration/Design/Use_Cases/Add_a_Target_in_Target_Design.htm)
for more information.

Refer to [Add Fields to Tables](Add_Fields_to_Tables.htm)  to add fields
to the System Type table.

To generate records in the History table and add an index to the History
table:

1.  Select <span style="font-weight: bold;">Automation Engine \>
    Automation Engine Params</span> from the *Navigation* pane.
    
    **NOTE:** The AE Insert History must not be enabled. In the event
    that it is, click **Edit** and uncheck the box.

2.  Delete all records in ttAutomationEngineHistory in DSPCommon
    database.

3.  Navigate to **Target Design** and click **DESIGN FINISH** for a
    Target.

4.  Recheck that the table ttAutomationEngineHistory is empty in
    DSPCommon database.

5.  Select **Automation Engine \> Automation Engine Params** from the
    *Navigation* pane.

6.  Select the **AE Insert History** check box to enable it.

7.  Navigate to **Target Design** and change the Design Status to DESIGN
    FINISHED for a target. Refer to [Set the Design
    Status](../../../Migration/Design/Use_Cases/Set_the_Design_Status.htm)
    for more information.

8.  Ensure that entries have been added to ttAutomationEngineHistory in
    DSPCommon Database by getting a count.

9.  Navigate to **Automation Engine \> Automation Engine Params**.

10. Click **AE Insert History** to disable it.
