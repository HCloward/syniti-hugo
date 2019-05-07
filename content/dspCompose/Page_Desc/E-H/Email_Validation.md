+++
title = 'Email Validation'
solution = 'Data Quality'
+++

# Email Validation

<div class="use">

Use this page to:

  - [Set Up Email
    Validations](../Use_Cases/Set_up_Email_Validations.htm)
  - [Add Custom Email Validation
    Rules](../Use_Cases/Set_up_Email_Validations.htm#Add_Custom_Email_Validations)

</div>

To access this page, select <span style="font-weight: bold;">dspCompose
\>
</span><span style="background: #ffffff;font-weight: bold;">Configuration
\> Email
Validation</span> from *<span style="background: #ffffff;">Navigation</span> *pane.

|                     |                                                                                                                                                                                   |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field               | Description                                                                                                                                                                       |
| PRIORITY            | Displays order in which the email validation rule is run.                                                                                                                         |
| DATA SOURCE ID      | Displays data source that contains the view or stored procedure that is used for the email validation rule.                                                                       |
| RULE                | Displays rule used for the email validation. The rule is a view or stored procedure from the Data Source ID.                                                                      |
| DESCRIPTION         | Displays a brief description of the rule.                                                                                                                                         |
| CONTINUE ON FAILURE | If enabled, the validation process continues even if a validation rule fails for the email. If disabled, the validation process stops if the validation rule fails for the email. |
| EMAIL ON FAILURE    | If enabled, an email with the information about the failure is sent to the email sender if a validation rule fails for an email.                                                  |
| Message             | Click to open the Email Validation Message page to edit text of the email validation failure message for the specified language.                                                  |
