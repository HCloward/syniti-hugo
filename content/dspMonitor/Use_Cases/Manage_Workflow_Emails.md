+++
title = 'Manage Workflow Emails'
solution = 'Data Quality'
+++

# Manage Workflow Emails

Workflow emails are sent to notify when reports have been run.

This use case covers the following topics:

  - [Configure Workflow Content](#Configure_Workflow_Content)

  - [Configure Workflow
Schedules](#Configure_Workflow_Schedules)

## <span id="Configure_Workflow_Content"></span>Configure Workflow Content

The content of workflow emails, such as the email To, From and Subject
lines, and the email body are configurable.

To configure workflow content:

1.  Navigate to <span style="font-weight: bold;">Configuration \>
    Parameters</span> in
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Workflow Parameters</span>
    tab.

3.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Parameters
    page](../Page_Desc/Parameters)

4.  Configure the Workflow Parameters as needed.

5.  Click
**Save**.

## <span id="Configure_Workflow_Schedules"></span>Configure Workflow Schedules

Workflow email schedules are [configured at the group
level,](#Configure_Workflow_Schedules_for_Groups) but can be further
customized [at the user report
level](#Configure_Workflow_Schedules_for_User_Reports). Workflow
monitoring is also available to view details about scheduled and sent
workflow emails.

Workflow schedules can be configured for groups and for individual
users.

## <span id="Configure_Workflow_Schedules_for_Groups"></span>Configure Workflow Schedules for Groups

Workflow schedules are configured at the group level, which impacts all
reports in the group.

To configure workflow schedules for
groups:

1\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Select
**Configuration \> Groups** in *Navigation* pane.

2\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Click
**Vertical View** for Group ID.

3\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Click
**Workflow Scheduling** tab.

4\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Click
**Edit<span style="font-weight: normal;">.</span>**

[View the field descriptions for the Groups page's Vertical
View](../Page_Desc/Groups_H)

5\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Select
a schedule form **Workflow Schedule ID** to control when workflow emails
are sent for the group.

**NOTE:** Since the Workflow Schedule ID can be customized at the user
level, dspMonitor™ must calculate all workflow schedule options for the
group in case a user sets the schedule at a different frequency. If
these fields are left blank, default values are automatically entered.

**NOTE:** Schedules are maintained in Common. Refer to [Create
Schedules](../../../Platform/Common/Use_Cases/Create_Schedules) for
detailed information.

6\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Click
**Save<span style="font-weight: normal;">.</span>**

## <span id="Configure_Workflow_Schedules_for_User_Reports"></span>Configure Workflow Schedules for User Reports

Workflow emails can be configured at the user level for specific reports
to trigger emails at a higher frequency than the schedule set for the
report group.

To configure workflow schedules for
users:

1\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Select
**Configuration \> User Reports/Filters** in *Navigation* pane.

2\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Click
**Reports** for User ID.

3\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Click
**Edit<span style="font-weight: normal;">.</span>**

[View the field descriptions for the User (Reports)
page](../Page_Desc/User_Reports_H)

4\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Select
a schedule form **Workflow Schedule ID** to control when workflow emails
are sent for the group.

**NOTE:** Schedules are maintained in Common. Refer to [Create
Schedules](../../../Platform/Common/Use_Cases/Create_Schedules) for
detailed information.

5\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">   </span> Click
**Save<span style="font-weight: normal;">.</span>**
