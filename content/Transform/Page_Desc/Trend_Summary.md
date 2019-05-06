# Trend Summary

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

This report displays a set of icons that display tables, procedures,
views and error reports for each object where objects have been captured
on the *Milestones* page. Refer to [Create
Milestones](../Use_Cases/Create_Milestones.htm) for detailed information
on capturing objects.

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Select <span style="font-weight: bold;">Tracking \> Summary</span>
    in the <span style="font-style: italic;">Navigation</span>
pane.

|               |                                                                                                                                                                                                                               |
| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field         | Description                                                                                                                                                                                                                   |
| OBJECT        | Displays the object name as configured in Console.                                                                                                                                                                            |
| Tables        | Click to open the *[Trend Summary (Tables)](Trend_Summary_Tables.htm)* page,  which displays the tables associated with the object, captured when the most recent milestone was captured for the object.                      |
| Procedures    | Click to open the *[Trend Summary (Procedures)](Trend_Summary_Procedures.htm)*  page, which displays the stored procedures associated with the object, captured when the most recent milestone was captured for the object.   |
| Views         | Click to open the [*Trend Summary (Views)*](Trend_Summary_Views.htm)  page, which displays the views associated with the object, captured when the most recent milestone was captured for the object.                         |
| Error Reports | Click to open the *[Trend Summary (Error Reports)](Trend_Summary_Error_Reports.htm)*  page, which displays the error reports associated with the object, captured when the most recent milestone was captured for the object. |
