# Add Target Data Services Reports

<span style="font-weight: bold;">NOTE:</span> Transform writes report
files to the path defined in the Report Path field on the Transform tab
of the <span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">Parameters</span> page in Console. All
files are generated to the path: C:\\DSW\\Report\\\<Wave
Name\>-\<Process Area\> - \<Object\>\\\<Target Name\>.

To add a Target Data Services report in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)*.

2.  Click the **Data Services Reports** icon for a Target.
    
    **NOTE:** The *Target Data Services Reports* page displays in Add
    Mode if no Target Data Services Reports have been built for the
    Target.

3.  Click **Add**.
    
    *[View the field descriptions for the Target Data Services Reports
    page](../Page_Desc/Target_Data_Services_Reports_H.htm)*

4.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** If multiple reports are registered to the Target, the
    priority determines the order the report is processed.

5.  Select a value from the
    **<span id="Status" class="popUpLink">STATUS</span>** list box.

6.  Select a type from the
    **<span id="Report Type" class="popUpLink">REPORT TYPE</span>** list
    box.

7.  Select a report from the **TARGET DATA SERVICES REPORT** list box.
    
    **NOTE:** This report is a view that must already exist in the
    database.

8.  Enter a Target report description in the **DESCRIPTION** field.

9.  Click **Save**; the *Vertical* View displays.
    
    [View the field descriptions for the Target Data Services Reports
    page’s Vertical
    View](../Page_Desc/Target_Data_Services_Reports_H.htm#Target_Data_Services_Reports_V).

10. Select a field from the **Segment By Field** list box.
    
    **NOTE:** Segment By Field displays a list of all fields in the
    report. Selecting a field causes Transform to create a separate
    report and a sub-directory for each value in this field.

11. Click the **Documentation** tab on the *Target Data Services
    Reports* page.

12. Enter a justification for the report in the **Specification
    Section** field.

13. Enter text in the **Comment** field to document any notes about the
    Target report (optional).

14. Click the **Process Information** tab on the *Target Data Services
    Reports* page.

15. Select a method from the **Sample Method** list box, if applicable.
    
    **NOTE:** The **Sample Method** provides a selection of random rows
    to verify the data. It can be configured by selecting Configuration
    \> Setup \> Sampling Methods (Setup) in the*Navigation* pane.

16. Select a format from the **Report Format** list box to determine if
    translated columns (for example, if column headings are German
    abbreviations as in SAP), field names or both translated columns and
    field names are used in column headings.

17. Enter a value in the **Report Order By** field to sort the result
    set in the report. 

18. Click **Save**.

Target reports can be run in the foreground or background.

<span style="font-weight: bold;">NOTE:</span> If a process takes less
than 0.5 seconds to run, the duration in the DURATION field is 0.

Run a report in the background if there is a large amount of data to
process that may affect system performance or may time out a session.
Monitor reports that run in the background on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page.

A report that runs in the foreground processes immediately.

To run a Target Data Services report in the background in Transform:

1.  Click the **Process Information** tab on the *Vertical* View of the
    *Target Data Services Reports* page.
2.  Click the **Process**icon; a confirmation message displays.
3.  Click **OK**.

To run a Target Data Services report in the foreground in Transform:

1.  Navigate to the *Horizontal* View of the *Target Data Services
    Reports* page.
2.  Click the **Execute** icon in the Page toolbar on the child pane; a
    confirmation message displays.
3.  Click **OK**.
