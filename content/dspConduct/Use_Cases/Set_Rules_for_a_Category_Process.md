+++
title = 'Set Rules for a Category Process'
solution = 'Master Data Management'
+++

# Set Rules for a Category Process

A Designer can register a rule, in the form of a SQL stored procedure,
to a category process. The rule is executed right before the process is
posted via a Group post or single posting event. These rules are
preparation procedures that move data from the request tables to the
integrate staging tables needed for integrate to post successfully.

This task is optional. Not every process requires a rule.

<span style="font-weight: bold;">NOTE</span>: The rule must be a stored
procedure written in SQL stored in a data source that has been
registered in the DSP®.

The Designer can select other rules at the scenario level as needed.
Refer to [Add Process Rules at the Scenario
Level](Add_Process_Rules_at_the_Scenario_Level.htm) for more
information.

To register a rule for a category process in dspConduct:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Vertical View</span> for a
    category.

3.  Click the <span style="font-weight: bold;">Posting Processes</span>
    icon.

4.  Click the <span style="font-weight: bold;">Rules</span> icon for a
    process.

5.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Category Process Rule
    page](../Page_Desc/Category_Process_Rule.htm)

6.  Enter a value in the
    <span style="font-weight: bold;">PRIORITY</span> field.
    
    **NOTE:** If the process has multiple rules, the priority sets the
    order these rules run.

7.  Select the data source that stores the rule from the
    <span style="font-weight: bold;">DATA SOURCE ID</span> list box.
    
    **NOTE:** An Administrator must have registered this data source in
    the platform.

8.  Select the rule in the <span style="font-weight: bold;">RULE</span>
    list box.

9.  Enter a brief description of the rule in the
    <span style="font-weight: bold;">DESCRIPTION</span> check box.

10. Click <span style="font-weight: bold;">Save</span>.

<span style="font-weight: bold;">NOTE:</span> After the rule is assigned
to the category process, it is also assigned to that process in all
scenarios. However, these rules are not active for the scenario by
default and a Designer must activate the rule for it to run for the
process.

To activate the rule registered at the category process level at the
scenario level in dspConduct:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Scenarios</span> icon for
    a category.
3.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a scenario.
4.  Click the <span style="font-weight: bold;">Rules</span> icon for a
    process.
5.  Click <span style="font-weight: bold;">Edit</span>.
6.  Click the <span style="font-weight: bold;">ACTIVE</span> check box
    for a rule.
