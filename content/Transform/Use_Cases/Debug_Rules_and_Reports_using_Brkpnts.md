+++
title = 'Debug Rules and Reports using Breakpoints'
solution = 'Migration'
+++

# Debug Rules and Reports using Breakpoints

A breakpoint stops rule or report processing at a specified place to
assist when troubleshooting an issue. Set breakpoints on the *[Debug –
Breakpoints](../Page_Desc/Debug_Breakpoints.htm)* page, which displays
all the steps that can be processed for the selected Target or Target
Source.

Make changes to the rule or report, then add a breakpoint to stop the
job prior to the rule or report is run to see if the fix was successful.

Breakpoints can be set for Target Source rules, Target Source reports,
Target rules and Target reports.

A Transform job processes in this order: Source imports, Source Rules,
Source Reports, Target, Target Rules, Target Reports. These processes
also display in this order on the *Debug – Breakpoints* page. The Target
priority, Source priority and rule and report priority determine the
order that individual Targets, Sources, rules and reports are run.

**NOTE:** A Target can be debugged if it is in a valid and executable
Transform <span id="Status" class="popUpLink">status</span> (a status
that has the Execute check box checked on the *Status Setup* page). By
default, items in a status of Active or Development can be executed

Setting breakpoints for Target rules, Target reports, Target Source
rules and Target Source reports follows the same process.

Set breakpoints for the selected Target’s Target rules and Target
reports by clicking the Debug icon on the Page toolbar on the
*[Targets](../Page_Desc/Targets_H.htm)* page, the *[Target
Reports](../Page_Desc/Target_Reports_H.htm)* page, and the *[Target
Rules](../Page_Desc/Target_Rules_H.htm)* page. Accessing the *Debug –
Breakpoints* page from any of these pages displays all of the steps in
the process that can be debugged for the selected Target.

Set breakpoints for Target Source rules and Target Source reports by
clicking the Debug icon on the Page toolbar on the *[Target
Sources](../Page_Desc/Target_Sources_H.htm)* page, the *[Target Source
Reports](../Page_Desc/Target_Source_Reports_H.htm)* page, and the
*[Target Source Rules](../Page_Desc/Target_Source_Rules_H.htm)* page.
Accessing the *Debug – Breakpoints* page from any of these pages
displays all of the steps in the process that can be debugged for the
selected Target Source.

**NOTE:** When the *Debug – Breakpoints* page is open, the Process icon
is disabled on the *Targets*, *Target Sources*, and their corresponding
rules and reports pages.

To set and use a breakpoint in Transform:

1.  Click the **Debug** icon on the Page toolbar.

2.  Click the **Breakpoint** check box to set a breakpoint for each
    report or rule in the process to be debugged.
    
    **NOTE:** This breakpoint stops the job prior to running the rule or
    report.

3.  Click the **Process** icon in the Page toolbar to run the job up to
    the breakpoint.
    
    **NOTE:** A processing icon displays until the job has reached the
    breakpoint.

4.  Once the breakpoint has been reached, examine the rule or report in
    SQL to confirm fixes worked.

5.  Click the **Continue From** icon in the Page toolbar to continue
    processing the job from the current breakpoint. The job runs until
    another breakpoint is encountered or until the job is finished.

6.  Click the **Clear Breakpoints** icon in the Page toolbar to remove
    all breakpoints.
