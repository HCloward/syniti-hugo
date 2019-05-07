+++
title = 'Register Target Data Services Remediation Rules'
solution = 'Migration'
+++

# Register Target Data Services Remediation Rules

Data Services Target Remediation allows a remediation rule to be
registered to an error report. Remediation rules are used only when
there is a need to temporarily fix a data issue so the affected records
can be loaded into a test environment.

Once Transform has processed Target data, it generates error reports.
Based on these reports, a user may create remediation rules to correct
erroneous values so that the data can be loaded successfully into the
Target system using a load tool.

Using Target Report Caching, Transform maintains the error reports so
that there is a record of the data changed by the remediation rule. This
feature, which runs when one or more Remediation events are active for
the Target report, caches all records from a Target report prior to the
execution of remediation rules.

Remediation rules can be used for complicated actions such as inserting
records into parent tables in a report and other indirect remediation
techniques.

Remediation rules:

  - Are always written based on the data in error reports
  - Must have a Where Clause
  - Must use the same Where Clause as the error report

**NOTE:** For the Data Services options and pages to be available, the
Data Service Repository must be registered in Common. The Data Services
check box must be checked in Console for the Process Area: Object. Refer
to [Register a Data Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
and  [Create the Context by Adding a Wave and Creating
Elements](../../Console/Use_Cases/Add_a_Wave_and_Create_Elements.htm)
for more information.

If Data Services remediation rules exist for a Target, the Data Services
Remediation icon on the Targets page is active and displays a record
count.

A Data Services remediation rule consists of a view, a stored procedure,
and a table stored in the database.

A user can add a Data Services remediation rule to a Target error
report, but the rule must already exist in the database.

**NOTE:** Click the Data Services Remediations icon on the *Targets*
page to see all remediation rules on all the selected Target’s reports.
Click the Data Services Remediations icon on the Target *Data Services
Reports* page to see all remediation rules for the selected Target
report. If the Data Services Remediations icon is disabled, no
remediation rules exist.

Before creating a Data Services remediation rule, ensure that a
Transform parameter is set in Console:

1.  Select **Advanced Configuration \> Parameters** in the *Navigation*
    pane.
2.  Click the **Transform** tab on the
    *[Parameters](../../Console/Page_Desc/Parameters.htm)* page.
3.  Click the **Run Remediation Rules** check box to enable it.

To register a remediation rule to a Target report in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the **Data Services Reports** icon for a Target.
    
    **NOTE:** This icon displays if a Data Services repository has been
    set at the object level. Refer to [Configure Data Services
    Functionality](../../Console/Config/Configure_Data_Services_Functionality.htm)
    for more information.

3.  Click the **Vertical View** icon for a report.

4.  Click the **Remediation Information** tab on the *[Target Data
    Services Reports](../Page_Desc/Target_Data_Services_Reports_H.htm)*
    page's *Vertical* view.

5.  Click the **Remediation** icon.

6.  Click **Add**.
    
    *[View the field descriptions for the Target Data Services
    Remediation page](../Page_Desc/Target_DS_Remediation_H.htm).*

7.  Enter a sort value in the **PRIORITY** field.
    
    **NOTE:** If multiple remediation rules are registered to the Target
    report, the priority determines the order the rule is run.

8.  Select a value from the
    **<span id="Status" class="popUpLink">STATUS</span>** list box.

9.  Select a view from the **TARGET DATA SERVICES REPORT REMEDIATION
    RULE VIEW** list box.

10. Select a type from the **RULE TYPE** list box. Options are:
    
      - **Delete –** Delete only rules.
      - **Insert –** Insert only rules.
      - **Manual –** All rules.
      - **Move –**Move only rules.
      - **Update –** Update only rules.

11. Select a rule from the **TARGET DATA SERVICES REPORT REMEDIATION
    RULE** list box.

12. Enter a Target remediation rule description in the **DESCRIPTION**
    field.

13. Click **Save**; the *Vertical* View displays.

14. Click the **Documentation** tab.

15. Enter additional text in the **Comment** field to document any notes
    about the Target remediation rule (optional).

16. Click **Save**.

Target remediation rules can be run in the foreground or background.

<span style="font-weight: bold;">NOTE:</span> If a process takes less
than 0.5 seconds to run, the duration in the DURATION field is 0.

Run a rule in the background if there is a large amount of data to
process that may affect system performance or may time out a session.
Monitor rules that run in the background on the *Monitor* page.

A rule that runs in the foreground processes immediately.

To run a Target Data Services remediation rule in the background in
Transform:

1.  Click the **Process Information** tab on the *Vertical* View of the
    *Target Data Services Reports* page.
2.  Click the **Process** icon; a confirmation message displays.
3.  Click **OK**.

To run a Target Data Services remediation rule in the foreground in
Transform:

1.  Navigate to *Horizontal* View of the *Target Data Services Reports*
    page.
2.  Click the **Execute** icon in the Page toolbar; a confirmation
    message displays.
3.  Click **OK**.

Refer to [View Data Services Remediation Rule
Information](View_DS_Remediation_Rule_Information.htm) for more
information.
