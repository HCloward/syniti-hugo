# Project Distributions H

[Project Distributions V](#_Project_Distributions_V)

<div class="use">

Use this page to [Add Distributions to a
Project](../Use_Cases/Add_Distributions_to_a_Project).

</div>

To access this page:

1.  Click **Information Steward Accelerator \>  Project Summary** in the
    *Navigation* pane.
2.  Click <span style="font-weight: bold;">Distributions</span> for a
    project.

|                    |                                                                                                                                                                                                                                                                                |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field              | Description                                                                                                                                                                                                                                                                    |
| DISTRIBUTION       | Displays the unique name of the Distribution, used to group users and Quality Dimensions in a project. If no Distributions exist for the project they must be added before any other work can occur in ISA.                                                                    |
| DISTRIBUTION OWNER | Displays the user name of the user who is the primary contact of information for the data quality rules configured in the Distribution.                                                                                                                                        |
| Rules              | Click to open the *[Project Distribution Rules](Project_Distribution_Rules)* page to add and view the rules and bindings created in IS that are associated with the project Distribution.                                                                                  |
| Users              | Click to open the *[Project Distribution Users](Project_Distribution_Users)* page to add and user filters.                                                                                                                                                                 |
| Filters            | Click to open the *[Project Distribution Filters](Project_Distribution_Filters)* page to set up filters on fields to limit the data viewed on reports for the project distribution                                                                                         |
| Quality Dimensions | Click to open the *[Project Quality Dimensions](Project_Quality_Dimensions)* page to view projects and rules associated with Quality Dimensions.                                                                                                                           |
| Custom Attributes  | Click to open the <span style="font-family: Arial, sans-serif;font-style: italic;">[Project Distribution Attributes](Project_Distribution_Attributes)</span> page to add or remove rules from the project distribution based on the attributes assigned to the rule in IS. |
| Workflow Template  | Click to open the <span style="font-family: Arial, sans-serif;font-style: italic;">[Workflow Template](Workflow_Template)</span> page to add, edit or delete the templates used in workflows in the project distribution.                                                  |

## <span id="_Project_Distributions_V"></span> Project Distributions V

[Project Distributions H](Project_Distributions_H)

<div class="use">

Use this page to [Add Distributions to a
Project](../Use_Cases/Add_Distributions_to_a_Project).

</div>

Field

Description

Basic

Distribution

Displays the project distribution name.

Distribution Owner

Displays the user ID of the primary contact for information for the data
quality rules configured in the Distribution. Each distribution can have
only one owner.

Scorecard Link

Displays the link to the IS scorecard for the project. Click the link to
view the measurement of performance against goals for the resolution of
records that failed IS rules.

Workflow

Do Not Send Workflow

If enabled, users in the project distribution do not receive workflow
notifications.

**NOTE**: If this check box is enabled, the Schedule ID cannot be
updated and the Next Run Time field is blank.

This field is disabled by default.

Schedule ID

Displays the schedule created in Common used for sending notifications.

Refer to [Create
Schedules](../../../Platform/Common/Use_Cases/Create_Schedules) for
more information.

**NOTE**: If Distributions are configured to use the Schedule ID for
sending workflows (instead of sending on the same day as processing),
this value must be at least equal to the number of days in the longest
schedule registered to a Project Distribution.

Next Run Time

Displays the date and time when the notifications will next be sent.
