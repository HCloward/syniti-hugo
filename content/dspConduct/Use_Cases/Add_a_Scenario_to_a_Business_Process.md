+++
title = 'Add a Scenario to a Business Process'
solution = 'Master Data Management'
+++

# Add a Scenario to a Business Process

The <span style="font-style: italic;">[Business Process
(Scenarios)](../Page_Desc/Business_Process_Scenarios)</span> page
allows a Designer to assign scenarios to a business process.

Scenarios and business processes are added to a category, and then
scenarios are added to business processes. Scenarios are added to
business processes to group related scenarios used to create, change or
extend an object. A scenario must be added to a category before it can
be added to a business process. Refer to [Add a
Scenario](Add_Scenario) and [Add a Business
Process](Add_Business_Process) for more information.

A scenario from a different category than the business process’s parent
category can be added as long as it is not assigned the lowest priority
in the business process. It also cannot be a dependent of any other
scenarios in its parent category. Refer to [Allow a Scenario to be used
in other
Categories](Allow_a_Scenario_to_be_used_in_Other_Categories) for
more information.

One or more different scenarios can be added to a business process. A
particular scenario can only be added to a business process once.

<span style="font-weight: bold;">NOTE</span>: For new requests that are
automatically created as part of a multi-scenario business process, the
Content Request page OnValidate event is automatically executed. The
Cransoft UserID 'process' must have access to the Content Request page
in order to execute the OnValidate event.

To add a scenario to a business process in dspConduct™:

1.  Select **dspConduct \> Design** in the *Navigation* pane.

2.  Click the **Business Processes** icon for a category.

3.  Click the <span style="font-weight: bold;">Scenarios</span> icon.
    
    *[View the field descriptions for the Business Process (Scenarios)
    page](../Page_Desc/Business_Process_Scenarios)*

4.  Click **Add**.

5.  Enter the order in which the scenario is processed within the
    business process in the **PRIORITY** field.

6.  Select the scenario ID from the **Scenario ID** list box.

7.  Click **Save**.
