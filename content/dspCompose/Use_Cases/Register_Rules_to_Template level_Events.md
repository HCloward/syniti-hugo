# Register Rules to Template-level Events

Business rules can be a powerful tool to help create default field
values and make mass change updates before any validations are executed.

dspCompose™ allows a Template Administrator to register a business  rule
that runs when a template-level event occurs. A rule is set to run when
a request is cancelled, created, deleted, or posted based on the
template for which the request was entered.

Rules can also be run when a request is created as a result of an
[External Request Scenario that Creates an Excel-initiated
request](External_Request_Scenarios_that_Create_Excel_Initiated_Requests.htm)
or an [External Request Scenario that Creates an Information
Steward-initiated
request](../../ISA/Use_Cases/External_Request_Scenarios_that_Create_Information_Steward%20initiated_Requests.htm).

When creating the template-level event rule, the Template Administrator
selects the rule that should run from a list of stored procedures from a
selected data source. These stored procedures can only accept the inputs
RequestID, TemplateID, boaUserID, and boaSAPLanguge.

Refer to [Register Rules to
Tables](../../../Platform/Collect/Use_Cases/Add_Rules_and_Indices_to_Tables.htm#Register_Rules_to_Tables)
for more information.

**NOTE**: To add a rule at the template level, the template must not be
active or must be in Developer Mode. Refer to [Modify an Active Template
in Developer Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for
more information.

To register a rule for a template-level event:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Vertical View** for a template.

4.  Click **Configuration** tab.

5.  Click **Events**.
    
    *[View the field descriptions for the Template (Events)
    page.](../Page_Desc/Template_Events.htm)*
    
    **NOTE:**The available Events are:
    
      - <span style="font-weight: bold;">Request Cancel</span> –
        Registered rules are executed when a template’s request is
        cancelled
    
    <!-- end list -->
    
      - <span style="font-weight: bold;">Request Create</span> –
        Registered rules are executed when a template’s request is
        created
      - <span style="font-weight: bold;">Request Delete</span> –
        Registered rules are executed when a template’s request is
        deleted
      - <span style="font-weight: bold;">Request Excel Create</span> –
        Registered rules are executed when a request is created as the
        result of an external request scenario that creates an
        Excel-initiated request
      - **Request ISA Create** – Registered rules are executed when a
        request is created as the result of an external request scenario
        that creates an Information Steward-initiated request
      - <span style="font-weight: bold;">Request Post</span> –
        Registered rules are executed after a template’s request is
        posted

6.  Click **Rules** for an Event.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click Add.
    
    [View the field descriptions for the Template (Event Rule)
    page](../Page_Desc/Template_Event_Rule.htm)

7.  Enter a sort order in **PRIORITY** field.
    
    **NOTE:** If multiple rules are assigned to the event, the PRIORITY
    determines the order the rule is run.

8.  Select a data source from the **DATA SOURCE ID** list box.
    
    **NOTE:** The DATA SOURCE ID contains the rule.

9.  Select the rule from the **RULE** list box.

10. Enter a brief rule description in **DESCRIPTION** field.

11. Click **Save**.
