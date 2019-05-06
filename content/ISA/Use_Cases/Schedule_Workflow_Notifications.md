# Schedule Workflow Notifications

ISA runs a service page every hour to check if IS has processed rules.
ISA also runs a service page every 10 minutes to send workflows if IS
has processed rules.

If IS runs rules frequently (e.g.,  multiple times per day), the ISA
sends notifications to users (depending on how that user’s workflow
options are configured) each time the rule runs, resulting in numerous
emails.

A user may receive an email with an attachment in the form of an Excel
file, a summary in the body of the email with the count of failed
records and a link to the ISA to view additional details, or may not
receive a notification.

A user can schedule the frequency that notifications are sent at the
Project Distribution level. The schedule is set for all users in the
distribution.

<span style="font-weight: bold;">NOTE</span>: Schedules are created in
Common, and can be set to run hourly, daily, weekly, monthly, yearly, or
on a specific day. Refer to [Create
Schedules](../../../Platform/Common/Use_Cases/Create_Schedules.htm) for
more information about schedule recurrence.  

**NOTE**: If workflow notifications are to be sent using a schedule
created in Common, the user must update the ISA parameter Days to Retain
Files (ISA *[Parameters](../Page_Desc/ISA_Parameters.htm)* page Basic
Settings tab) so that it is at least equal to the number of days in the
longest schedule registered to a Project Distribution.

<span style="font-weight: bold;">NOTE</span>: A user can send workflows
on demand as well. Refer to [Run Rules and Send Workflows on
Demand](Run_RulesRun_Workflows_.htm) for more information.

<span style="font-weight: bold;">NOTE</span>: Workflow options can also
be configured for an individual user. Refer to [Configure Workflow
Options](Configure_Workflow_OptionsISA.htm) for more information.

<span style="font-weight: bold;">NOTE</span>: When the Do Not Send
Workflow check box is enabled on the
<span style="font-style: italic;">[Project
Distributions](../Page_Desc/Project_Distributions_H.htm)</span> page,
all workflow notifications for the distribution are deleted. It is
recommended to use this feature when designing a new distribution so
that notifications are not continually sent out during development and
testing runs.

<span style="font-weight: bold;">NOTE</span>: Depending on how workflow
options are configured at the Distribution level and the user level,
duplicate messages may be sent to a user. The Delete Duplicated Workflow
setting on the [Parameters](../Page_Desc/ISA_Parameters.htm) page
prevents duplicate workflows from being sent.

To schedule when workflows are sent:

1.  Select <span style="font-weight: bold;">Information Steward
    Accelerator \> Project Summary</span> in the
    <span style="font-style: italic;">Navigation</span> pane,

2.  Click the <span style="font-weight: bold;">Distributions</span> icon
    for a project.

3.  Click <span style="font-weight: bold;">Vertical View</span> for a
    distribution.

4.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Project Distributions page's
    Vertical
    View](../Page_Desc/Project_Distributions_H.htm#_Project_Distributions_V)

5.  Either:
    
    1.  Click the <span style="font-weight: bold;">Do Not Send
        Workflow</span> check box.
        
        OR
    
    2.  Select the schedule to send workflow notifications from the
        <span style="font-weight: bold;">Schedule ID</span> list box and
        click <span style="font-weight: bold;">Save</span>.

**NOTE:** The Next Run Time field displays the next date or time that
notifications are sent to users in this distribution.
