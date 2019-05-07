+++
title = 'Trend Summary (Error Reports)'
solution = 'Migration'
+++

# Trend Summary (Error Reports)

<span style="font-weight: bold;">NOTE:</span> For data to display on the
Trend Summary reports (Tracking \> Summary) and the Summary Type charts
(Process Area Launch \> Change Summary), the following must happen:

  - Trace must be turned on for the tables, views, functions and
    procedure counts. Refer to [Activate and Deactivate Data
    Sources](../../../Platform/Common/Use_Cases/Activate_and_Deactivate_Data_Source.htm)
    for more information. For Transform, trace should be activated for
    the databases beginning with “dsw”.
  - A milestone must be captured. Refer to [Create
    Milestones](../Use_Cases/Create_Milestones.htm) for more
    information.

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Select <span style="font-weight: bold;">Tracking \> Summary</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
3.  Click the <span style="font-weight: bold;">Error Reports</span> icon
    for an
Object.

|             |                                                                                                       |
| ----------- | ----------------------------------------------------------------------------------------------------- |
| Field       | Description                                                                                           |
| OBJECT      | Displays the Object name created in Console to which the target and source are assigned.              |
| TARGET      | Displays the target table associated with the view, stored procedure or table assigned to the object. |
| SOURCE      | Displays the source table associated with the view, stored procedure or table assigned to the object. |
| OBJECT TYPE | Displays the number associated with the object type (in this case, error report).                     |
| OBJECT NAME | Displays the name of the view, stored procedure or table.                                             |
| STATUS      | Displays the <span id="Status" class="popUpLink">status</span>.                                       |
| COUNT01     | Displays the number of records processed for the object name on the corresponding action date.        |
| ACTIONON01  | Displays the date Transform processed the object.                                                     |
| COUNT02     | Displays the number of records processed for the object name on the corresponding action date.        |
| ACTIONON02  | Displays the date Transform processed the object.                                                     |
| COUNT03     | Displays the number of records processed for the object name on the corresponding action date.        |
| ACTIONON03  | Displays the date Transform processed the object.                                                     |
| COUNT04     | Displays the number of records processed for the object name on the corresponding action date.        |
| ACTIONON04  | Displays the date Transform processed the object.                                                     |
