# Register a Collect Download After Post Rule Manually

When posting data to a target system, a Template Administrator can
register an After Post Rule to a process template. The rule runs after
the process template executes successfully and before the next process
template begins processing (if posting with a multi-template process).

Before performing this task, a Template Administrator must [create a
category](../Config/Create_Categories.htm), [create a
template](Create_a_Basic_Template.htm), and [create a
process](Create_a_Process.htm). The target, source and tables must be
registered in Collect.

A Collect Download rule downloads a Collect source - target - table
registration. When registering a Collect Download as an After Post Rule,
the source, target, and table to download must be selected. Once
selected, the source and target Where clauses can be manually entered or
[automatically built at run
time](Register_a_Collect_Download_After_Post_Rule_that_is_Built_Automatically.htm).
 

Refer to [Register After Post Rules to a Process Template
Overview](Register_After_Post_Rules_to_a_Process_Template_Overview.htm)
for general information.

To manually create a Collect Download After Post Rule in Integrate:

1.  Select <span style="font-weight: bold;">Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a process.

4.  Click the <span style="font-weight: bold;">After Post Rules
    </span>icon for a template ID.
    
    <span style="font-weight: bold;">NOTE</span>: If no After Post Rules
    have been added to the process template,
    <span style="font-style: italic;">Vertical</span> View displays. If
    rules do exist, click Add on the
    <span style="font-style: italic;">Process Templates: After Post
    Rules</span> page’s
    <span style="font-style: italic;">Horizontal</span> View.
    
    [View the field descriptions for the Process Templates: After Post
    Rules
    page](../../../Master_Data_Mgmt/dspConduct/Page_Desc/Process_Templates_After_Post_Rules_H.htm)

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

9.  Enter the rule to run on target data after the table downloads in
    the <span style="font-weight: bold;">Collect Target Where
    Clause</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: The Where clause
    selects records to delete from the target before the download.
    
    <span style="font-weight: bold;">NOTE</span>: The data returned from
    this Where clause is used as an input parameter to the next template
    in the process.
    
    <span style="font-weight: bold;">NOTE</span>: The Where clause must
    be syntactically correct.

10. Enter the rule to run on source data after the table downloads in
    the <span style="font-weight: bold;">Collect Source Where
    Clause</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: The Where clause must
    be syntactically correct.
    
    <span style="font-weight: bold;">NOTE</span>: The Where clause
    selects records to download from the source to the target.
    
    <span style="font-weight: bold;">NOTE</span>: The data returned from
    this Where clause is used as an input parameter to the next template
    in the process.

11. Click <span style="font-weight: bold;">Save</span>.
