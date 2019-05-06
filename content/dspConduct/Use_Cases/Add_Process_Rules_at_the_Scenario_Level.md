# Add Process Rules at the Scenario Level

A Designer can register a rule, in the form of a SQL stored procedure,
to a scenario process. These rules are any stored procedures that need
to execute before the process is used for posting. These rules must
include preparation procedures that move data from the request tables to
the integrate staging tables needed for integrate to post successfully.
Any rule registered to the process and marked as Active is executed
right before the process is posted via a Group post or single posting
events.

Rules can be assigned to the process by default at the category level.
Refer to [Set Rules for a Category
Process](Set_Rules_for_a_Category_Process.htm) for more information.

<span style="font-weight: bold;">NOTE</span>: The rule must be a stored
procedure written in SQL stored in a data source that has been
registered in the DSP®.

<span style="font-weight: bold;">NOTE</span>: The rules registered at
the scenario level do not need to be registered at the category level.

To add a process rule at the scenario level:

1.  Click <span style="font-weight: bold;">dspConduct
    \></span><span style="font-weight: bold;">Design</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Scenarios</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a scenario.

4.  Click the <span style="font-weight: bold;">Rules</span> icon.

5.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Scenario Process Rule
    page](../Page_Desc/Scenario_Process_Rule.htm)

6.  Enter a value in the
    <span style="font-weight: bold;">PRIORITY</span> field.
    
    **NOTE:** If multiple rules are assigned to the process, the
    priority determines the order rules are run for the process.

7.  Select the data source that stores the rule from the
    <span style="font-weight: bold;">DATA SOURCE ID</span> list box.
    
    **NOTE:** An Administrator must have registered this data source in
    the platform.

8.  Select the rule in the <span style="font-weight: bold;">RULE</span>
    list box.

9.  Enter a brief description of the rule in the
    <span style="font-weight: bold;">DESCRIPTION</span> check box.

10. Click the <span style="font-weight: bold;">ACTIVE</span> check box
    to enable it.
    
    **NOTE:** This check box is not enabled by default but must be
    enabled for the rule to run.

11. Click <span style="font-weight: bold;">Save</span>.
