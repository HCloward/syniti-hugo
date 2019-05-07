+++
title = 'Set the Current User as the External Role Contact'
solution = 'Data Quality'
+++

# Set the Current User as the External Role Contact

When creating an external request scenario, a user configures a template
to use emails received from designated external contacts to create a
request via email. The user can also designate that dspCompose™:

  - Sends an email to the current user to initiate the email creation
    process and

  - Accepts email from the current user when processing the external
    request scenario for the current request.

In some cases, a user who sends an email to create a request with
external roles should also be the recipient of one or many of those
external roles. To simplify this process, one or several of the external
roles can be configured to use the sender's email address as the
external role contact information for a request created via email.

The *Template (External Request Scenario External Role)* page has a
column named **USE SENDER EMAIL ADDRESS**. When the check box is
enabled, the current user, (i.e., the sender), is also the recipient of
emails as an external role for the request.

Using this process simplifies setting up external contacts for an
external request scenario. The current user will:

  - Receive an email from dspCompose™ to inform the external contact to
    initiate the email creation process and

  - Send email to dspCompose™ when processing the external request
    scenario for the current request.

**NOTE:** If the **USE SENDER EMAIL ADDRESS** check box is enabled, a
validation checks to ensure that other email values on the record,
stored in the **RECIPIENT EMAIL ADDRESS** column, are cleared. If the
check box is disabled, a validation checks to ensure that the
**RECIPIENT EMAIL ADDRESS** column contains a valid email address. The
email address must contain a period (.) and an "at" sign (@) in order to
be valid.

**NOTE:** The **LANGUAGE ID** column can be used to set the language of
the message sent to the sender's email address. If no **LANGUAGE ID** is
selected, then English is used. <span>Language-specific messages are
added on the *Workflow Message* page and the *Workflow Language Message*
page.</span>

To allow the sending user to receive emails for the external request
scenario:

1.  Click **Team** on *Navigation* pane.
2.  Click **Templates** for a team.
3.  Click **Vertical View** for a template.
4.  Click **Configuration** tab.
5.  Click **External Request Scenarios**.
6.  Click **External Roles** for a scenario.
7.  Click the **USE SENDER EMAIL ADDRESS** check box to enable it.
