+++
title = 'Configure a Process Template Loop for an IG Universal Connect Process Template Automatically'
solution = 'Platform'
+++

# Configure a Process Template Loop for an IG Universal Connect Process Template Automatically

Follow these steps if using parameters, which are optional.

A Process Template Loop assigns a view from the Process’s data source to
a loop within the template. The loop is mapped to a view which contains
the data to post for the corresponding template loop in the Process. In
the case of IG Universal Connect Templates, the data is parameter names
and values that are used as inputs to a Boomi Process.

The view that stores these fields and the field mappings can be created
manually. Refer to [Create a View in SQL
Server](../Integrate/Use_Cases/Create_a_View_in_SQL_Server) for more
information.

The view can also be generated automatically. Refer to [Generate
Database Objects
Automatically](../Integrate/Use_Cases/Generate_Database_Objects_Automatically)
for more information.

A process template loop can be configured manually or automatically.
Refer to [Configure a Process Template Loop for an IG Universal Connect
Process Template
Manually](Configure%20a%20Process%20Template%20Loop%20for%20an%20IG%20Universal%20Connect%20Process%20Template%20Manually)
for more information.

Before performing this task [Add the Template to a
Process](Add%20the%20Template%20to%20a%20Process%20IGUC) but
<span style="font-weight: bold;">do not select a View Name</span>.

The parameter name is a unique name for the parameter. The value is used
whenever this parameter is identified on a posting record, unless
otherwise indicated by the Where clause used in the Process post
(entered on the <span style="font-style: italic;">Vertical</span> View
on the <span style="font-style: italic;">[Process
Post](../Integrate/Page_Desc/Process_Post_H)</span> page).

<span style="font-weight: bold;">NOTE</span>: A process must be inactive
to configure its Process Template Loops.

To configure the Process Template Loop using the Auto Generate Database
Objects feature:

1.  Select <span style="font-weight: bold;">Categories</span> from
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    the category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a Process.

4.  Click the <span style="font-weight: bold;">Loops</span> icon for the
    template.

5.  Click <span style="font-weight: bold;">Auto Generate Database
    Objects.</span>
    
    <span style="font-weight: bold;">NOTE</span>: Auto Generate Database
    Objects create tables and views in the designated database for the
    Process Template Loop. Integrate creates a view with the name
    tx\[Process Name\] \_{Template Name}\_{LoopName}Int and creates a
    table with the name tt\[Process Name\]\_ \[Template
    Name\]\_{LoopName}\_Upload.  
    The feature also:

<!-- end list -->

  - Populates the VIEW NAME field in Integrate with \[Process Name\]
    \[Template Name\]
  - Sets the PRIMARY KEY COLUMN NAME to ID
  - Automatically maps the fields for the Process Template Loop. The
    TEMPLATE FIELD UNIQUE NAME and the MAPPING VALUE column have the
    same value.

Continue with [Configure Field Mappings for an IG Universal Connect
Process
Template.](Configure%20Field%20Mappings%20for%20an%20IG%20Universal%20Connect%20Template)
