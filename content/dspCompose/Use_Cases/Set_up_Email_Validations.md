+++
title = 'Set up Email Validations'
solution = 'Data Quality'
+++

# Set up Email Validations

Using an external request scenario, an external contact can send an
email to the external data email account to:

  - Add a request
  - Create an Excel-initiated request

This topic contains the following sections:

  - [Validations](#Validations)
  - [Email Validations Included with
    dspCompose](#Email_Validations_Included_with_dspCompose)
  - [Edit Default Email Validations](#Edit_Default_Email_Validations)
  - [Add Custom Email Validations](#Add_Custom_Email_Validations)

## <span id="Validations"></span>Validations

Validations are stored procedures or views that have been written and
saved in a data source that is registered in the DSP®. A validation
executes when an event occurs, and confirms that a process is valid. If
the validation fails, processing stops. For example, a validation is
registered to a Receive Email event. The validation confirms that an
email received at a designated address has an attachment in a specified
format. If the attachment is in a valid format, the validation passes
and processing can continue. However, if the attachment is in an invalid
format, the validation fails, and processing stops.

Validations may have Severity of Error, Warning, Message, or Workflow
Only. If the validation Severity is set to Error and the validation
fails, processing stops and the event the validation was registered to
does not run.

**NOTE:** That message was entered in the Message field on the *[Email
Validation Message](../Page_Desc/Email_Validation_Message)* page.

dspCompose™ is delivered with multiple email
validations.

## <span id="Email_Validations_Included_with_dspCompose"></span>Email Validations Included with dspCompose

A Template Administrator can register email validations that are run on
emails received at the external data email account. These validations
reduce time needed for support by handling basic email validation
automatically.

When dspCompose™ is installed, it is automatically configured to run
email validations to check that:

  - The message is a valid type ( i.e., the alias included in the
    subject line of the email matches the alias for an external request
    scenario)
  - The request role is active for an active request (for example, the
    External Data role has not been finished for the request)
  - The sender has permission to enter a request for the template (for
    example, the sender has been added as an External Contact for the
    external request scenario)
  - The template for the request is active

For external request scenarios that create Excel-initiated requests,
dspCompose™ also runs validations to check that:

  - The email has only one attachment
  - The email contains an attachment
  - The attachment is in .xls or .xlsx format
  - The sender has access to the template that is associated with the
    Excel file attached to the email
  - The template related to the Excel file attached to the email is
    active

When an External Contact for an external request scenario that creates
an Excel-initiated request submits an Excel file as an attachment to an
email, if any of the worksheets fail an email validation listed above,
none of the worksheets in the Excel file will be processed. The external
contact will receive a message from the first validation that fails. The
external contact must correct and resubmit the Excel
file.

## <span id="Edit_Default_Email_Validations"></span>Edit Default Email Validations

The Template Administrator can further configure each validation to:

  - Stop processing the validation and ignore the email on failure
  - Email the sender in the case of a failure

To edit the default email validations:

1.  Select **Configuration \> Email Validation** from the *Navigation*
    pane.

2.  Click the **CONTINUE ON FAILURE** check box to enable the validation
    process to continue if an email fails the validation. Clear the
    check box if the validation process should stop if an email fails
    the validation.

3.  Click the **EMAIL ON FAILURE** check box to enable it if dspCompose™
    should send an email to the sender when an email fails a validation.

4.  Click **Message** to view the text and language of the email message
    that dspCompose™ sends to the original sender.

5.  Click **Edit** to update the message text.
    
    [View the field descriptions for the Email Validation Message
    page.](../Page_Desc/Email_Validation_Message)

6.  Enter the text of the message for a language in the **MESSAGE**
    field.

7.  Click
**Save**.

## <span id="Add_Custom_Email_Validations"></span>Add Custom Email Validations

A Template Administrator can add custom email validations, in the form
of views or stored procedures, to validate inbound emails from External
Data roles. In the case of a stored procedure, the validation takes in
an EmailMessageID parameter. A view binds on an EmailMessageID.

The EmailMessageID value should correspond to a value in the table
ttEmailMessage.EmailMessageID. When dspCompose™ runs the validation, if
a view returns at least one record or a procedure returns 1 then the
validation fails.

To add a custom email validation:

1.  Select **Configuration \> Email Validation** from the *Navigation*
    pane.

2.  Click **Add**.
    
    *[View the field descriptions for the Email Validation
    page.](../Page_Desc/Email_Validation)*

3.  Enter a sort order in the **PRIORITY** field.
    
    **NOTE:** The priority determines the order in which the validations
    are run.

4.  Select a data source ID from the **DATA SOURCE ID** list box.
    
    **NOTE:** The data source contains the view or stored procedure that
    is the email validation.

5.  Select the validation from the **RULE** list box.
    
    **NOTE:** The validation is a view or a stored procedure from the
    data source.

6.  Enter a brief description of the validation in the **DESCRIPTION**
    field.

7.  Click the **CONTINUE ON FAILURE** check box to enable it if the
    process should continue after an email validation failure.

8.  Click the **EMAIL ON FAILURE** check box to enable it if dspCompose™
    should send an email to the sender with information about the
    failure.

9.  Click **Save**.

10. Click **Message**.

11. Click **Edit** next to the message’s language.
    
    [View the field descriptions for the Email Validation Message
    page](../Page_Desc/Email_Validation_Message)

12. Enter the text for the email validation failure error message in the
    **MESSAGE** field.

13. Click **Save**.
