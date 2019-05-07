+++
title = 'Configure a Process Template Loop for a SAP Data Services Job Process Template Automatically'
solution = 'Platform'
+++

# Configure a Process Template Loop for a SAP Data Services Job Process Template Automatically

Follow these steps if using Global Variables, which are optional.

A process template loop assigns a view from the process’s data source to
a loop within the template. The loop is mapped to a view which contains
the data to post for the corresponding template loop in the process. In
the case of SAP Data Services Job templates, the data is global variable
names and values that are used as inputs to a Data Services Job.

The view that stores these fields and the field mappings can be created
manually. Refer to [Create a View in SQL
Server](Create_a_View_in_SQL_Server.htm) for more information.

The view can also be generated automatically. Refer to [Generate
Database Objects
Automatically](Generate_Database_Objects_Automatically.htm) for more
information.

A process template loop can be configured manually or automatically.
Refer to [Configure a Process Template Loop for a SAP Data Services Job
Process Template
Manually](Configure_a_Process_Template_Loop_for_a_SAP_Data_Services_Job_Process_Template_Manually.htm)
for more information.

Before performing this task [Add the Template to a
Process](Add_the_Template_to_a_Process_DSJob.htm) but
<span style="font-weight: bold;">do not select a View Name</span>.

Once a SAP Data Services Job template has been added to a process,
access the <span style="font-style: italic;">[Process Template
Loop](../Page_Desc/Process_Template_Loop.htm)</span> page to view the
single loop Integrate added automatically to the process. The loop,
called GlobalVariables, has two fields.

The Name is the unique name for the Global Variable.

The Value  is used whenever this Global Variable is identified on a
posting record, unless otherwise indicated by the Where clause used in
the process post (entered on the
<span style="font-style: italic;">Vertical</span> View on the
<span style="font-style: italic;">[Process
Post](../Page_Desc/Process_Post_H.htm)</span> page).

<span style="font-weight: bold;">NOTE</span>: A process must be inactive
to configure its process template loops.

To configure the process template loop using the Auto Generate Database
Objects feature:

1.  Select <span style="font-weight: bold;">Categories</span> from
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    the category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a process.

4.  Click the <span style="font-weight: bold;">Loops</span> icon for the
    template.

5.  Click <span style="font-weight: bold;">Auto Generate Database
    Objects.</span>
    
    <span style="font-weight: bold;">NOTE</span>: Auto Generate Database
    Objects create tables and views in the designated database for the
    process template loop. Integrate creates a view with the name
    tx\[Process Name\] \_{Template Name}\_{LoopName}Int and creates a
    table with the name tt\[Process Name\]\_ \[Template
    Name\]\_{LoopName}\_Upload.  
    The feature also:

Populates the VIEW NAME field in Integrate with \[Process Name\]
\[Template Name\]

Sets the PRIMARY KEY COLUMN NAME to ID

Automatically maps the fields for the process template loop. The
TEMPLATE FIELD UNIQUE NAME and the MAPPING VALUE column have the same
value.

Continue with [Configure Field Mappings for an SAP Data Services Job
Process
Template](Configure_Field_Mappings_for_an_SAP_Data_Services_Job_Process_Template.htm).
