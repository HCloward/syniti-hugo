# Add Custom Business Rules

A Designer can add a custom business rule at the scenario role level.
The custom business rules are run on the [Request
Role](../Page_Desc/Request_Role_H.htm) page.

Adding custom business rules allows stored procedures written on-site to
be executed from dspConduct™ [Request
Role](../Page_Desc/Request_Role_H.htm) page or dspConduct™
<span style="font-style: italic;">[Request Role
Task](../Page_Desc/Request_Role_Task.htm)</span> page. These pages
cannot be modified, so this is the means of running stored procedures
for certain events on these pages. For example, using this feature a
user can register custom business rules to the Foreground Post to
transfer data from Content tt tables into Integrate tables that are used
for posting.

Custom business rules can be added to the following events. The rules
are executed based on Role Type:

  - **Task ID** rules run when the TaskID button is clicked on the
    <span style="font-style: italic;">[Request Role
    Task](../Page_Desc/Request_Role_Task.htm)</span> page to access a
    Content page for entering or updating request data.

**NOTE:** The Task ID must not be an expected parameter of the custom
rule. Custom rules registered at this level are not specific to a
particular content page. Rules specific to a particular page must be
registered to that content page.

  - **Validate** rules run when the Validate button is clicked on the
    <span style="font-style: italic;">Request Role</span> page for any
    role.
  - **Finish** rules run when the Finish button is clicked on the
    <span style="font-style: italic;">Request Role</span> page for the
    Application role or Post role, or when the Approve button is clicked
    for the Review role.
  - **FinalFinish** rules run when the FinalFinish event executes for
    the Post Role.
  - **Reset** rules run when the Reset button is clicked on the
    <span style="font-style: italic;">Request Role</span> page for the
    Application role or the Reject button for the Review role.
  - **ForegroundPost** rules run before the Integrate posting adapter is
    called.

Refer to [dspConduct™ Design Process
Overview](dspConduct_Design_Process_Overview.htm) for information about
setting up Category, Scenario and Roles in dspConduct™. .

When adding a custom business rule, the Designer selects the rule from a
list of stored procedures from the selected data source. These stored
procedures can only accept the inputs RequestID and RoleID.

To add a custom business rule in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Design** in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the **Scenarios** icon for a category on the
    <span style="font-style: italic;">Category</span> page.

3.  Click the **Roles** icon for a scenario.

4.  Click the **Events** icon for a role.
    
    The events display depending on the type of role selected.
    
    *[View the field descriptions for the Scenario Role Event
    page.](../Page_Desc/Scenario_Role_Event.htm)*

5.  Click the **Rules** icon for an event.

6.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    *[View the field descriptions for the Scenario Role Event Rules
    page.](../Page_Desc/Scenario_Role_Event_Rule.htm)*

7.  Enter a priority for the position in the **PRIORITY** field.
    
    if there are multiple rules, the PRIORITY determines the order in
    which the rules run.

8.  Select a data source that stores the rule from the **DATA SOURCE
    ID** list box.

9.  Select a rule from the **RULE** list box.

Click **Save**.
