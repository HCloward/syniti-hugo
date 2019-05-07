+++
title = 'Correct Errors in Target Data with Fixed Remediation Rules'
solution = 'Migration'
+++

# Correct Errors in Target Data with Fixed Remediation Rules

Transform offers a quick and simple way to correct the data in one field
for multiple records using a fixed remediation rule.

A fixed remediation rule can be used in situations where only one field
in the Target data requires remediation to quickly correct the data in
that one field for all the records. Fixed remediation rules can correct
instances where a required field in the Target system has been left
blank in the source data, or has been formatted incorrectly to be loaded
into the Target system. During report processing, a Fixed Remediation
rule can replace the values in a specified field with a specified value
for any records present in a Target report.

If multiple fields require remediation, fixed remediation cannot be
used, and a remediation rule must be added for each field. Refer to
[Register Target Remediation
Rules](Register_Target_Remediation_Rules.htm) for more information.

**NOTE:** When generating reports, Transform automatically replaces the
invalid characters ?|: \*” \<\>. The default replacement value is ^. The
default value can be set in the Replacement Char field on the Transform
tab on the *Parameters* page in Console.

**NOTE:** A fixed remediation rule cannot be saved with a
<span id="Status" class="popUpLink">status</span> of Active for a report
that cannot be updated, such as a report based on a view that has been
grouped by a column. To create a fixed remediation rule for a report
that is not updateable, set the status to Development.

**NOTE:** The number of remediation rules set for a Target can affect
the severity of score card limits. Refer to [Configure Score Card
Limits](../Config/Configure_Score_Card_Limits.htm) for more information.

**NOTE:** If a Target report uses a Fixed Remediation rule, every record
in the Target report is remediated with the value provided.

To create a fixed remediation rule in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the **Reports** icon for a Target.

3.  Click the **Vertical View** icon for a report.

4.  Click the **Remediation Information** tab on the *Target Reports*
    page's *Vertical* View.

5.  Click **Edit**.
    
    *[View the field descriptions for the Target Report’s Vertical View
    Remediation Information
    tab.](../Page_Desc/Target_Reports_H.htm#Remediation_Information)*

6.  Select an option from the
    **<span id="Status" class="popUpLink">Remediation Status</span>**
    list box.
    
    **NOTE:** If the report cannot be updated, such as a report grouped
    by a column name, select **Development**.

7.  Select a field name from the **Remediate Field** list box.
    
    **NOTE:** This field contains a value that should be updated by the
    fixed remediation rule. This list box displays all of the fields
    available on the report.

8.  Enter a value in the **Remediate Value** field.
    
    **NOTE:** This value will replace the value in the Remediate Field
    for all records in the Target report.

9.  Enter text in the **Remediation Comment** field to document notes
    about the fixed remediation rule.

10. Click **Save**.

11. Navigate to the *Target Reports* page's *Horizontal* View.

12. Click the **Execute** icon for the Target report.
    
    **NOTE:**The remediation rule runs along with the report.

Refer to [View Remediation Rule
Information](View_Remediation_Rule_Information.htm) for more
information.
