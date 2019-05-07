+++
title = 'Add Target Audit Rules'
solution = 'Migration'
+++

# Add Target Audit Rules

If auditing is enabled, Transform creates an Excel file to record what
data was manipulated by the Target Rule, how long it took to run, who
ran it and other details.

To enable auditing in Transform, access Console:

1.  Select **Advanced Configuration \> Parameters** in the *Navigation*
    pane.
2.  Click the **Transform** tab.
3.  Click the **Audit Reports** check box to check it.
4.  Click **Save**.

To register an audit rule to a Target in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the
    <span class="StyleListNumberBold" style="font-weight: bold;">Rules</span>
    icon for a Target.

3.  Click **Vertical View** for a Target Rule.

4.  Click the **Documentation** tab on the *[Target
    Rules](../Page_Desc/Target_Rules_H.htm)* page.

5.  Click the **Audit** icon.

6.  Click **Add**.
    
    *[View the field descriptions for the Target Rule Audit
    page](../Page_Desc/Target_Rule_Audit_H.htm)*

7.  Select an option from the
    **<span id="Status" class="popUpLink">STATUS</span>** list box.

8.  Select a report to be audited from the **AUDIT REPORT** list box.
    
    **NOTE:** This report must have been already created as a view in
    SQL.

9.  Select a method from the **SAMPLE METHOD** list box.
    
    **NOTE:** This sample method is used when selecting random rows of
    data for verification during the audit process. The sample methods
    are set up by selecting Configuration \> Setup \> Sampling Methods
    (Setup).

10. Click **Save**.

Target audit rules can be run in the foreground or background.

Run a rule in the background if there is a large amount of data to
process that may affect system performance or may time out a session.
Monitor rules that run in the background on the *Monitor* page.

A rule that runs in the foreground processes immediately.

To run a Target audit rule in the background in Transform:

1.  Click the **Process Information** tab on the *Vertical* View of the
    *Target Rule Audit* page.
2.  Click the **Process** icon; a confirmation message displays.
3.  Click **OK**.

To run a Target audit rule in the foreground in Transform:

1.  Navigate to *Horizontal* View of the
    <span style="font-style: italic;">Targets</span> page.
2.  Click the **Process** icon on the Page toolbar; a confirmation
    message displays.
3.  Click **OK**.

To view the audit data returned from the rule in Transform:

1.  Access the *Target Rules* page.
2.  Click **Vertical View** for the rule.
3.  Click the **Documentation** tab.
4.  Click the **Audit** icon.
5.  Click the **Download** icon to view the audit data.

**NOTE:** This icon is enabled if the audit report displays data.
