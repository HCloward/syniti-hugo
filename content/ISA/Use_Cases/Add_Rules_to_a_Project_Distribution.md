# Add Rules to a Project Distribution

Add rules to a Project Distribution to send failed records from the rule
to users who belong to the Project Distribution.

**NOTE**: If a rule has a rule status of Approved in IS, it is available
to be added to all projects. If the rule has any other status, it is
only available to be added to the project in which the rule was built.

<span style="font-weight: bold;">NOTE:</span> If a rule is bound to a
single table on multiple fields, each binding will generate a
spreadsheet to send as an attachment to users in the project
distribution. The spreadsheet will contain data that failed the rule for
each field-table combination.

To add a rule:

1.  Select <span style="font-weight: bold;">Information Steward
    Accelerator \> </span>**Configuration \> Project Summary** in the
    *Navigation* pane.

2.  Click the **Distributions** for a project.

3.  Click **Rules** for a Project Distribution.

4.  If no records exist, the page displays in add mode. Otherwise click
    <span style="font-weight: bold;">Add</span>.
    
    [View field descriptions for the Project Distributions Rules
    page.](../Page_Desc/Project_Distribution_Rules.htm)

5.  Select a rule name from the **RULEID** list box.
    
    **NOTE:** This list box contains all rules created for the project,
    regardless of the rule status in IS, and all rules in other projects
    that have a rule status of Approved in IS.

6.  Click <span style="font-weight: bold;">Save</span>.
    
    **NOTE:** The Quality Dimension added to the rule in IS displays in
    the **QUALITY DIMENSION** field.
