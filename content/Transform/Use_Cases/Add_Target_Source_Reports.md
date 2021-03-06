+++
title = 'Add Target Source Reports'
solution = 'Migration'
+++

# Add Target Source Reports

A Target Source Report is a report run against the Source table. These
reports are typically used to display data relevant to processing the
rules.

**NOTE:** BackOffice follows a strict naming convention for creating
names that each member of the object can understand. Any manually
created objects must also follow these conventions. Refer to [Naming
Conventions](Naming_Conventions.htm) for more information.

**NOTE:** Target Source reports must be manually created as a view in
SQL.

<span style="font-weight: bold;">NOTE:</span> Transform writes report
files to the path defined in the Report Path field on the Transform tab
of the <span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">[Parameters](../../Console/Page_Desc/Parameters.htm)</span>
page in Console. All files are generated to the path:
C:\\DSW\\Report\\\<Wave Name\>-\<Process Area\>\\\<Target Name\>.  

To register a Target Source report to a Target Source in Transform:

1.  Select the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the
    <span class="StyleListNumberBold" style="font-weight: bold;">Sources</span>
    icon for a Target.

3.  Click the
    <span class="StyleListNumberBold" style="font-weight: bold;">Reports</span>
    icon for a Target Source.

4.  Click **Add**.
    
    *[View the field descriptions for the Target Source Reports
    page.](../Page_Desc/Target_Source_Reports_H.htm)*

5.  Enter a sort value in the
    <span class="StyleListNumberBold" style="font-weight: bold;">PRIORITY</span>
    field.
    
    <span style="font-weight: bold;">NOTE:</span> If multiple Target
    Source reports exist for the Target Source, the Priority determines
    the order the rules are run.

6.  Select a value from the
    <span class="StyleListNumberBold" style="font-weight: bold;"><span id="Status" class="popUpLink">STATUS</span></span>
    list box.

7.  Select a type from the
    <span id="Report Type" class="popUpLink">REPORT TYPE</span> list
    box.

8.  Select a report from the
    <span class="StyleListNumberBold" style="font-weight: bold;">SOURCE
    REPORT</span> list box.
    
    **NOTE:** This is the view manually created in SQL.

9.  Enter a brief Source report description in the
    <span class="StyleListNumberBold" style="font-weight: bold;">DESCRIPTION</span>
    field.

10. Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>;
    the *Vertical* View displays.

11. Select a field from the
    <span class="StyleListNumberBold" style="font-weight: bold;">Segment
    By Field</span> list box.
    
    **NOTE:Segment By Field** displays a list of all fields in the
    report. Selecting a field causes Transform to create a separate
    report and sub-directory for each value in this field.

12. Click the **Documentation** tab.

13. Enter text in the
    <span class="StyleListNumberBold" style="font-weight: bold;">Comment</span>
    field to document any notes about the Source report.

14. Click the **Process Information** tab.

15. Select a method from the
    <span class="StyleListNumberBold" style="font-weight: bold;">Sample
    Method</span> list box, if applicable.
    
    **NOTE:** The Sample Method provides a selection of random rows to
    verify the data. It can be configured by selecting Configuration \>
    Setup \> Sampling Methods (Setup).

16. Select a format from the
    <span class="StyleListNumberBold" style="font-weight: bold;">Report
    Format</span> list box to determine if translated columns (from
    SAP's German abbreviation), field names or both translated columns
    and field names are used in column headings. SAP fields are German
    abbreviations.

17. Enter a value in **Report Order By** field to sort the result set in
    the report.

18. Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>.

Target Source reports can be run in the foreground or background.

**NOTE:** If a process takes less than 0.5 seconds to run, the duration
in the DURATION field is 0.

Run a report in the background if there is a large amount of data to
process that may affect system performance or may time out a session.
Monitor reports that run in the background on the Monitor page.

A report that runs in the foreground processes immediately.

To run a Target Source report in the background in Transform:

1.  Click the **Process Information** tab on the Target Source Report's
    *Vertical* View.
2.  Click the **Process** icon;a confirmation message displays.
3.  Click **OK**.

To run a Target Source report in the foreground in Transform:

1.  Navigate to the Target Source Report's *Horizontal* View.
2.  Click the **Execute** icon in the Page toolbar; a confirmation
    message displays.
3.  Click **OK**.
