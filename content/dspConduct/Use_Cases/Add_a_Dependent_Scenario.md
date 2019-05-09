+++
title = 'Add a Dependent Scenario'
solution = 'Master Data Management'
+++

# Add a Dependent Scenario

The [Scenario (Dependencies)](../Page_Desc/Scenarios_Dependencies)
page allows a Designer to set up dependencies between scenarios. Refer
to [Add a Scenario](Add_Scenario) for information on adding
scenarios. Dependent scenarios affect all business processes to which
they are assigned.

A Designer can configure a scenario to allow it to have a dependency
relationship with scenarios in other categories. Refer to [Allow a
Scenario to be used in other
Categories](Allow_a_Scenario_to_be_used_in_Other_Categories) for
more information. 

<span style="font-weight: bold;">NOTE</span>: For new requests that are
automatically created as part of a multi-scenario business process, the
Content Request page OnValidate event is automatically executed. The
Cransoft UserID 'process' must have access to the Content Request page
in order to execute the OnValidate event.

To add a dependent scenario to a scenario in dspConduct™:

1.  Select **dspConduct \> Design**.

2.  Click the **Scenarios** icon for a category on the
    *[Category](../Page_Desc/Category_H)* page.

3.  Click the **Dependencies** icon.

4.  Click **Add**.
    
    *[View the field descriptions for the Scenario (Dependencies)
    page](../Page_Desc/Scenarios_Dependencies)*

5.  Select the dependent scenario from the **DEPENDENT SCENARIO ID**
    list box.

6.  Click **Save**.
