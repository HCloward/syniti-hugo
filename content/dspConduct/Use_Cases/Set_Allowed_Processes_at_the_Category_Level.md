+++
title = 'Set Allowed Processes at the Category Level'
solution = 'Master Data Management'
+++

# Set Allowed Processes at the Category Level

Integrate processes are the methods in which data from dspConduct™ is
posted into a target system.

A Designer can limit the allowed processes for scenarios at the category
level. Only these allowed processes display in the INTEGRATE PROCESS ID
list box on the <span style="font-style: italic;">[Scenario
Process](../Page_Desc/Scenario_Process.htm)</span> page.

<span style="font-weight: bold;">NOTE</span>: This task must be
completed so that requests created from the scenario are posted to the
target system. Refer to [Add a Process to a
Scenario](Add_an_Integrate_Process_to_a_Scenario.htm) for more
information.

The process must be active in Integrate to be registered at the category
or scenario level.

To set allowable processes:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Vertical View</span> for a
    category.

3.  Click the <span style="font-weight: bold;">Posting Processes</span>
    icon.

4.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Category Process
    page](../Page_Desc/Category_Process.htm)

5.  Select the allowable process for scenarios in the category from
    the<span style="font-weight: bold;"> INTEGRATE PROCESS ID</span>
    list box.
    
    **NOTE:** All active processes available in Integrate display.

6.  Click <span style="font-weight: bold;">Save</span>.

After the record is saved, click the link for the integrate process to
view details about the process in Integrate.

A Designer can also register a rule, if needed, in the form of a SQL
stored procedure, to the process that is executed right before the
process is posted via a Group post or single posting events. Refer to
[Set Rules for a Category Process](Set_Rules_for_a_Category_Process.htm)
for more information.
