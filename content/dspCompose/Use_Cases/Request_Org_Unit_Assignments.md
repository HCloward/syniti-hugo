# Request Org Unit Assignments

If the request is based on a template that has Org Units assigned, the
template’s Org Unit assignments are copied to the request when the
request is created. These Org Unit assignments display on the *[*Request
(Org Unit
Assignments)*](../Page_Desc/Request_Org_Unit_Assignments.htm)*page.

Template settings control which Org Unit assignments display on this
page, and whether the **ASSIGNED** check box can be enabled or disabled
on this page.

**NOTE**: A user is not allowed Org Unit security for a Request if not
assigned Org Unit Values for each Org Unit on the template.

This topic contains the following sections:

  - [Set Org Unit Assignment Security for a
    Request](#Set_Org_Unit_Assignment_Security_for_a_Request)
  - [Set Security at the Global
    Level](#Set_Security_at_the_Global_Level)
  - [Set Security at the Template
    Level](#Set_Security_at_the_Template_Level)
  - [Configure Org Unit Assignments for a
    Request](#Configure_Org_Unit_Assignments_for_a_Request)
  - [Reset the Org Unit Assignments for a
    Request](#Reset_the_Org_Unit_Assignments_for_a_Request)
  - [Updates to the Org Unit Table for a
    Request](#Updates_to_the_Org_Unit_Table_for_a_Request)

## <span id="Set_Org_Unit_Assignment_Security_for_a_Request"></span>Set Org Unit Assignment Security for a Request

A setting controls whether only Org Unit values assigned to the
requester display or all Org Unit values for the template display on the
*[Request (Org Unit
Assignments)](../Page_Desc/Request_Org_Unit_Assignments.htm)* page.

A setting also controls whether the **ASSIGNED** check box can be
enabled or disabled on this page, which allows a user to add or remove
Org Unit values from the request. This setting can control user access
to request data based on a user’s assigned Org Unit values.

These parameters are set at the global level and may be overridden at
the individual template
level.

## <span id="Set_Security_at_the_Global_Level"></span>Set Security at the Global Level

To set security for request Org Unit Assignment at the global level:

1.  Select **Configuration \> Parameters** from *Navigation* pane.

2.  Click the **Template** tab.
    
    To set security parameters that will be used by the *Request (Org
    Unit Assignments)* page:

3.  Click the **Only Show Org Unit Values Assigned to Requester** check
    box to enable it.
    
    **NOTE:** On the *[*Request (Org Unit
    Assignments)*](../Page_Desc/Request_Org_Unit_Assignments.htm)* page,
    only those Org Unit values assigned to the requester display. If the
    check box is not selected, Org Unit values assigned to all users on
    the template display.

4.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Parameters page, Template
    tab](../Page_Desc/Parameters.htm#Template_Tab)

5.  Select an option from the **Org Unit Security Level** list box.
    
    **NOTE:** The value chosen sets how Org Unit values are assigned to
    requests by default. The **ASSIGNED** column on the *[*Request (Org
    Unit Assignments)*](../Page_Desc/Request_Org_Unit_Assignments.htm)*
    page is checked or unchecked based on the Org Unit Security Level.
    Options are:
    
      - **OrgUnit Values Available For Assignment** – All of the
        individual Org Unit values possible for the request are
        available for assignment to the request, but no assignments are
        assigned by default. (None of the **ASSIGNED** check boxes are
        enabled by default.)
    
      - **User Assignments Defaulted, Change Allowed** – All of the
        individual Org Unit values available to the user creating the
        request are assigned to the request by default, but may be
        unassigned. (All of the **ASSIGNED** check boxes on the
        <span style="font-style: italic;">Request (Org Unit
        Assignments)</span><span>page</span> are enabled by default.)
    
      - **User Assignments Defaulted, No Change Allowed** – All of the
        individual Org Unit values available to the user are assigned to
        the request and cannot be unassigned. (All of the **ASSIGNED**
        check boxes on the <span style="font-style: italic;">Request
        (Org Unit Assignments)</span> page are enabled by default.) If
        this option is selected, the **Select All**, **Unselect All**,
        and **Reset Defaults** buttons are disabled on the *Request (Org
        Unit Assignments)* page.

6.  Click <span style="font-weight: bold;">Save</span>.

The Org Unit Security Level set on
the<span style="font-style: italic;">[Parameters](../Page_Desc/Parameters.htm)</span><span>page
is the default value for all newly created
templates.</span>

## <span id="Set_Security_at_the_Template_Level"></span>Set Security at the Template Level

To change the global parameter values for an individual template,
navigate to the settings at the template level:

1.  Click **Team** on *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **VerticalView** for a template.

4.  Click **Advanced** tab.

5.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Templates page, Advanced
    tab](../Page_Desc/Templates_H.htm#Advanced_Tab)

6.  Make choices as described above.

Once a user has set Org Unit values on the *Request (Org Unit
Assignments)* page, unassigned Org Units (i.e., Org Unit values from a
request that do not have the **ASSIGNED** check box enabled on the
*Request (Org Unit Assignments)* page)  are removed from the request
automatically when a user clicks the **Confirm Org Units** button on the
*Request* page.

**NOTE**: If all of a user’s Org Unit assignments are removed at the
request level, the user will not be able to process the request. If the
user entered the request, the request still displays on the *Request*
page for the user, but the user cannot process
it.

## <span id="Configure_Org_Unit_Assignments_for_a_Request"></span>Configure Org Unit Assignments for a Request

To configure Org Unit assignments for a request:

1.  Click **Requests** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Org Units** for a request.

3.  Click the **ASSIGNED** check box to include the Org Unit assignment
    in the request.
    
    **NOTE**: Click **Select All** or **Unselect All** to include or
    exclude all Org Unit assignments from the request.
    
    **NOTE**: To reset a request’s Org Unit assignments back to the
    template Org Unit assignments, click **Reset Defaults**. Refer to
    [Reset the Org Unit Assignments for a
    Request](#Reset_the_Org_Unit_Assignments_for_a_Request) for more
    information.

4.  Navigate to the *Request* page.

5.  Click **Confirm Org Units** on the Page toolbar; a confirmation
    message displays.
    
    **NOTE**: The user clicks **Confirm Org Units** to indicate that all
    applicable Org Unit Values have been assigned to the request. Once
    confirmed they cannot be changed and the request will become active.
    
    **NOTE**: If a request is based on a template that uses Org Units,
    the user must click **Confirm Org Units** on the Page toolbar, even
    if there are no Org Unit values assigned to the request. The
    **Roles** icon on the *Request* page will remain disabled until the
    user clicks **Confirm Org Units**.

6.  Click **Ok**.

Once Org Units have been confirmed, the **Org Units** icon is no longer
active for the request. The **Org Units Assigned** icon is now active.
Click this icon to view the request’s Org Unit assignments.

Once a request with Org Units is saved, the Org Unit, request ID, and
user ID are written to the Org Units table in the cMass\_Data database.
Refer to [TEMPLATE COLUMN
Information](Set_up_Org_Units.htm#TEMPLATE_COLUMN_Information) for more
information.

## <span id="Reset_the_Org_Unit_Assignments_for_a_Request"></span>Reset the Org Unit Assignments for a Request

Org Unit assignments are originally made at the template level, but may
be modified at the request level depending on the Org Unit parameter
values chosen at the template level. If the assignments are changed at
the request level, the user can reset the Org Unit assignments back to
those assigned to the template.

**NOTE**: Once a request’s Org Units have been confirmed, the request’s
Org Unit assignments cannot be reset back to the template Org Unit
assignments. Refer to [Request Org Unit Assignments](#) for more
information.

To reset Org Unit assignments for a request:

1.  Click **Requests** on *Navigation
    <span style="font-style: normal;">pane</span>*.
2.  Click **Org Units** for a request.
3.  Click **Reset Defaults** on the Page toolbar; a confirmation message
    displays.
4.  Click
**Ok**.

## <span id="Updates_to_the_Org_Unit_Table_for_a_Request"></span>Updates to the Org Unit Table for a Request

Once a request that uses Org Units has been saved, dspCompose™ updates
the Org Unit table for the template in the cMass\_Data database.

The Org Unit table contains rows for each combination of Org Unit values
for each user who is assigned security for each of those values.

For example, a template has the Org Units Plant and Sales Org assigned.

User A is assigned to all Plants and all Sales Orgs.

User B is assigned to Plant AB10 and Sales Org AB01.

A user creates a request based on the template that has the Org Unit
values of Plants ‘AB10’ and ‘AB12’ and Sales Orgs ‘AB01’ and ‘AB02.’

For User A, the Org Unit table will contain the following entries:

  - Plant AB10, Sales Org AB01
  - Plant AB12, Sales Org AB01
  - Plant AB10, Sales Org AB02
  - Plant AB12, Sales Org AB02

For User B, the Org Unit table will contain the following entry:

  - Plant AB10, Sales Org AB01
