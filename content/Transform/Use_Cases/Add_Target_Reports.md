+++
title = 'Add Target Reports'
solution = 'Migration'
+++

# Add Target Reports

A Target report is a view built in SQL and stored in the Target table.

**NOTE:** For each Target used in Map, Map can generate a Rulebook
report, which contains all the mappings created for the Target. The
Rulebook report can be accessed in Map by selecting ProcessArea \>
Metrics \> Rule Book.

**NOTE:** BackOffice follows a strict naming convention for creating
names that each member of the object can understand. Any manually
created objects must also follow these conventions. Refer to [Naming
Conventions](Naming_Conventions.htm) for more information.

**NOTE:** Reports can also be built automatically using SQL AutoGen.
Refer to [Build Reports](../../SQL_AutoGen/Use_Cases/Build_Reports.htm)
for more information.

<span style="font-weight: bold;">NOTE:</span> Transform writes report
files to the path defined in the Report Path field on the Transform tab
of the Vertical View of the Parameters page in Console. All files are
generated to the path: C:\\DSW\\Report\\\<Wave Name\>-\<Process
Area\>\\\<Target Name\>.  

To add a Target report in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the
    <span class="StyleListNumberBold" style="font-weight: bold;">Reports</span>
    icon for a Target.

3.  Click <span style="font-weight: bold;">Add</span>.
    
    *[View the field descriptions for the Target Reports
    page](../Page_Desc/Target_Reports_H.htm)*

4.  Enter a value in the
    <span class="StyleListNumberBold" style="font-weight: bold;">PRIORITY</span>
    field.
    
    **NOTE:** If multiple reports are registered to the Target, the
    priority determines the order the report is processed.

5.  Select a value from the
    <span class="StyleListNumberBold" style="font-weight: bold;"><span id="Status" class="popUpLink">STATUS</span></span>
    list box.

6.  Select a type from the
    <span class="StyleListNumberBold" style="font-weight: bold;"><span id="Report Type" class="popUpLink">REPORT
    TYPE</span></span> list box.

7.  Select a report from the
    <span class="StyleListNumberBold" style="font-weight: bold;">TARGET
    REPORT</span> list box.
    
    **NOTE:** This report is a view that must already exist in the
    database.

8.  Enter a Target report description in the
    <span class="StyleListNumberBold" style="font-weight: bold;">DESCRIPTION</span>
    field.

9.  Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>;
    the *Vertical* View displays.

10. Select a field from the
    <span class="StyleListNumberBold" style="font-weight: bold;">Segment
    By Field</span> list box.
    
    **NOTE:**Segment By Field displays a list of all fields in the
    report. Selecting a field causes Transform to create a separate
    report and a sub-directory for each value in this field.

11. Click the **Documentation** tab.

12. Enter a justification for the report in the
    <span class="StyleListNumberBold" style="font-weight: bold;">Specification
    Section</span> field.

13. Enter text in the
    <span class="StyleListNumberBold" style="font-weight: bold;">Comment</span>
    field to document any notes about the Target report.

14. Click the **Process Information** tab.

15. Select a method from
    <span class="StyleListNumberBold" style="font-weight: bold;">Sample
    Method</span> list box, if applicable.
    
    **NOTE:** The Sample Method provides a selection of random rows to
    verify the data. It can be configured by selecting Configuration \>
    Setup \> Sampling Methods (Setup) in the *Navigation* pane.

16. Select a format from the
    <span class="StyleListNumberBold" style="font-weight: bold;">Report
    Format</span> list box to determine if translated columns (for
    example, if column headings are German abbreviations as in SAP),
    field names or both translated columns and field names are used in
    column headings.

17. Enter a value in the **Report Order By** field to sort the result
    set in the report.

18. Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>.

Target reports can be run in the foreground or background.

**NOTE:** If a process takes less than 0.5 seconds to run, the duration
in the DURATION field is 0.

Run a report in the background if there is a large amount of data to
process that may affect system performance or may time out a session.
Monitor reports that run in the background on the *Monitor* page.

A report that runs in the foreground processes immediately.

To run a Target report in the background in Transform:

1.  Click the **Process Information** tab on the *Vertical* View of the
    *Target Reports* page.
2.  Click the **Process** icon; a confirmation message displays.
3.  Click **OK**.

To run a Target report in the foreground in Transform:

1.  Navigate to the *Horizontal* View of the *Target Reports* page.
2.  Click the **Execute** icon on the Page toolbar in the child pane; a
    confirmation message displays.
3.  Click **OK**.
