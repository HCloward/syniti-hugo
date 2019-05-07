+++
title = 'Configure a Process Template Loop for an IG Universal Connect Process Template Manually'
solution = 'Platform'
+++

# Configure a Process Template Loop for an IG Universal Connect Process Template Manually

Follow these steps if using parameters, which are optional.

A Process Template Loop assigns a view from the Process’s data source to
a loop within the template. The loop is mapped to a view which contains
the data to post for the corresponding template loop in the Process. In
the case of IG Universal Connect Templates, the data is parameter names
and values that are used as inputs to a Boomi Process.

The view that stores these fields and the field mappings can be created
manually. Refer to [Create a View in SQL
Server](../Integrate/Use_Cases/Create_a_View_in_SQL_Server.htm) for more
information.

The view can also be generated automatically. Refer to [Generate
Database Objects
Automatically](../Integrate/Use_Cases/Generate_Database_Objects_Automatically.htm)
for more information.

A Process Template Loop can be configured manually or automatically.
Refer to [Configure a Process Template Loop for an IG Universal Connect
Process Template
Automatically](Configure%20a%20Process%20Template%20Loop%20for%20an%20IG%20Universal%20Connect%20Process%20Template%20Automatically.htm)
for more information.

Before performing this task [Add the Template to a
Process](Add%20the%20Template%20to%20a%20Process%20IGUC.htm).

Once an IG Universal Connect template has been added to a Process,
access the [Process Template
Loop](../Integrate/Page_Desc/Process_Template_Loop.htm) page to view the
single loop Integrate added automatically to the Process and to edit the
Process Template Loop. The loop, called Parameters, has two fields to be
mapped: Name and Value.

The Name is the unique name for the parameter.

The Value is used whenever this parameter is identified on a posting
record, unless otherwise indicated by the Where clause used in the
process post (entered on the
<span style="font-style: italic;">Vertical</span> View on the [Process
Post](../Integrate/Page_Desc/Process_Post_H.htm) page).

In the View created in the data source, either manually or automatically
generated, add the parameter Name and Values to the Name and Value
columns.  

<span style="font-weight: bold;">NOTE</span>: A Process must be inactive
to configure its Process Template Loops.

To manually update the VIEW NAME and PRIMARY KEY COLUMN NAME for a
Process Template Loop:

1.  Select <span style="font-weight: bold;">Categories</span> from
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    the category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a Process.

4.  Click the <span style="font-weight: bold;">Loops</span> icon for the
    template.
    
    <span style="font-weight: bold;">NOTE</span>: The
    <span style="font-style: italic;">[Process Template
    Loop](../Integrate/Page_Desc/Process_Template_Loop.htm)</span> page
    displays one loop that Integrate created automatically with the LOOP
    NAME “Parameter.”  The VIEW NAME and PRIMARY KEY COLUMN NAME fields
    are blank.

5.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Process Template Loop
    page.](../Integrate/Page_Desc/Process_Template_Loop.htm)

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

Continue with [Configure Field Mappings for an IG Universal Connect
Process
Template](Configure%20Field%20Mappings%20for%20an%20IG%20Universal%20Connect%20Template.htm).
