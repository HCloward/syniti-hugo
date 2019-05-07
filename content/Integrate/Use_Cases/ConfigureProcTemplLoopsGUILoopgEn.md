+++
title = 'Configure Process Template Loops for a GUI Script Template with Looping Enabled'
solution = 'Platform'
+++

# Configure Process Template Loops for a GUI Script Template with Looping Enabled

<span id="Post Data using a GUI Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

A process template loop assigns a view from the process’s data source to
a loop within the template. Each loop is mapped to a view which contains
the data to post for the corresponding template loop in the process.

Once a GUI Script template with looping enabled has been added to a
process, access the *Process Template Loop* page to view the loops
Integrate added automatically to the process, and to edit and exclude
process template loops. Each loop contains a Loop Name, a View Name, a
Primary Key Column Name (which Integrate uses to automatically map the
columns from the view to the fields in the template), and Field
Mappings.

Integrate  can either create a View and Primary Key Column Name for each
loop automatically using the Auto Generate Database Objects feature, or
a user can assign a View and Primary Key Column Name manually based on
views already created in the data source. Each loop must be mapped to a
separate view.

**NOTE**: If using the Auto Generate Database Objects feature, do not
select a view name when adding the process that will be associated with
the GUI Script template. Refer to [Generate Database Objects
Automatically](Generate_Database_Objects_Automatically.htm) for more
information.

Assign specific columns in the view to unique template fields using
field mappings or generate them automatically using the Auto Generate
Database Objects feature. Refer to[Configure Field Mappings for a
Process based on a GUI Script
Template](ConfigureFieldMappingsGUI_Script_Template.htm)<span style="color: #000000;">for
more information.</span>

If the process is based on a GUI template with multiple loops,
relationships must be established to link the views assigned to
different loops.  A user can set up relationships manually or can use
the Auto Generate Database Objects feature to create them automatically.
Refer to [View and Configure Relationships for a Process Based on a GUI
Script Template](VwConfigureRelshpsGUIe.htm) for more
information.

**N<span style="font-family: Arial, sans-serif;">OTE</span>**<span style="font-family: Arial, sans-serif;">:
A process based on a GUI template with multiple loops requires
relationships between loops be established. Relationships map values in
parent views to values in child views to link views assigned to
different loops. Refer to [View and Configure Relationships for a
Process Based on a GUI Script Template](VwConfigureRelshpsGUIe.htm) for
more information.</span>

**NOTE**: A process must be inactive to configure its process template
loops.

To view process template loops:

1.  Select **Categories** from *Navigation pane*.

2.  Click the **Processes** icon for the category.

3.  Click the **Templates** icon for a process.

4.  Click the **Loops** icon for the template.
    
    **NOTE**: The number displays the number of loops.
    
    *[View the field descriptions for the Process Template Loop
    page.](../Page_Desc/Process_Template_Loop.htm)*
    
    <span style="font-weight: bold;">NOTE</span>: The **VIEW NAME** and
    **PRIMARY KEY COLUMN NAME** may be updated manually for each loop
    level. The view must already exist in the data source assigned to
    the process.

5.  Click **Edit** for a loop.
    
    *[View the field descriptions for the Process Template Loop
    page.](../Page_Desc/Process_Template_Loop.htm)*

6.  Select a name in the **VIEW NAME** list box.
    
    **NOTE**: The view must already exist in the data source to be
    available in the list box.

7.  Select a name in the **PRIMARY KEY COLUMN NAME** list box.
    
    **NOTE**: The list box displays all columns available in the view.
    The column selected must uniquely identify a record in the view.

8.  Click **Save**.

To configure the process template loop using the Auto Generate Database
Objects feature:

1.  Create a process and add the template to it, but do not select a
    view name.

2.  Navigate to the *Process Template Loop* page.

3.  Click **Auto Generate Database Objects**.
    
    **NOTE**: Auto Generate Database Objects create stables and views in
    the designated database for the process template loops. Integrate
    creates each view with the name tx\[Process Name\] {Template
    Name}Int and creates each table with the name tt\[Process Name\]
    {Template Name\]\_Upload.
    
    The feature also:
    
      - Populates the **VIEW NAME** field in Integrate with \[Process
        Name\] \[Template Name\]
      - Sets the **PRIMARY KEY COLUMN NAME** to **ID**
      - Automatically maps the fields for the process template loops.
        The **TEMPLATE FIELD UNIQUENAME** and the **MAPPING VALUE**
        column will have the same value
      - Configures relationships for process template loops

Refer to [Generate Database Objects
Automatically](Generate_Database_Objects_Automatically.htm) for more
information.
