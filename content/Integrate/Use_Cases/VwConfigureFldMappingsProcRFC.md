+++
title = 'View and Configure Field Mappings for a Process Based on an RFC'
solution = 'Platform'
+++

# View and Configure Field Mappings for a Process Based on an RFC

<span id="Post Data using an RFC Steps" class="popUpLink">\>Review the
steps in the process. </span>

Field Mappings can be performed by Integrate’s Auto Generate Database
Object feature or can be configured manually.

Integrate’s Auto Generate Database Objects feature maps the fields for
each process template loop. The **MAPPING VALUE** is identical to the
**TEMPLATE FIELD UNIQUE NAME**.

When mapping fields for a process template based on a BAPI template,
both Upload and Download field mappings are possible.  Use filter
buttons in the toolbar to quickly filter on **All Fields**, only
**Upload** Fields, or only **Download** Fields. 

**NOTE:** Field mappings automatically update to reflect a change in a
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

To view field mappings and edit them manually if necessary:

1.  Click the **Field Mappings** icon for a loop.

2.  Click **Upload Fields**, **Download Fields**, or **All Fields** to
    apply a filter if necessary.
    
    **NOTE:** If no Upload fields exist, the **Upload Fields** button
    does not display. If no Download fields exist, the **Download
    Fields** button does not display.

3.  Click **Edit** for a field.
    
    *[View the field descriptions for the Process Template Loop Field
    Mappings
    page.](../Page_Desc/Process_Template_Loop_Field_Mappings_H)*

4.  Update **the MAPPING VALUE** or **FIXED VALUE** field.
    
    **NOTE:** Both fields cannot contain data for a Field Mapping.

5.  Click **Save**.
