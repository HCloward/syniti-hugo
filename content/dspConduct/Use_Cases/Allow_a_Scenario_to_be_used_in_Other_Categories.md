+++
title = 'Allow a Scenario to be Used in Other Categories'
solution = 'Master Data Management'
+++

# Allow a Scenario to be Used in Other Categories

Scenarios and business processes are added to a category, and then
scenarios are added to business processes. Refer to [Add a
Scenario](Add_Scenario) and [Add a Business
Process](Add_Business_Process) for more information.

A Designer can allow a scenario to be added to a business process from a
different category than the business process’s parent category as long
as it is not assigned the lowest priority in the business process. The
scenario also cannot be a dependent of any other scenarios in its parent
category.

<span style="font-weight: bold;">NOTE:</span> When a business process
uses a scenario from another category, the request that is created for
that scenario will be created in the database/WebApp that is the default
WebApp for that other category. For example, a category called Northwest
Region has a default WebApp of NWRegion. It  contains a scenario called
Create SoldTo – General Data. This scenario has been configured for use
in the category US Operations. A scenario in US Operations is Create
SoldTo. A user could create a business process in the US Operations
category that uses the Create SoldTo scenario as a parent of the Create
SoldTo – General Data scenario from the Northwest Region category. When
the business process is executed, a request is created in the NWRegion
WebApp.  

<span style="font-weight: bold;">NOTE:</span> For new requests that are
automatically created as part of a multi-scenario business process, the
Content Request page OnValidate event is automatically executed. The
Cransoft UserID 'process' must have access to the Content Request page
in order to execute the OnValidate event.

To allow a scenario to be assigned to a business process that is in a
category other than its parent category in dspConduct:

1.  Select <span style="font-weight: bold;">dspConduct \> Design</span>
    in the *Navigation* pane; the Category page displays.

2.  Click the **Scenarios** icon for the category.

3.  The category displayed next to the page name is the scenario’s
    parent category.

4.  Click <span style="font-weight: bold;">Vertical View</span> for a
    scenario.

5.  Click the **Use In Other Category** icon.
    
    *[View the field descriptions for the Scenario Use In Other Category
    page.](../Page_Desc/Scenario_Use_in_Other_Category)*

6.  Select the category in the **OTHER CATEGORY ID** list box.

7.  Enter the reason the scenario is being used in the category in the
    **COMMENT** field.

8.  Click **Save**.

Continue with [Add a Scenario to a Business
Process](Add_a_Scenario_to_a_Business_Process).
