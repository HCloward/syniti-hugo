+++
title = 'Register a Stored Procedure as an After Post Rule'
solution = 'Platform'
+++

# Register a Stored Procedure as an After Post Rule

When posting data to a target system, a Template Administrator can
register an After Post Rule to a process template. The rule runs after
the process template executes successfully and before the next process
template begins processing (if posting with a multi-template process).

A stored procedure can be run as an After Post rule that may take a
variable of @PostingID GUID. If this property exists, then the PostingID
of the posting passes to the procedure. When a business rule After Post
rule is encountered, Integrate runs the rule and waits for it to
complete before running the next rule.

Before performing this task, a Template Administrator must [create a
category](../Config/Create_Categories), [create a
template](Create_a_Basic_Template), and [create a
process](Create_a_Process). A stored procedure must be written and
stored in a data source accessible to the platform.

Refer to [Register After Post Rules to a Process Template
Overview](Register_After_Post_Rules_to_a_Process_Template_Overview)
for general information.

To register a stored procedure After Post rule in Integrate:

1.  Select <span style="font-weight: bold;">Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a process.

4.  Click the <span style="font-weight: bold;">After Post Rules</span>
    icon for a template ID.
    
    <span style="font-weight: bold;">NOTE</span>: If no After Post rules
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

6.  Select the data source that stores the rule from the
    <span style="font-weight: bold;">After Post Rule Data Source
    ID</span> list box.

7.  Select the rule from the<span style="font-weight: bold;"> After Post
    Rule</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: The data returned from
    this rule is used as an input parameter to the next template in the
    process.

8.  Click <span style="font-weight: bold;">Save</span>.
