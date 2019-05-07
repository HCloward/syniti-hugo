+++
title = 'Configure Field Mappings for a Process based on a GUI Script Template'
solution = 'Platform'
+++

# Configure Field Mappings for a Process based on a GUI Script Template

<span id="Post Data using a GUI Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

The field mappings for process template loops can be created
automatically using the Auto Generated Database Object feature. In this
case, the <span style="font-weight: bold;">MAPPING VALUE</span> field
and the <span style="font-weight: bold;">TEMPLATE FIELD UNIQUE
NAME</span> field will have identical values. Refer to [Generate
Database Objects
Automatically](Generate_Database_Objects_Automatically.htm) for more
information.

Once the process template loop is configured, configure the field
mappings for each loop level

When a template is added to a process, Integrate automatically creates
loop levels based on the template. Each loop level of the template has a
view mapped to it which contains the data to post for the corresponding
template loop level for the process.

A process template loop field mapping provides the link between a field
on a template and a column in a view. Each field on the template can be
mapped to a view, be assigned a fixed value or be ignored.

Once a view is registered to the process template loop, Integrate
compares the column in that view with the field names in the process
template loop and automatically maps them if possible. If the fields in
the view are named with valid SAP fields names, Integrate completes the
mapping automatically based on the fields in the recording.

Synchronous templates also allow mappings to be tied to Return Values.
Refer to [Post Data Using Transaction
Stringing](Post_Data_Using_Transaction_Stringing.htm) for more
information.

**NOTE**: Template Process Loop Field Mappings cannot be edited if the
process is active.

**NOTE**: Field mappings automatically update to reflect a change in a
process template loop’s view. For example, a user creates a process and
selects a view name in the **View Name** list box on the *Process*
page’s *Vertical* View on the **General** tab. When the process is
saved, Integrate automatically maps the fields according to this view on
the *Process Template Loop Field Mappings* page. If the user then
updates the view name in the **VIEW NAME** list box on the *Process
Template Loop* page, the Field Mappings are reset to reflect the columns
in the updated view. If the process was created using the Auto Generate
Database Object feature, updates to the **VIEW NAME** on the *Process
Template Loop* page are also reflected in the field mappings on the
*Process Template Loop Field Mappings* page.

To configure field mapping manually for a GUI Script process template:

1.  Select **Categories** from *Navigation pane*.

2.  Click the **Processes** icon for the category.

3.  Click the **Templates** icon for the process.

4.  Click the **Loops** icon for the process template.
    
    **NOTE**: The number displays the number of loops.

5.  Click **Fields Mappings** for a loop level on the *Process Template
    Loops* page.

6.  Click **Edit**.
    
    *[View the field descriptions for the Process Template Loop Field
    Mappings
    page.](../Page_Desc/Process_Template_Loop_Field_Mappings_H.htm)*

7.  Locate a **TEMPLATE FIELD UNIQUE NAME** to configure.  
    Either:
    
    Select a value from **Mapping Value** list box.
    
    **NOTE**: This value is a column in the database view.
    
    OR
    
    Enter a value in **FIXED VALUE** field.
    
    **NOTE**: A fixed value is a hard coded value sent during each
    posting process. It is read from the registration and not from the
    database. 
    
    **NOTE:**To ignore a field during a post, leave both **MAPPING
    VALUE** and **FIXED VALUE** fields blank.
    
    **NOTE:** If a mapping value is set but the value in the database is
    NULL, then Integrate will not include the field in the posting.

8.  Click **Save**.
