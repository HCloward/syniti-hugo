# Activate the Template

After creating a template, a Template Administrator must activate the
template before it can be used for posting a request.

A template cannot be activated if:

  - It has not been generated.
    
    **NOTE**: Until the template has been generated, the
    ACTIVATE/DEACTIVATE button is disabled. Generate a template on the
    Vertical View of the Templates page on the General tab. For
    non-custom templates, click Generate. For custom templates, click
    Generate Custom.

<!-- end list -->

  - Role dependencies have not been set up for all of the template
    roles.
    
    **NOTE**: When the Template Administrator clicks the Activate button
    on the Templates page, dspCompose™ validates the role dependencies
    for the template. Each role assigned to the template must either be
    dependent on another role assigned to the template, or must have a
    dependency on another role assigned to the template.

<!-- end list -->

  - No columns in the spreadsheet have been mapped to the template
    columns on the Template (External Request Scenario Column) page if
    the template uses an external request scenario that creates
    Excel-initiated requests. Refer to [Map Columns from the Template to
    Columns from the
    Spreadsheet](../../../Migration/Map/Use_Cases/Map_Columns_Template_to_Sprdsht.htm)
     for more information.

To activate a template:

1.  Click **Team** in *Navigation* pane.
2.  Click **Templates** for a team.
3.  Click **ACTIVATE/DEACTIVATE** for a template.

**NOTE**: If a template is active, a green icon displays and the ACTIVE
column contains a check mark. If the template is inactive, a red icon
displays and the ACTIVE column is blank.

**NOTE**: A warning message may display: “No archive page ID has been
set for this Template. Users will not be able to access the Archived
records via the WebApp until a value is set." If necessary, set the
archive page ID on the Templates page’s Vertical View on the Advanced
tab.

**NOTE**: An active template cannot be modified.

**NOTE**: Once a template has been activated and there are active
requests for the template, it cannot be deactivated. To make changes to
template configuration, either finish the requests and deactivate the
template, [Modify an Active Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode.htm), or delete all
requests for the template (on the Templates page’s Vertical View, on the
Advanced tab, click Delete All Requests).
