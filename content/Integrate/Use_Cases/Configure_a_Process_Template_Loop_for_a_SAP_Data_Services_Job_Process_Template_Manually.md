# Configure a Process Template Loop for a SAP Data Services Job Process Template Manually

Follow these steps if using Global Variables, which are optional.

A process template loop assigns a view from the process’s data source to
a loop within the template. The loop is mapped to a view which contains
the data to post for the corresponding template loop in the process. In
the case of SAP Data Services Job templates, the data is global variable
names and values that are used as inputs to a Data Services Job.

The view that stores these fields and the field mappings can be created
manually. Refer to [Create a View in SQL
Server](Create_a_View_in_SQL_Server.htm) for more information.

The view  can also be generated automatically. Refer to [Generate
Database Objects
Automatically](Generate_Database_Objects_Automatically.htm) for more
information.

A process template loop can be configured manually or automatically.
Refer to [Configure a Process Template Loop for a SAP Data Services Job
Process Template
Automatically](Configure_a_Process_Template_Loop_for_a_SAP_Data_Services_Job_Process_Template_Automatically.htm)
for more information.

Before performing this task [Add the Template to a
Process](Add_the_Template_to_a_Process_DSJob.htm).

Once an SAP Data Services Job template has been added to a process,
access the [Process Template
Loop](../Page_Desc/Process_Template_Loop.htm) page to view the single
loop Integrate added automatically to the process and to edit the
process template loop. The loop, called GlobalVariables, has two fields
to be mapped: Name and Value.

The Name is the unique name for the Global Variable.

The Value is used whenever this Global Variable is identified on a
posting record, unless otherwise indicated by the Where clause used in
the process post (entered on the
<span style="font-style: italic;">Vertical</span> View on the [Process
Post](../Page_Desc/Process_Post_H.htm) page).

In the View created in the data source, either manually or automatically
generated, add the Global Variable Name and Variable Values to the Name
and Value columns.  

<span style="font-weight: bold;">NOTE</span>: A process must be inactive
to configure its process template loops.

To manually update the VIEW NAME and PRIMARY KEY COLUMN NAME for a
process template loop:

1.  Select <span style="font-weight: bold;">Categories</span> from
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    the category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a process.

4.  Click the <span style="font-weight: bold;">Loops</span> icon for the
    template.
    
    <span style="font-weight: bold;">NOTE</span>: The
    <span style="font-style: italic;">[Process Template
    Loop](../Page_Desc/Process_Template_Loop.htm)</span> page displays
    one loop that Integrate created automatically with the LOOP NAME
    “GlobalVariables.”  The VIEW NAME and PRIMARY KEY COLUMN NAME
    fields are blank.

5.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Process Template Loop
    page.](../Page_Desc/Process_Template_Loop.htm)

6.  Select a name in the <span style="font-weight: bold;">VIEW
    NAME</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: The view must already
    exist in the data source to be available in the list box.

7.  Select a name in the <span style="font-weight: bold;">PRIMARY KEY
    COLUMN NAME</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: The list box displays
    all columns available in the view. The column selected must uniquely
    identify a record in the view.

8.  Click <span style="font-weight: bold;">Save</span>.

Continue with [Configure Field Mappings for an SAP Data Services Job
Process
Template](Configure_Field_Mappings_for_an_SAP_Data_Services_Job_Process_Template.htm).
