# Create Language-specific Workflow Email Templates

Workflow templates can be created that take a user’s language setting
into account. The language for a user is set by an Administrator when
creating user accounts.

If no language is set for a template, the default language is used.

If a user does not have a language specified, the default site language
is used.

A user can add multiple versions of templates at the parameter, project
and project distribution levels, one for each language.

To add a language-specific template at the parameters page:

1.  Select <span style="font-weight: bold;">Information Steward
    Accelerator \></span>**Configuration \> Parameters** in the
    *Navigation* pane.

2.  Click the **Attachment Settings** tab or **Summary Settings** tab.

3.  Click **Attachment Workflow Translation** or **Summary Workflow
    Translation.**

4.  Click <span style="font-weight: bold;">Add</span>.
    
    *[View the field descriptions for the Workflow Template
    page.](../Page_Desc/Workflow_Template)*

5.  Select the language that will be used for the email message that
    includes an attachment from the **LANGUAGE ID** field.
    
    **NOTE:** A user will receive an email with this translation when
    the user’s language ID setting matches the language selected in the
    LANGUAGE ID field.

6.  Enter text in the specified language that will appear in the subject
    of the email in the **SUBJECT** field.
    
    **NOTE:** A value preceded and followed by \# is a dynamic
    substitution value for replacement at run time. For example, the
    \#NAME\# field will be replaced with the user name of the user
    receiving the workflow email.
    
    **NOTE:** The available replacements for Summary emails are
    \#CURRENTDATE\#, \#NAME\#, \#SUMMARYTABLE\#, though only
    \#CURRENTDATE\# and \#NAME\# are available for Summary email subject
    lines. The available replacements for Attachment emails are
    \#PROJECT\#, \#DISTRIBUTION\#, \#CURRENTDATE\#, \#NAME\#,
    \#OWNERNAME\#, \#OWNERPHONE\#, \#OWNEREMAIL\#, \#SUMMARYTABLE\#,
    \#SCORECARDLINK\#, though only \#PROJECT\# and \#DISTRIBUTION\# are
    available for Attachment email subject lines.

7.  Enter text in the specified language that will appear in the body of
    the email as needed in the **BODY** field.

8.  Click **Save**.

9.  Follow these steps at the project and project distribution levels to
    add language-specific workflow emails.
