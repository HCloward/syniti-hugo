# Set Available Connections at the Process Template Level

A Process Designer can reuse a process template by adding connections to
load programs for multiple target systems to a single process template.
Data can then be posted to these target systems sequentially.

Refer to [Post Data to Multiple Target Systems with One Process
Template](Post_Data_to_Multiple_Target_Systems_with_One_Process_Template.htm)
for general information.

Before performing this task, add a template and add a process.

The steps to add a template and process are different for each template
type. Refer to the sections specific to the template type for more
information:

  - [Post Data with a BDC Script](Post_Data_with_a_BDC_Script.htm)

  - [Post Data Using a GUI Script](Post_Data_Using_a_GUI_Script.htm)

  - [Post Data Using a BAPI](Post_Data_Using_a_BAPI.htm)

  - [Post Using RFC Execution](Post_Using_RFC_Execution.htm)

  - [Create and Transfer Files for User Defined Fixed Width or Delimited
    Templates](CreatTransferFilesUrDTemplates.htm)

  - [Create and Transfer XML Files](CreateTransferXMLOverview.htm)

  - [Post Data Using an SAP Data Services
    Job](Post_Data_Using_an_SAP_Data_Services_Job_Overview.htm)

  - [Post Data Using IG Universal
    Connect](../../IGUC/Post%20Data%20Using%20IG%20Universal%20Connect%20Overview.htm)

<span style="font-weight: bold;">NOTE</span>: The process must be
inactive to add a connection.

To set available connections at the process template level in Integrate:

1.  Click <span style="font-weight: bold;">Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a process.

4.  Click the <span style="font-weight: bold;">Allowed
    Connections</span> icon for the automatically created process
    template.

5.  Note the connection in the
    <span style="font-weight: bold;">CONNECTION ID</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: One record, the
    connection that was added to the template on the
    <span style="font-style: italic;">[Template](../Page_Desc/Template_H.htm)</span>
    page, displays as the default connection. Additional connections can
    be added to this process template, however, the default connection
    is used when posting. The connection can be edited at the process
    post level.

6.  Navigate back to the <span style="font-style: italic;">[Process
    Templates](../Page_Desc/Process_Templates_H.htm)</span> page.

7.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Process Templates
    page.](../Page_Desc/Process_Templates_H.htm)

8.  Enter a number in the
    <span style="font-weight: bold;">PRIORITY</span> field.

9.  Select the same template as the one in the first process template
    from the <span style="font-weight: bold;">TEMPLATE ID</span> list
    box.

10. Click <span style="font-weight: bold;">Save</span>.

11. Click the <span style="font-weight: bold;">Allowed Connections
    i</span>con for the second process template.

12. Select the connection to the second target system from the
    <span style="font-weight: bold;">CONNECTION ID</span> list box.

13. Click <span style="font-weight: bold;">Save</span>.

14. Click the <span style="font-weight: bold;">Set Default</span> icon
    in the Page toolbar.
    
    <span style="font-weight: bold;">NOTE</span>: Additional connections
    can be added, but only one default connection is allowed.

15. Navigate back to the <span style="font-style: italic;">Process
    Templates</span> page.

16. Click the
    <span style="font-weight: bold;">ACTIVATE/DEACTIVATE</span> icon for
    the process on the
    <span style="font-style: italic;">[Process](../Page_Desc/Process_H.htm)</span>
    page.

Continue with [editing connections to target systems at the process post
level](Edit_Connections_to_Target_Systems_at_the_Process_Post_Level.htm)
(if needed).
