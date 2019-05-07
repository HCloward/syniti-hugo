+++
title = 'Validate a Role'
solution = 'Data Quality'
+++

# Validate a Role

**NOTE:** The **Validate** button, which is used to validate a role
(i.e., run a series of registered validation rules) will only be visible
for the Data and Review roles on the
<span style="font-style: italic;">Request (Roles)</span> page when role
validations have been registered to the template or when column
properties have been added to the Data Entry page for the template,
thereby triggering the use of the validation rules. Refer to [Add
Validations to Roles](Add_Validations_to_Roles.htm) and [Enable Role
Validations](../Config/Enable_Role_Validations.htm) for more
information.

Validations allow for template-specific data standards to be applied at
the role level. dspCompose™ runs validations registered for roles when a
user with that role enters a record for the request, or when a user
clicks Validate for a role on the *Request (Roles)* page. dspCompose™
runs validations against records that have not been posted or have been
posted unsuccessfully for the selected request role.

In addition to setting role validations, a user can:

  - Import validations from the registered page
  - Register validations from any pages in any component

If a user clicks **Validate** on the *Request (Roles)* page and there
are validation errors, a message displays. What happens next depends on
how the Prevent Finish Severity option is configured at the role level.
When an option is selected in the Prevent Finish Severity list box,
dspCompose™ will prevent a role from finishing if, during processing, a
validation fails that matches the selected or higher severity level.
Values are:

  - **Error** – Marks the role status as
    <span style="font-style: italic;">invalid</span> until the error is
    corrected and the Validation Rule passes.
  - **Message** – Marks the role status as
    <span style="font-style: italic;">valid</span> but a message
    displays.
  - **Warning** – Displays a message but the user can proceed with the
    task even if the validation fails.

If an option is not selected from the Prevent Finish Severity list box,
a warning displays if there is a validation error, but the role can be
finished. The Prevent Finish Severity is set on the *Vertical* View of
the *Template (Role)* page on the Approve and Finish Settings tab.

When a request record fails a validation check, dspCompose™ displays a
validation error message to help users troubleshoot the problem with the
data. Each validation error message displays on the
dspCompose™-generated *Data Entry*, *Comparison Approval*, and
*Request (Role Validation Failure)* pages. Validation error messages
also display in the Excel files dspCompose™ generates for request data
entry.

The error message displays the number of each validation failure type
with a link to the *Request (Roles - Validations*) page. On this page,
the user can see all of the validation failures for the keys on the
underlying page.

**NOTE:** The number of validation errors can be used by the Force
Reject Severity option set at the global level as a parameter. If an
option is selected from the Force Reject Severity list box on the
Parameters page on the Template tab, dspCompose™ rejects data entry
records that fail a validation whose severity meets or exceeds the Force
Reject Severity. These records cannot be approved by the Review role and
are automatically rejected and sent back to the Data role for
correction. Refer to [Set Force Reject
Severity](Set_Force_Reject_Severity.htm) for more information.

Set role-level and page-level validations on the *Template (Role
Validations)* page.

Refer to [Add Validations to Roles](Add_Validations_to_Roles.htm) for
more information.

To validate a role:

1.  Select **Requests** in the *Navigation* pane.

2.  Click **Roles** for a request.
    
    <span style="font-weight: bold;font-size: 11.0pt;">NOTE:</span> The
    count on the Roles icon is the number of roles the current user can
    access, not the total number of roles for the request.

3.  Click **Validate** for a role.

<span style="font-weight: bold;">NOTE:</span> The Validate button is not
available for the Post role.

<span style="font-weight: bold;">NOTE:</span> If a user clicks the
Validate button on the <span style="font-style: italic;">Request
(Roles</span>) page, only records for which the user has permission are
validated. If there are validation failures, the count that displays on
the Failures icon reflects all failures for all validating users. When
the user clicks the Failures icon to navigate to the
<span style="font-style: italic;">Request (Roles – Validations)</span>
page, the user only sees their validation failures.
