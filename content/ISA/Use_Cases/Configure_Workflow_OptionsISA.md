# Configure Workflow Options

Workflow options set how and whether or not users receive information
about data that failed IS rules. A user may receive an email with an
attachment in the form of an Excel file, a summary in the body of the
email with the count of failed records and a link to the ISA to view
additional details, or may not receive notification.

Refer to [Summaries and Attachments](Summaries_and_Attachments) and
Review the Excel File for more information.

Workflow options can be set at the user level or at the project
distribution level.

Workflow notifications can be sent on a schedule for all users in the
project at the project distribution level. Refer to [Schedule Workflow
Notifications](Schedule_Workflow_Notifications) for more
information.

<span style="font-weight: bold;">NOTE</span>: Depending on how workflow
options are configured at the Distribution level and the user level,
duplicate messages may be sent to a user. The Delete Duplicated Workflow
setting on the
<span style="font-style: italic;">[Parameters](../Page_Desc/ISA_Parameters)</span>
page prevents duplicate workflows from being sent.

On the *[Users](../Page_Desc/Users_ISA)* page, configure how the
user receives a workflow with records that failed IS rules.

To configure user workflow options:

1.  Select <span style="font-weight: bold;">Information Steward
    Accelerator \> </span>**Configuration** in the *Navigation* pane.

2.  Click **Edit**.
    
    <span style="color: #0000ff;">[View the field descriptions for the
    Users page.](../Page_Desc/Users_ISA)</span>

3.  Select an option in the **WORKFLOW OPTION** list box.

4.  Values are: Configure at Distribution Level, Do Not Send Workflows,
    and Send Summaries Only.

5.  If the option selected is Configure at Distribution Level,
    additional configuration is required.

6.  Click **Save**.

7.  **NOTE:** Only Project Distributions in which the user is
    active display on the
    <span style="font-style: italic;">[Distribution Workflow Attachment
    Option](../Page_Desc/Distribution_Workflow_Attachment_Option)</span>
    page.  If a user is selected on the
    <span style="font-style: italic;">[Users](../Page_Desc/Users_ISA)</span>
    page and the <span style="font-style: italic;">Distribution Workflow
    Attachment Option</span> page does not display any records, ensure
    that the selected user is active in a distribution. Refer to
    [Activate Users for a Project
    Distribution](Add_Users_to_a_Project_Distribution) for more
    information.

**NOTE:** If the setting <span style="font-weight: bold;">Configure at
Distribution Level</span> is selected, perform the steps below.

To set the Workflow Attachment options at the Project Distribution
level:

1.  Click <span style="font-weight: bold;">Information Steward
    Accelerator \></span>**Configuration** in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click **Distribution Workflow Options** for a user with a WORKFLOW
    OPTION of **Configure at Distribution Level**.
    
    **NOTE:** If the WORKFLOW OPTION for the user is Send Summaries or
    Do Not Send Workflows, the Distribution Workflow Options icon is
    disabled.
    
    **NOTE:** The list of project distributions are those in which the
    selected user is active.
    
    **NOTE:** Only Project Distributions in which the user is active
    display on the <span style="font-style: italic;">[Distribution
    Workflow Attachment
    Option](../Page_Desc/Distribution_Workflow_Attachment_Option)</span>
    page.  If a user is selected on the
    <span style="font-style: italic;">[Users](../Page_Desc/Users_ISA)</span>
    page and the <span style="font-style: italic;">Distribution Workflow
    Attachment Option</span> page does not display any records, ensure
    that the selected user is active in a distribution. Refer to
    [Activate Users in a Project
    Distribution](Add_Users_to_a_Project_Distribution) for more
    information.

3.  Select a project distribution.

4.  Click the icon in the Page toolbar to configure how reports are sent
    to all of the users in the distribution. Values are:

<!-- end list -->

  - **Send Attachments** - An email is sent with the report of records
    that failed the IS rules included as an attachment.
  - **Send Emails Only** - An email is sent that has a summary table
    listing each rule with failed records along with record counts. The
    email has a link to the report in ISA.
  - **Do not Send Emails** - No emails are sent to users in the Project
    Distribution.
