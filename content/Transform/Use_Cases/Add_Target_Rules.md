+++
title = 'Add Target Rules'
solution = 'Migration'
+++

# Add Target Rules

A Target rule cleans and manipulates data before it is loaded into the
Target.

Each rule consists of a view and a stored procedure that must be created
and stored in the Target table.

**NOTE:** BackOffice follows a strict naming convention for creating
names that each member of the object can understand. Any manually
created objects must also follow these conventions. Refer to [Naming
Conventions](Naming_Conventions.htm) for more information.

**NOTE:** Target rules can be created automatically using SQL AutoGen.
Refer to [Create Rules](../../SQL_AutoGen/Use_Cases/Create_Rules.htm)
for more information.

To add a Target rule in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the
    <span class="StyleListNumberBold" style="font-weight: bold;">Rules</span>
    icon for a Target.
    
    **NOTE:** The *[Target Rules](../Page_Desc/Target_Rules_H.htm)* page
    displays in Add Mode if no Target rules have been built for the
    Target.

3.  Click **Add**.
    
    *[View the field descriptions for the Target Rules
    page.](../Page_Desc/Target_Rules_H.htm)*

4.  Enter a sort value in the **PRIORITY** field.
    
    **NOTE:** If multiple rules are registered to the Target, the
    priority determines the order the rule is processed.

5.  Select a value from the
    <span class="StyleListNumberBold" style="font-weight: bold;"><span id="Status" class="popUpLink">STATUS</span></span>
    list box.

6.  Select a type from the **RULE TYPE** list box. Options are:
    
      - **Delete –** Delete only rules.
      - **Insert –** Insert only rules.
      - **Manual –** All rules.
      - **Move–** Move only rules.
      - **Update –** Update only rules.

7.  Select an option from the **TARGET RULE** list box.
    
    **NOTE:** The TARGET RULE is a stored procedure that must exist in
    the SQL database.
    
    <span style="font-weight: bold;">NOTE:</span> Only rules that use
    the proper naming convention display in the list box. Refer to
    [Naming Conventions](Naming_Conventions.htm) for more information.

8.  Enter a brief Target rule description in the
    <span class="StyleListNumberBold" style="font-weight: bold;">DESCRIPTION</span>field.

9.  Select a view from the **TARGET RULE VIEW** list box.
    
    **NOTE:** The Target rule view must exist in the SQL database.
    
    <span style="font-weight: bold;">NOTE:</span> Only views that use
    the proper naming convention display in the list box. Refer to
    [Naming Conventions](Naming_Conventions.htm) for more information.

10. Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>;
    the *Vertical* View displays.

11. Click the **Documentation** tab.

12. Click **Edit.**
    
    *[View a field descriptions of the Target Rule page’s Vertical View
    Documentation
    tab](../Page_Desc/Target_Rules_H.htm#Target_Rules_V_All_Tabs)*

13. Enter text in
    <span class="StyleListNumberBold" style="font-weight: bold;">Comment</span>
    field to document any notes about the Target Rule.

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

16. Click **Audit** to register audit rules, if applicable.
    
    **NOTE:** Refer to the [Add Target Audit
    Rules](Add_Target_Audit_Rules.htm) section for detailed information.

Target rules can be run in the foreground or background.

<span style="font-weight: bold;">NOTE:</span> If a process takes less
than 0.5 seconds to run, the duration in the DURATION field is 0.

Run a rule in the background if there is a large amount of data to
process that may affect system performance or may time out a session.
Monitor rules that run in the background on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page.

A rule that runs in the foreground processes immediately.

To run a Target rule in the background in Transform:

1.  Click the **Process Information** tab on the *Vertical* View.
2.  Click the **Process** icon; a confirmation message displays.
3.  Click **OK**.

To run a Target rule in the foreground in Transform:

1.  Navigate to the *Horizontal* View.
2.  Click **Execute**; a confirmation message displays.
3.  Click **OK**.

Additional features are available for Target rules:

  - <span style="font-weight: bold;">Reset</span> – Resets the
    processing status if the process fails for any of the Target rules.
    This option is available on the *Horizontal* View only.
  - <span style="font-weight: bold;">Queue</span> – Allows monitoring of
    background job processes for Target rules. This option is available
    on the *Horizontal* View only.
  - <span style="font-weight: bold;">Build Rule</span> – Builds a new
    rule based on the Target Rule view. If a rule already exists, it is
    overwritten. This option is available on the *Vertical* View General
    tab.
