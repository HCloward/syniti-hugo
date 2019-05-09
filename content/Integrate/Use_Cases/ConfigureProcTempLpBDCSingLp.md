+++
title = 'Configure a Process Template Loop for a BDC Script Template with a Single Loop'
solution = 'Platform'
+++

# Configure a Process Template Loop for a BDC Script Template with a Single Loop

<span id="Post Data using a BDC Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

A process template loop assigns a view from the process’s data source to
a loop within the template. The loop is mapped to a view which contains
the data to post for the corresponding template loop in the process.

Once a BDC Script template with a single loop has been added to a
process, access the *Process Template Loop* page to view the loop
Integrate added automatically to the process and to edit the process
template loop. The loop contains a View Name, a Primary Key Column Name
(which Integrate uses to automatically map the columns from the view to
the fields in the template), and Field Mappings.

A process template loop for a BDC Script template that does not have
looping enabled can be configured manually or can be automatically
configured using the Auto Generate Database Objects feature.

Integrate automatically adds a single process template loop to the
process when the template is added to the process. Integrate uses the
View Name established for the template during process creation as the
View Name for this loop. If possible, Integrate automatically creates
the Primary Key Column Name based on the column that uniquely identifies
the record in the view. The Loop Name is blank.

**NOTE**: If using the Auto Generate Database Objects feature, do not
select a view name when adding the process that will be associated with
the BDC Script template with a single loop. Refer to [Generate Database
Objects Automatically](Generate_Database_Objects_Automatically) for
more information.

Assign specific columns in the view to unique template fields using
field mappings or generate them automatically using the Auto Generate
Database Objects feature. Refer to [Configure Field Mappings for a
Process Based on a BDC Script
Template](ConfigureFieldMappingsBDC_Script_Template)  for more
information.

**NOTE**: A process must be inactive to configure its process template
loops.

To view process template loops:

1.  Select **Categories** from *Navigation pane*.

2.  Click the **Processes** icon for the category.

3.  Click the **Templates** icon for a process.

4.  Click the **Loops** icon for the template.
    
    <span style="font-family: Arial, sans-serif;">**NOTE**: The number
    displays the number of</span> loops.

The *Process Template Loop* page displays one loop only and the **LOOP
NAME** for this record is blank.

The **VIEW NAME** and **PRIMARY KEY COLUMN NAME** may be updated
manually for each loop level. The view must already exist in the data
source assigned to the process.

To manually update the **VIEW NAME** and **PRIMARY KEY COLUMN NAME** for
a process template loop:

1.  On the *Process Template Loop* page, click **Edit** for a loop.
    
    *[View the field descriptions for the Process Template Loop
    page.](../Page_Desc/Process_Template_Loop)*

2.  Select a name in the **VIEW NAME** list box.
    
    **NOTE**: The view must already exist in the data source to be
    available in the list box.

3.  Select a name in the **PRIMARY KEY COLUMN NAME** list box.
    
    **NOTE**: The list box displays all columns available in the view.
    The column selected must uniquely identify a record in the view.

4.  Click **Save**.

To configure the process template loop using the Auto Generate Database
Objects feature:

1.  Create a process and add the template to it, but do not select a
    view name.

2.  Navigate to the *Process Template Loop* page.

3.  Click **Auto Generate Database Objects**.
    
    **NOTE**: Auto Generate Database Objects create stables and views in
    the designated database for the process template loop. Integrate
    creates a view with the name tx\[Process Name\] {Template Name}Int
    and creates a table with the name tt\[Process Name\] {Template
    Name\]\_Upload.  
    The feature also:
    
      - Populates the **VIEW NAME** field in Integrate with \[Process
        Name\] \[Template Name\]
      - Sets the **PRIMARY KEY COLUMN NAME** to ID
      - Automatically maps the fields for the process template loop. The
        **TEMPLATE FIELD UNIQUE NAME** and the **MAPPING VALUE** column
        will have the same value.

Refer to [Generate Database Objects
Automatically](Generate_Database_Objects_Automatically) for more
information.
