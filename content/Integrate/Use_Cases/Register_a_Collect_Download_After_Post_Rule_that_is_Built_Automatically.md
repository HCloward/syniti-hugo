+++
title = 'Register a Collect Download After Post Rule that is Built Automatically'
solution = 'Platform'
+++

# Register a Collect Download After Post Rule that is Built Automatically

When posting data to a target system, a Template Administrator can
register an After Post Rule to a process template. The rule runs after
the process template executes successfully and before the next process
template begins processing (if posting with a multi-template process).

Before performing this task, a Template Administrator must [create a
category](../Config/Create_Categories), [create a
template](Create_a_Basic_Template), and [create a
process](Create_a_Process). The target, source and tables must be
registered in Collect.

A Collect Download rule downloads a Collect source - target - table
registration.  When registering a Collect Download as an After Post
Rule, the source, target, and table to download must be selected. Once
selected, the source and target Where clauses can be [manually
entered](Register_a_Collect_Download_After_Post_Rule_Manually) or
automatically built at run time.  

Refer to [Register After Post Rules to a Process Template
Overview](Register_After_Post_Rules_to_a_Process_Template_Overview)
for general information.

To automatically create a Collect Download After Post Rule at run time
in Integrate:

1.  Select <span style="font-weight: bold;">Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a process.

4.  Click the <span style="font-weight: bold;">After Post Rules</span>
    icon for template ID.
    
    <span style="font-weight: bold;">NOTE</span>: If no After Post Rules
    have been added to the process template,
    <span style="font-style: italic;">Vertical</span> View displays. If
    rules do exist, click Add on the
    <span style="font-style: italic;">Process Templates: After Post
    Rules</span> page’s
    <span style="font-style: italic;">Horizontal</span> View.
    
    [View the field descriptions for the Process Templates: After Post
    Rules
    page](../../../Master_Data_Mgmt/dspConduct/Page_Desc/Process_Templates_After_Post_Rules_H)

5.  Enter a number in the
    <span style="font-weight: bold;">Priority</span> field to set the
    order this After Post Rule runs if multiple After Post Rules exist.
    
    <span style="font-weight: bold;">NOTE</span>: Rules execute in
    ascending priority order.

6.  Select the source name to use for the Collect Download in the
    <span style="font-weight: bold;">Collect Source</span> list box.

7.  Select the target name to use for the Collect Download in the
    <span style="font-weight: bold;">Collect Target</span> list box.

8.  Select the name of the target or source table to download in the
    <span style="font-weight: bold;">Collect Table Name</span> list box.

9.  Click <span style="font-weight: bold;">Save</span>.

10. Click the <span style="font-weight: bold;">Collect Where
    Clause</span> icon.

11. Enter the column name that is evaluated by the Where clause in the
    <span style="font-weight: bold;">Column Name</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: The column is stored
    in the table in the Collect Table Name field.

12. Select the operator for the Where clause in the
    <span style="font-weight: bold;">Operator</span> list box.

13. Enter the value to use in the Where clause in the
    <span style="font-weight: bold;">Value</span> field.

14. Click <span style="font-weight: bold;">Save</span>.

At run time, the system automatically builds the Where clause.
