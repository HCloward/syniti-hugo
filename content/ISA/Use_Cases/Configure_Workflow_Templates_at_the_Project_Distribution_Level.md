# Configure Workflow Templates at the Project Distribution Level

Workflow emails are sent to users that contain reports about data that
failed IS rules.  All attachment emails will be sent at the project
distribution level (i.e., all users in the project distribution will
receive attachment emails).

Multiple workflow templates for attachment emails can be configured at
the project distribution level. Templates for summary emails can be
configured at the parameter level only.

**NOTE**: For all template levels (parameter, project and project
distribution), do not configure multiple attachment templates in the
same language for the same project.

Workflow email templates can be configured at the
[parameter](Configure_Workflow_Templates_at_the_Parameter_Level.htm) or
[project](Configure_Workflow_Templates_at_the_Project__Level.htm) level
as well.

When the ISA applies templates, a user’s project distribution-level
template is applied by default. If no project distribution
level-template exists, the project template is applied. If no project
level-template exists, the parameter-level template is applied to the
user’s workflow template.

To configure a workflow template at the project distribution level:

1.  Select <span style="font-weight: bold;">Information Steward
    Accelerator \></span>**Configuration \> Project Summary** in the
    *Navigation* pane.

2.  Click the **Distributions** for a project.

3.  Click **Filters** for a project distribution.

4.  Click **Edit**.
    
    *[View the field descriptions for the Workflow Template
    page.](../Page_Desc/Workflow_Template.htm)*

5.  Select the language that will be used for the email message from the
    **LANGUAGE ID** field. Refer to [Create Language-specific Workflow
    Email
    Templates](Create_Language%20specific_Workflow_Email_Templates.htm)
    for more information..
    
    **NOTE:** Users can access the information on the report through an
    attachment, a summary, or links depending on the user’s workflow
    attachment options.  Refer to [Configure Workflow
    Options](Configure_Workflow_OptionsISA.htm) for more information.

6.  Update the text that will appear in the subject of the email as
    needed in the **SUBJECT** field.

7.  Update the text that will appear in the body of the email as needed
    in the **BODY** field.

8.  Click **Save**.
