# Add Source Audit Rules

If auditing is enabled, Transform creates an Excel file to record what
data was manipulated by the Target Source rule, how long it took to run,
who ran it and other details.

To enable auditing in Transform, access Console:

1.  Select <span style="font-weight: bold;">Advanced Configuration \>
    Parameters</span> in the *Navigation* pane.

2.  Click the **Transform** tab.
    
    *[View the field descriptions for the Transform tab on the
    Parameters page in
    Console](../../Console/Page_Desc/Parameters.htm#Transform_Tab)*

3.  Click the **Audit Reports** check box to check it.

To register an audit rule to a Target Source in Transform:

1.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](../Page_Desc/Process_Area_Launch.htm)*
    page.

2.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

3.  Click the
    <span class="StyleListNumberBold" style="font-weight: bold;">Rules</span>
    icon for a Target Source.

4.  Click **Vertical View** for a rule.

5.  Click the **Documentation** tab.

6.  Click the <span style="font-weight: bold;">Audit</span> icon.

7.  Click **Add**.
    
    *[View the field descriptions for the Target Source Rule Audit
    page](../Page_Desc/Target_Source_Rule_Audit.htm)*

8.  Select an option from the
    **<span id="Status" class="popUpLink">STATUS</span>** list box.

9.  Select a report to be audited from the **AUDIT REPORT** list box.
    
    **NOTE:** This report was built and is stored in the Source table.

10. Select a method from the **SAMPLE METHOD** list box.
    
    **NOTE:** This sample method is used when selecting random rows of
    data for verification during the audit process. The sample methods
    are set up in Transform by selecting Configuration \> Setup \>
    Sampling Methods (Setup).

11. Click **Save**.

Source audit rules can be run in the foreground or background.

Run a rule in the background if there is a large amount of data to
process that may affect system performance or may time out a session.
Monitor rules that run in the background on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page.

A rule that runs in the foreground processes immediately.

To run a Source audit rule in the background in Transform:

1.  Navigate to the Target Source Rule's
    <span style="font-style: italic;">Vertical</span>View.
2.  Click the **Process Information** tab.
3.  Click the **Process** icon; a confirmation message displays.
4.  Click **OK**.

To run a Source audit rule in the foreground in Transform:

1.  Navigate to the *[Target Source
    Rules](../Page_Desc/Target_Source_Rules_H.htm)* page's *Horizontal*
    View.
2.  Click the **Execute** icon in the Page toolbar; a confirmation
    message displays.
3.  Click **OK**

To view the audit data returned from the rule in Transform:

1.  Access the *Target Source Rules* page.

2.  Click **Vertical View** for the rule.

3.  Click the **Documentation** tab.

4.  Click the **Audit** icon.

5.  Click the <span style="font-weight: bold;">Download</span> icon to
    view the audit data.
    
    **NOTE:** This icon is enabled if the audit report displays data met
    by the sample criteria.
