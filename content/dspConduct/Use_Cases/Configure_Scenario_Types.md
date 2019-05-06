# Configure Scenario Types

dspConduct™ is delivered with these default scenario types:

  - <span style="font-weight: bold;">Create</span> - Creates new
    business objects, such as materials, customers, vendors, profit
    centers, GL accounts, etc.
  - <span style="font-weight: bold;">Change</span> - Updates the data in
    a logical way for an existing business object, such as by material
    up (Basic Data) for an existing material, pricing procedure (Sales
    Data) for an existing customer or incoterms (Purchasing Data) for an
    existing vendor.
  - <span style="font-weight: bold;">BusinessExtend</span> - Makes a new
    business object that is associated with an existing business object,
    such as a new BOM (Bill of Material) for an existing material, a new
    ship-to for an existing customer or a new order from address for an
    existing vendor.
  - <span style="font-weight: bold;">OrganizationalExtend</span> -
    Extends an existing business object to one or more Org Units, such
    as an existing material to a new plant, an existing customer to a
    new sales organization or company or an existing vendor to a new
    purchasing organization or company.

A Designer can configure a default scenario type to allow updates, but
cannot delete the scenario type.

A Designer can add, edit, and delete custom scenario types, which allow
the Content WebApp to manage how scenarios behave around data that
already exists in the Target system.

The Scenario Type is used by dspConduct™ supplied function
apiSecurityScenarioEdit to return a value to indicate whether a record
can be edited. This function can be used in a Content WebApp when
building Data Control Views (DCV) for content pages.

When building content application pages, a typical Data Control View
uses the apiSecurityScenarioEdit function as one component to determine
if a record should be editable.  A typical Page Control View checks the
Scenario Type to enable the Add functions only when the scenario type is
Create or OrganizationalExtend. The Content WebApp Designer determines,
based on the business requirements of the users and technical
requirements of the target system, how these control views should be
built and whether they should follow these typical control view
guidelines.

To configure scenario types

Click <span style="font-weight: bold;">dspConduct \> Configuration \>
Setup \> Scenario Type</span> in the
<span style="font-style: italic;">Navigation</span> pane.

1.  Either:
    
    Click <span style="font-weight: bold;">Edit</span> and select the
    <span style="font-weight: bold;">UPDATE ALLOWED</span> check box.
    
    OR
    
    Click <span style="font-weight: bold;">Add</span> to add a custom
    scenario type.
    
    [View the field descriptions for the Scenario Type
    page](../Page_Desc/Scenario_Type.htm)

2.  Enter the scenario type name in the
    <span style="font-weight: bold;">SCENARIO TYPE</span> field.

3.  Click the <span style="font-weight: bold;">UPDATE ALLOWED</span>
    check box as needed.

4.  Click <span style="font-weight: bold;">Save</span>.
