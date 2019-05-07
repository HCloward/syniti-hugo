+++
title = 'Add Target Source Rules'
solution = 'Migration'
+++

# Add Target Source Rules

A Target Source Rule (also referred to as a Source Rule) cleans and
massages the data before it is loaded in the Target table. The final
Target Source rule pushes the data into the Target table from the
source.

Each Target Source rule consists of a view and a stored procedure that
is created and stored in the source table.

**NOTE:** BackOffice follows a strict naming convention for creating
names that each member of the object can understand. Any manually
created objects must also follow these conventions. Refer to [Naming
Conventions](Naming_Conventions.htm) for more information.

**NOTE:** Rules can also be created automatically using SQL AutoGen.
Refer to [Create Rules](../../SQL_AutoGen/Use_Cases/Create_Rules.htm)
for more information.

To register a Target Source rule to a Target Source in Transform:

1.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](../Page_Desc/Process_Area_Launch.htm)*
    page.

2.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

3.  Click the
    <span class="StyleListNumberBold" style="font-weight: bold;">Rules</span>
    icon for a Target Source.
    
    **NOTE:** The *Target Source Rules* page displays in Add Mode if no
    Target Source rules have been built for the Target Source.
    
    **NOTE:** If the status is inactive for the source or the SOURCE
    DATABASE OBJECT is SrcTable, this icon is disabled.

4.  Click **Add**.
    
    *[View the field descriptions for the Target Source Rules
    page.](../Page_Desc/Target_Source_Rules_H.htm)*

5.  Enter a sort value in the
    <span style="font-weight: bold;">PRIORITY</span> field.
    
    **NOTE:** If multiple Target Source rules are registered to the
    Target Source, the Priority determines the order the rule is
    processed.

6.  Select a value from the
    <span class="StyleListNumberBold" style="font-weight: bold;"><span id="Status" class="popUpLink">STATUS</span></span>
    list box.

7.  Select a type from the **RULE TYPE** list box from these options:
    
      - **Delete –** Delete only rules.
      - **Insert –** Insert only rules.
      - **Manual –** All rules.
      - **Move –** Move only rules.
      - **Update –** Update only rules.

8.  Select a view from the **SOURCE RULE VIEW** list box.
    
    **NOTE:** This view was built and is stored in the source table.
    
    <span style="font-weight: bold;">NOTE:</span> Only views that use
    the proper naming convention display in the list box. Refer to
    [Naming Conventions](Naming_Conventions.htm) for more information.

9.  Select an option from the **SOURCE RULE** list box.
    
    **NOTE:** This stored procedure was built and is stored in the
    source table.
    
    <span style="font-weight: bold;">NOTE:</span> Only rules that use
    the proper naming convention display in the list box. Refer to
    [Naming Conventions](Naming_Conventions.htm) for more information.

10. Enter a brief Target Source rule description in the
    <span class="StyleListNumberBold" style="font-weight: bold;">DESCRIPTION</span>
    field.

11. Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>;
    the *Vertical* View displays.

12. Click the **Documentation** tab.
    
    *[View the field descriptions for the Target Source Rules page's
    Vertical
    View.](../Page_Desc/Target_Source_Rules_H.htm#Target_Source_Rules_V)*

13. Enter text in the
    <span class="StyleListNumberBold" style="font-weight: bold;">Comment</span>
    field to document any notes about the Target Source rule.

14. Select a type from the
    <span class="StyleListNumberBold" style="font-weight: bold;">Recon
    Type</span> list box.
    
    **NOTE:** The Recon Type indicates if a rule adds records, deletes
    records or is informational. If a data audit is conducted to
    determine if all data records were loaded (as they were expected to
    be loaded), the Recon Type justifies why records were not loaded.
    Use the options Adds records (+) or Deletes records (-) on certain
    exports (delta loads, multi-step loads, etc.) from the Target
    Reconciliation Report.

15. Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>.

16. Click the **Audit** icon to register audit rules, if applicable.

**NOTE:** Refer to [Add Source Audit Rules](Add_Source_Audit_Rules.htm)
for detailed information.

Target source rules can be run in the foreground or background.

**NOTE:** If a process takes less than 0.5 seconds to run, the duration
in the DURATION field is 0.

Run a rule in the background if there is a large amount of data to
process that may affect system performance or may time out a session.
Monitor rules that run in the background on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page.

A rule that runs in the foreground processes immediately.

To run a Target Source rule in the background in Transform:

1.  Click the **Process Information** tab on the *Target Source Rules*
    page's *Vertical* View.
2.  Click the **Process** icon; a confirmation message displays.
3.  Click **OK**.

To run a Target Source rule in the foreground in Transform:

1.  Navigate to the *Target Source Rule* page's *Horizontal* View.
2.  Click the **Execute** icon in the Page toolbar; a confirmation
    message displays.
3.  Click **OK**.
