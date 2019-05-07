+++
title = 'Register a Status View as an After Post Rule'
solution = 'Platform'
+++

# Register a Status View as an After Post Rule

When posting data to a target system, a Template Administrator can
register an After Post Rule to a process template. The rule runs after
the process template executes successfully and before the next process
template begins processing (if posting with a multi-template process).

A Status View used to communicate posting status to the user can be run
as an After Post Rule. The view status is "pass" when there are no
records in the view for the PostingID (i.e., all the records posted
successfully). The view status is "fail" if the view contains at least
one record of data for the PostingID (i.e., at least one record failed
to post). The view’s failed status becomes the posting status of that
template.

Before performing this task, a Template Administrator must [create a
category](../Config/Create_Categories.htm), [create a
template](Create_a_Basic_Template.htm), and [create a
process](Create_a_Process.htm). A Status View must be written and stored
in a data source accessible to the platform.

Refer to [Register After Post Rules to a Process Template
Overview](Register_After_Post_Rules_to_a_Process_Template_Overview.htm)
for general information.

<span style="font-weight: bold;">NOTE</span>: Status Views must be used
for Asynchronous postings if it is required for an Asynchronous posting
to potentially have a failed status.

To register a Status View After Post rule in Integrate:

1.  Select <span style="font-weight: bold;">Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a process.

4.  Click the <span style="font-weight: bold;">After Post Rules</span>
    icon for the template ID.
    
    <span style="font-weight: bold;">NOTE</span>: If no After Post rules
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

6.  Select the data source that stores the view in the
    <span style="font-weight: bold;">Status View Data Source ID</span>
    list box.

7.  Select the name of the view in the
    <span style="font-weight: bold;">Status View</span> list box.

8.  Click <span style="font-weight: bold;">Save</span>.
