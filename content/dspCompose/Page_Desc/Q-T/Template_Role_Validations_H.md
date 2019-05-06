# Template (Role Validations) H

[Template (Role Validations) V](#Template_Role1)

<div class="use">

Use this page to [Add Validations to
Roles](../Use_Cases/Add_Validations_to_Roles.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspCompose \>
    Team</span> on *Navigation *pane.
2.  Click <span style="font-weight: bold;">Templates</span> for a team.
3.  Click <span style="font-weight: bold;">Roles</span> for a template.
4.  Click <span style="font-weight: bold;">Validations</span> for a
    role.

|                         |                                                                                                                                                                                                                                                                                                                                                                                 |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                   | Description                                                                                                                                                                                                                                                                                                                                                                     |
| Refresh All Validations | Click to refresh all validation registrations from the PageID (and all child pages) registered to the Template-Role, and mark them as system-generated. In other words, if the page that is associated with the Role has any validation registrations, these validations will be automatically added to this page and can be activated or deactivated to be used with the role. |
| PRIORITY                | Displays order in which the validation rule is run against the data.                                                                                                                                                                                                                                                                                                            |
| RULE                    | Displays name of the validation rule.                                                                                                                                                                                                                                                                                                                                           |
| ACTIVE                  | If enabled, the role validation rule is active. Only active validation rules are run for the role.                                                                                                                                                                                                                                                                              |
| ACTIVATE/DEACTIVATE     | Click to activate or deactivate the validation rule. Only active validation rules are run for the role.                                                                                                                                                                                                                                                                         |
| SYSTEM VALIDATION       | If enabled, the validation is system-generated.                                                                                                                                                                                                                                                                                                                                 |

## <span id="Template_Role1"></span>Template (Role Validations) V

[Template (Role Validations) H](Template_Role_Validations_H.htm)

Field

Description

Run Order

Priority

Displays order in which the validation rule is run against the data.

Page Validation Rule

Web App ID

Displays WebApp that contains the page where the validation rule is
registered.

Page ID

Displays the name of the page where the validation rule is registered.

Object Name

Displays the name of the validation rule registered on the page to run
against data for the template role.

Role Level Validation

Data Source ID

Displays name of the data source that contains the validation rule.

Role Object Name

Displays the name of the validation rule to run against data for the
template-role.

Validation

Severity

Displays severity of validation rule. Values are:

  - <span style="font-weight: bold;">Error</span> – Marks the role
    status as <span style="font-style: italic;">invalid</span> until the
    error is corrected and the validation rule passes
  - <span style="font-weight: bold;">Message</span> – Marks the role
    status as <span style="font-style: italic;">invalid</span>, but
    displays a message
  - <span style="font-weight: bold;">Warning</span> – Displays a message
    but the user can proceed with the task even if the validation fails.

Comment

Displays text seen by end user, indicating the error.
