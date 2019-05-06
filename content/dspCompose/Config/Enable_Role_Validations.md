# Enable Role Validations

Role Validations are based on a view in the database specified for the
template's data source. dspCompose™ automatically generates validations
for list boxes, check boxes and required fields for the data entry page
when the Data Entry role is validated.

These validations are set to run by default, but can be configured at
the global role level on the *Parameters* page, or at the template level
on the *Templates* page’s *Vertical* View on the **Advanced** tab.

Custom role validations can also be added on the *Template (Role
Validations)* page. Refer to [Add Validations to
Roles](../Use_Cases/Add_Validations_to_Roles.htm) for more information.

The **Validate** button automatically displays on the *Request (Roles)*
page for the Data role and the Review role if:

  - A list box, check box, or required column exists on the Data Entry
    page and the corresponding check box to run the validation is
    checked on the *Parameters* page
  - The Review role has the appropriate column properties set to display
    the list box, check box, or required column
  - A validation has been added to the role on the *Template (Role
    Validations)* page

A template is not required to have any validations. In this case, the
**Validate** button is hidden on the *Request (Roles)* page.

If a user clicks **Validate** on the *Request (Roles)* page and there
are validation errors, a message displays. What happens next depends on
how the Prevent Finish Severity option is configured at the role level.
When an option is selected in the **Prevent Finish Severity** list box,
dspCompose™ prevents a role from finishing if, during processing, a
validation fails that matches the selected or higher severity level.
Values are:

  - **Error –** Marks the role status as *invalid* until the error is
    corrected and the Validation Rule passes.
    
    **NOTE:** All role validations that are enabled on this page and on
    the *Template*page’s *Vertical* View on the Advanced tab fail with a
    severity of Error. Custom role validations can be configured to fail
    with other severity levels. Refer to [Add Validations to
    Roles](../Use_Cases/Add_Validations_to_Roles.htm) for more
    information.

  - **Message –** Marks the role status as *valid* but a message
    displays.

  - **Warning –** Displays a message but the user can proceed with the
    task even if the validation fails.

If a Prevent Finish Severity option is not selected, a warning displays
if there is a validation error, but the role can be finished.

Validation messages can be customized. Refer to [Update Validation
Messages](Update_Validation_Messages.htm)  for more information.

To enable role validations at the global level:

1.  Select **Configuration \> Parameters** on the *Navigation* pane.

2.  Click the **Template** tab.

3.  Click the **Enable List Box Validation** check box to enable it.
    
    **NOTE:** If checked, values entered on data entry pages that have
    list or combo boxes will be validated to ensure that values in the
    columns are contained in the list boxes assigned to the data entry
    pages. The validation takes **List Unique** (if a list box does not
    allows a user to add values) and **List Allow Insert** (if a list
    box does allow a user to add values) into account. Records that fail
    this validation will fail with a severity of Error.

4.  Click the **Enable Check Box Validation** check box to enable it.
    
    **NOTE:** If checked, values entered on data entry pages that have a
    Check Box column property defined will be validated to ensure that
    the values in the table correspond to the proper check box format
    set on the column property. Records that fail this validation will
    fail with a severity of Error.

5.  Click the **Enable Required Validation** check box to enable it.
    
    **NOTE:** If checked, values entered on data entry pages for
    Required fields with a data type of nvarchar are validated to ensure
    that all required columns have values entered. Records with blank
    required fields fail with a severity of Error.
    
    **NOTE:** Validations are not run on required fields with data types
    other than nvarchar.

To enable role validations at the template level:

1.  Click **Team** in the *Navigation* pane.
2.  Click **Templates** for a team.
3.  Click **Vertical View** for a template.
4.  Click the **Advanced** tab.
5.  Continue with step 3 above.
