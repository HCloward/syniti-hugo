# Configure Workflow Templates at the Parameter Level

Workflow emails are sent to users that contain reports about data that
failed IS rules. 

When the ISA applies templates, a user’s project distribution-level
template is applied by default. If no project distribution-level
template exists, the project template is applied. If no project-level
template exists, the parameter-level template is applied to the user’s
workflow template.

The types of templates for workflows that can be configured at the
parameter level are:

  - A generic template for attachment emails set at the parameter level
  - A generic template set for summary emails at the parameter level

**NOTE**: Templates for attachment emails can also be added at the
[project](Configure_Workflow_Templates_at_the_Project__Level) or
[project
distribution](Configure_Workflow_Templates_at_the_Project_Distribution_Level)
levels. A template for summary emails can only be set at the parameter
level.

**NOTE**: Summary workflows are sent at the user level only. Summary
emails will not be sent to all users in a project distribution, unless
all users in that project distribution have selected to receive
summaries as a workflow option.

The workflow template a user receives depends on whether that user
belongs to a  project distribution that has a template assigned. If a
template is configured at the project distribution  level, all users in
the project distribution will receive emails based on the project
distribution template. If a template is not configured at the project
distribution level, but is configured at the project level, users in the
project distribution will receive emails based on the project template.

To configure generic workflow templates at the parameter level:

1.  Select <span style="font-weight: bold;">Information Steward
    Accelerator \></span>**Configuration \> Parameters** in the
    *Navigation* pane.

2.  Click the **Attachment Settings** tab.

3.  Click **Attachment Workflow Translation**.

4.  Click **Edit**.
    
    *[View the field descriptions for the Workflow Template
    page.](../Page_Desc/Workflow_Template)*

5.  Select the language that will be used for the email message that
    includes an attachment from the **LANGUAGE ID** field. Refer to
    [Create Language-specific Workflow Email
    Templates](Create_Language%20specific_Workflow_Email_Templates)
    for more information.
    
    **NOTE:** Users can access the information on the report through an
    attachment, a summary, or links depending on the user’s workflow
    attachment options.  Refer to [Configure Workflow
    Options](Configure_Workflow_OptionsISA) for more information.

6.  Update the text that will appear in the subject of the email as
    needed in the **SUBJECT** field.
    
    **NOTE:** A value preceded and followed by \# is a dynamic
    substitution value for replacement at run time. For example, the
    \#NAME\# field will be replaced with the user name of the user
    receiving the workflow email. The available replacements for Summary
    emails are \#CURRENTDATE\#, \#NAME\#, \#SUMMARYTABLE\#, though only
    \#CURRENTDATE\# and \#NAME\# are available for Summary email subject
    lines.  The available replacements for Attachment emails are
    \#PROJECT\#, \#DISTRIBUTION\#, \#CURRENTDATE\#, \#NAME\#,
    \#OWNERNAME\#, \#OWNERPHONE\#, \#OWNEREMAIL\#, \#SUMMARYTABLE\#,
    \#SCORECARDLINK\#, though only \#PROJECT\# and \#DISTRIBUTION\# are
    available for Attachment email subject lines.

7.  Update the text that will appear in the body of the email as needed
    in the **BODY** field.
    
    **NOTE:** A value preceded and followed by \# is a dynamic
    substitution value for replacement at run time. For example, the
    \#NAME\# field will be replaced with the user name of the user
    receiving the workflow email.

8.  Click **Save**.

9.  Click the Back button on the browser to return to the *Parameters*
    page.

10. Click the **Summary Settings** tab.

11. **NOTE:** Users can access the information on the report through an
    attachment,a summary or links depending on the user’s workflow
    attachment options.  Refer to [Configure Workflow
    Options](Configure_Workflow_OptionsISA) for more information.

12. Click **Summary Workflow Translation.**

13. Click **Edit**.
    
    *[View the field descriptions for the Workflow Template
    page.](../Page_Desc/Workflow_Template)*

14. Select the language that will be used for the email message that
    contains a summary from the **LANGUAGE ID** field. Refer to [Create
    Language-specific Workflow Email
    Templates](Create_Language%20specific_Workflow_Email_Templates)
    for more information..

15. Update the text that will appear in the subject of the email as
    needed in the **SUBJECT** field.
    
    **NOTE:** A value preceded and followed by \# is a dynamic
    substitution value for replacement at run time. For example, the
    \#NAME\# field will be replaced with the user name of the user
    receiving the workflow email.

16. Update the text that will appear in the body of the email as needed
    in the **BODY** field.
    
    **NOTE:** A value preceded and followed by \# is a dynamic
    substitution value for replacement at run time. For example, the
    \#NAME\# field will be replaced with the user name of the user
    receiving the workflow email.

17. Click **Save**.
