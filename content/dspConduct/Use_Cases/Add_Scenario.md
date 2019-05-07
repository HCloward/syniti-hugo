+++
title = 'Add a Scenario'
solution = 'Master Data Management'
+++

# Add a Scenario

The *[Scenario](../Page_Desc/Scenario_H.htm)* page allows a Designer to
add to a scenario to a category. Refer to [Create a
Category](Create_a_Category.htm) for information about adding a
category.

Once added, a scenario can be added to a business process from a
different category than the business process’s parent category. Refer to
[Allow a Scenario to be used in other
Categories](Allow_a_Scenario_to_be_used_in_Other_Categories.htm) for
more information.

To add a scenario to a category in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane; the
    <span style="font-style: italic;">Category</span> page displays.

2.  Click the **Scenarios** icon for the category.

3.  The category displayed next to the page name is the scenario’s
    parent category.

4.  Click **Add**.
    
    *[View the field descriptions for the Scenario
    page.](../Page_Desc/Scenario_H.htm)*

5.  Enter a scenario name in the **NAME** field.

6.  Enter a description for the scenario in the **DESCRIPTION** field.

7.  Select a type from the **TYPE** list box.
    
    Values are:
    
      - **Create** - Creates new business objects, such as materials,
        customers, vendors, profit centers, GL accounts, etc.
      - **Change** - Updates the data in a logical way for an existing
        business object, such as by material group (Basic Data) for an
        existing material, pricing procedure (Sales Data) for an
        existing customer or incoterms (Purchasing Data) for an existing
        vendor.
      - **BusinessExtend** - Makes a new business object that is
        associated with an existing business object, such as a new BOM
        (Bill of Material) for an existing material, a new ship-to for
        an existing customer or a new order from address for an existing
        vendor.
      - **OrganizationalExtend** - Extends an existing business object
        to one or more Org Units, such as an existing material to a new
        plant, an existing customer to a new sales organization or
        company or an existing vendor to a new purchasing organization
        or company.

8.  Click the **ACTIVE** check box to enable it.

9.  Click **Save**; the *Scenario* page's *Vertical* View displays.
    
    *[View the field descriptions for the Scenario page’s Vertical
    View.](../Page_Desc/Scenario_H.htm#Scenario_V)*

10. Select the owner in the **Owner** list box. if needed.
    
    **NOTE:** Owner defaults to the parent category owner. A different
    owner can be selected.

11. Select the child scenario in the **Child Scenario Criteria** list
    box (optional).
    
    **NOTE:** This is the org unit to be used to create child requests
    for the scenario. Refer to [Configure Child Scenario
    Criteria](Configure_Child_Scenario_Criteria.htm) for more
    information.

12. Enter comments in the **Comment** field.

13. Click **Save**.

Continue with [Add a Role to a Scenario](Add_a_Role_to_a_Scenario.htm).
