# Set Force Reject Severity

When a user clicks **Validate** on the *Request (Roles)* page for a Data
or a Review role, the request data is validated for that role. The types
of validations that run depend on how dspCompose™ is configured. Refer
to [Add Validations to Roles](Add_Role_Dependencies.htm) for more
information.

<span style="font-weight: bold;">NOTE:</span> The Validate button
displays on the <span style="font-style: italic;">Request (Roles)</span>
page if Role validations have been added to the request's template.

If there are validation errors, the severity of those errors can be used
by the Force Reject Severity option to prevent a Reviewer from approving
a role.

If the Force Reject Severity option is set, dspCompose™ rejects data
entry records that fail a validation whose severity meets or exceeds the
selected Force Reject Severity (Message, Warning, or Error). These
records cannot be approved by the Review role and are automatically
rejected and sent back to the Data role for correction. If no Force
Reject Severity is set, all data entry records can be rejected or
approved by Review role users.

For example, the **Force Reject Severity** is set to **Warning** for a
template. A user validates a role for a request based on that template,
which results in a validation error with a severity of
**Warning<span style="font-weight: normal;">.</span>** dspCompose™
automatically rejects the request. The Review role cannot approve it,
and the Data role must correct the request data.

The value can be set globally at the parameter level and can be
overwritten at the template level.

To set the Force Reject Severity on the
<span style="font-style: italic;">Parameters</span> page:

1.  Click **Configuration \> Parameters** on the *Navigation* pane.

2.  Click the **Template** tab.

3.  Click **Edit**.
    
    *[View the field descriptions for the Parameters
    page.](../Page_Desc/Parameters.htm)*

4.  Select an option in the **Force Reject Severity** list box.
    
    Values are:
    
      - **Error** – Marks the status as invalid until the error is
        corrected and the Validation Rule passes.
    
      - **Message** – Marks the status as valid but a message displays.
    
      - **Warning** – Displays a message but the user can proceed with
        the task even if the validation fails.

5.  Click **Save**.

To set the Force Reject Severity for a template:

1.  Select **Team** on the *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **Vertical View** for a template.

4.  Click the **Advanced** tab.

5.  Click **Edit**.
    
    *[View the field descriptions for the Templates page’s Vertical
    View.](../Page_Desc/Templates_H.htm#Templates_V_All_Tabs)*

6.  Select an option in the **Force Reject Severity** list box.
    
    Values are:
    
      - **Error** – Marks the status as invalid until the error is
        corrected and the Validation Rule passes.
    
      - **Message** – Marks the status as valid but a message displays.
    
      - **Warning** – Displays a message but the user can proceed with
        the task even if the validation fails.

7.  Click **Save**.
