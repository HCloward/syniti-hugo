# Configure Field Mappings for an IG Universal Connect Template

Follow these steps if using parameters, which are optional.

Before completing this task, Configure a Process Template Loop for an
IG Universal Connect Process Template
[Manually](Configure%20a%20Process%20Template%20Loop%20for%20an%20IG%20Universal%20Connect%20Process%20Template%20Manually.htm)
or
[Automatically](Configure%20a%20Process%20Template%20Loop%20for%20an%20IG%20Universal%20Connect%20Process%20Template%20Automatically.htm).

For parameters to be used as inputs for a Boomi Process, a view must be
created in SQL Server. The view serves as the basis of Process Template
Loop Field Mappings, which connect a column in a view with a field on a
Template.

A user can create the view using the Auto Generate Database Objects
feature. Refer to [Generate Database Objects
Automatically](../Integrate/Use_Cases/Generate_Database_Objects_Automatically.htm)
for more information. Views can also be created manually. Refer to
[Create a View in SQL
Server](../Integrate/Use_Cases/Create_a_View_in_SQL_Server.htm) for more
information.

A Process Template Loop field mapping provides the link between a field
on a template and a column in a view. Each field on the template can be
mapped to a column in a view, be assigned a fixed value, or be ignored.

Once a view is registered to the Process Template Loop, Integrate
compares the column in that view with the field names in the process
template loop and automatically maps them if possible. If the fields in
the view are named with valid SAP fields names, Integrate completes the
mapping automatically.

<span style="font-weight: bold;">NOTE</span>: Template Process Loop
Field Mappings cannot be edited if the Process is active.

To configure field mapping manually for an IG Universal Connect Process
template:

1.  Select <span style="font-weight: bold;">Categories</span> from
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    the category.

3.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a Process.

4.  Click the <span style="font-weight: bold;">Loops</span> icon for the
    template.

5.  Click the <span style="font-weight: bold;">Fields Mappings</span>
    icon for a loop level.

6.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Process Template Loop Field
    Mappings
    page](../Integrate/Page_Desc/Process_Template_Loop_Field_Mappings_H.htm)
    
    <span style="font-weight: bold;">NOTE</span>: An error message
    displays if a View is not defined on the
    <span style="font-style: italic;">[Process Template
    Loop](../Integrate/Page_Desc/Process_Template_Loop.htm)</span> page.

7.  For the Name and Value field, either:
    
    Select a value from the <span style="font-weight: bold;">MAPPING
    VALUE</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: This value is a column
    in the database view.
    
    Or
    
    Enter a value in <span style="font-weight: bold;">FIXED VALUE</span>
    field.
    
    <span style="font-weight: bold;">NOTE</span>: A fixed value is a
    hard coded value sent during each posting process. It is read from
    the registration and not from the database.
    
    <span style="font-weight: bold;">NOTE</span>: If a mapping value is
    set but the value in the database is NULL, then Integrate will not
    include the field in the posting.

8.  Click <span style="font-weight: bold;">Save</span>.

Continue with [Activate the
Process](Activate%20the%20Process%20IGUC.htm).
