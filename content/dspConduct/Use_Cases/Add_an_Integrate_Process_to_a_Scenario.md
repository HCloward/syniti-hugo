+++
title = 'Add an Integrate Process to a Scenario'
solution = 'Data Quality'
+++

# Add an Integrate Process to a Scenario

Integrate processes are the methods in which data from dspConduct™ is
posted into a target system. Integrate processes are registered by a
Designer to scenarios on dspConduct™
<span style="font-style: italic;">[Scenario
Process](../Page_Desc/Scenario_Process.htm)</span> page. The process
must be active in Integrate to be available to add to a scenario. Refer
to [Create a
Process](../../../Platform/Integrate/Use_Cases/Create_a_Process.htm) in
Integrate for more information about processes. This task must be
completed in order for requests created from the scenario to be posted
to the target system.

Before adding a process to a scenario, [Add a
Scenario](Add_Scenario.htm).

**NOTE:** An Integrate process cannot be deactivated or deleted if it is
assigned to a dspConduct™ scenario that has a status of published.

<span style="font-weight: bold;">NOTE</span>: The Integrate process must
be active to be used for posting.

<span style="font-weight: bold;">NOTE</span>: When a Request is created,
each Integrate Process assigned to the Scenario is assigned a unique
Posting ID which can be used to assist while troubleshooting. Integrate
uses this Posting ID as a parameter for Integrate Process Template rules
and validations. The Integrate Process is also passed a Where Clause
used for the posting data views that only contains the Request ID (e.g.
“WHERE RequestID = 999”).

To add a process to a scenario in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Design** in the *Navigation* pane.

2.  Click the **Scenarios** icon for a category on the *Category* page.

3.  Click the **Processes** icon for a scenario.

4.  Click **Add**.
    
    *[View the field descriptions for the Scenario Process
    page.](../Page_Desc/Scenario_Process.htm)*

5.  Select the Integrate process for posting from the **INTEGRATE
    PROCESS ID** list box.
    
    **NOTE**: Only allowed processes set at the category level display.
    Refer to [Set Allowed Processes at the Category
    Level](Set_Allowed_Processes_at_the_Category_Level.htm) for more
    information.

6.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** This value determines the order the process displays on
    the *[Scenario Process](../Page_Desc/Scenario_Process.htm)* page and
    the order in which the processes are executed for posting.

7.  Click **Save**.
