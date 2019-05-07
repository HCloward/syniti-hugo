+++
title = 'Configure Child Scenario Criteria'
solution = 'Data Quality'
+++

# Configure Child Scenario Criteria

A Designer can select the org unit to be used to create child requests
for the scenario.

For example, a user creates a request, Create and Extend Finished Good.
The request has been added to a category that has an org unit 1 of
Plants.

The request is based on a multi-scenario business process where the
first scenario creates the material and the child scenario extends it to
Plant.

There are two options for generating child requests:

  - One child request for all Plants, so that no matter how many Plants
    the user chooses for the first request, dspConduct™ creates one
    child request for the scenario.
  - One child request per Plant, chosen at the time the first (parent)
    request was made. If the user chooses three Plants, when entering
    the request for the Parent scenario, dspConduct ™creates three
    parallel requests when the first request finishes. To use this
    option, set the org unit as described in the steps below.

<span style="font-weight: bold;">NOTE</span>: Org units are set up at
the category level. Refer to [Add an Org Unit Type to a Category
Object](Manage_Org_Units.htm#Add_an_Org_Unit_Type_to_a_Category_Object)
for more information.

To configure child scenario criteria:

1.  Select **dspConduct \> Design** in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the **Scenarios** icon for a category on the *Category* page.

3.  Click **Vertical View** for a scenario.
    
    [View the field descriptions for the Scenario page’s Vertical
    View.](../Page_Desc/Scenario_H.htm#Scenario_V)

4.  Click **Edit**.

5.  Select the org unit to be used to create child requests from the
    **Child Scenario Criteria** list box.

6.  Click <span style="font-weight: bold;">Save</span>.
