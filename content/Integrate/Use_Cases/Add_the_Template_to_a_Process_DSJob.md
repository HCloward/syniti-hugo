+++
title = 'Add the Template to a Process'
solution = 'Platform'
+++

# Add the Template to a Process

A Template Administrator can add a template to a process so that the
process template can be used to post data to the target system.

Refer to [Manage Processes](Manage_Processes) for an overview of
processes..

Before performing this task, [create a
template](Create_an_SAP_Data_Services_Job_template) and [activate
it](Activate_the_Template_DS_Job).

For general information about the SAP Data Services Job template, refer
to [Post Data Using an SAP Data Services Job
Overview](Post_Data_Using_an_SAP_Data_Services_Job_Overview).

To add a SAP Data Services Job template to a process in Integrate:

1.  Select <span style="font-weight: bold;">Categories</span> from
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a category.
    
    <span style="font-weight: bold;">NOTE</span>: The number on the
    Processes icon represents the number of active and inactive
    processes assigned to the category.

3.  Click <span style="font-weight: bold;">Add</span>; the
    <span style="font-style: italic;">Vertical</span> View displays.
    
    [View the field descriptions for the Process page’s Vertical
    View.](../Page_Desc/Process_H#Process_V_All_Tabs)
    
    <span style="font-weight: bold;">NOTE</span>: At least one active
    template must exist for the category before a process can be added.

4.  Enter a sort value in
    <span style="font-weight: bold;">Priority</span>.
    
    <span style="font-weight: bold;">NOTE</span>: This value determines
    the order the process displays on the
    <span style="font-style: italic;">[Process](../Page_Desc/Process_H)</span>
    page.

5.  Enter a process name in
    <span style="font-weight: bold;">Name</span>.
    
    <span style="font-weight: bold;">NOTE</span>: A process name must be
    unique. The process name can contain A-Z, 0-9, and underscore. No
    special characters are allowed in process names. Integrate will
    replace special characters with underscores when the process is
    saved.

6.  Enter a description in
    <span style="font-weight: bold;">Description</span>.

7.  Select the SAP Data Services Job template from the
    <span style="font-weight: bold;">Template ID</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: The Template ID list
    box only displays active templates assigned to the category.

8.  Select a data source from <span style="font-weight: bold;">Data
    Source ID</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: The Data Source ID
    list box displays all data sources registered to the platform’s
    instance.

9.  Select an option in the <span style="font-weight: bold;">View
    Name</span> list box if the view to store the Global Variables has
    already been created in the data source.
    
    <span style="font-weight: bold;">NOTE</span>: Global Variables are
    optional.
    
    <span style="font-weight: bold;">NOTE</span>: The view can also be
    automatically generated. In this case, leave the View blank. Refer
    to [Configure a Process Template Loop for an SAP Data Services Job
    Process Template
    Automatically](Configure_a_Process_Template_Loop_for_a_SAP_Data_Services_Job_Process_Template_Automatically)
    for more information.

10. Click <span style="font-weight: bold;">Save</span>; the Template ID
    is automatically registered to the process.

Continue with [Activate the Process,](Activate_the_Process8) or, if
using Global Variables, Configure a Process Template Loop for a SAP Data
Services Job Process Template
[Manually](Configure_a_Process_Template_Loop_for_a_SAP_Data_Services_Job_Process_Template_Manually)
or
[Automatically](Configure_a_Process_Template_Loop_for_a_SAP_Data_Services_Job_Process_Template_Automatically).
