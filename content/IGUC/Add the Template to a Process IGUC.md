+++
title = 'Add the Template to a Process'
solution = 'Platform'
+++

# Add the Template to a Process

A Template Administrator can add a template to a Process so that the
Process template can be used to post data to the target system.

Refer to [Manage Processes](../Integrate/Use_Cases/Manage_Processes)
for an overview of Processes.

Before performing this task, [create a
template](Create%20an%20IG%20Universal%20Connect%20Template) and
[activate it.](Activate%20the%20Template%20IGUC)

For general information about the IG Universal Connect template, refer
to [Post Data Using IG Universal
Connect](Post%20Data%20Using%20IG%20Universal%20Connect%20Overview).

To add an IG Universal Connect Template template to a Process in
Integrate:

1.  Select <span style="font-weight: bold;">Categories</span> from
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a category.
    
    <span style="font-weight: bold;">NOTE:</span> The number on the
    Processes icon represents the number of active and inactive
    processes assigned to the category.

3.  Click <span style="font-weight: bold;">Add</span>; the
    <span style="font-style: italic;">Vertical</span> View displays.
    
    [View the field descriptions for the Process page’s Vertical
    View.](../Integrate/Page_Desc/Process_H#Process_V_All_Tabs)
    
    <span style="font-weight: bold;">NOTE:</span> At least one active
    template must exist for the category before a process can be added.

4.  Enter a sort value in
    <span style="font-weight: bold;">Priority</span>.
    
    <span style="font-weight: bold;">NOTE:</span> This value determines
    the order the process displays on the
    <span style="font-style: italic;">[Process](../Integrate/Page_Desc/Process_H)</span>
    page.

5.  Enter a process name in
    <span style="font-weight: bold;">Name</span>.
    
    <span style="font-weight: bold;">NOTE:</span> A process name must be
    unique. The process name can contain A-Z, 0-9, and underscore. No
    special characters are allowed in process names. Integrate will
    replace special characters with underscores when the process is
    saved.

6.  Enter a description in
    <span style="font-weight: bold;">Description</span>.

7.  Select the IG Universal Connect template from the
    <span style="font-weight: bold;">Template ID</span> list box.
    
    <span style="font-weight: bold;">NOTE:</span> The Template ID list
    box only displays active templates assigned to the category.

8.  Select the data source where the data to be posted is stored and
    where the integration views (tx\*Iint) exist from **Data Source ID**
    list box.
    
    <span style="font-weight: bold;">NOTE:</span> The Data Source ID
    list box displays all data sources registered to the platform’s
    instance.

9.  Select an option in the <span style="font-weight: bold;">View
    Name</span> list box if the view to store the parameter names and
    values has already been created in the data source.
    
    <span style="font-weight: bold;">NOTE:</span> Parameters are
    optional.
    
    <span style="font-weight: bold;">NOTE:</span> The view can also be
    automatically generated. In this case, leave the View Name blank.
    Refer to [Configure a Process Template Loop for an IG Universal
    Connect Process Template
    Automatically](Configure%20a%20Process%20Template%20Loop%20for%20an%20IG%20Universal%20Connect%20Process%20Template%20Automatically)
    for more information.

10. Click <span style="font-weight: bold;">Save</span>; the Template ID
    is automatically registered to the process.

Continue with [Activate the
Process](Activate%20the%20Process%20IGUC), or, if using parameters,
Configure a Process Template Loop for an IG Universal Connect Process
Template
[Manually](Configure%20a%20Process%20Template%20Loop%20for%20an%20IG%20Universal%20Connect%20Process%20Template%20Manually)
or
[Automatically](Configure%20a%20Process%20Template%20Loop%20for%20an%20IG%20Universal%20Connect%20Process%20Template%20Automatically).
