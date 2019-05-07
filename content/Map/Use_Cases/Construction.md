+++
title = 'Construction'
solution = 'Migration'
+++

# Construction

The Construction action is used when mapping a field that has not been
defined in the Source system.

Using the Construction action in Map is also called using Enhanced
Construction. Refer to [Enhanced
Construction](../../Construct/Use_Cases/Enrichment_Construction.htm) for
more information.

**NOTE:** If the field group is All (the default field group (\*)) and
the action is Construction, Map creates the default rule from which to
pull values from Construct.

<span style="font-weight: bold;">NOTE</span>: A mapping with a
Construction action that is assigned to a field in a Field Group other
than the default field group (\* or “All” ) requires rules to be built
manually. Developers need to create a custom table to store the
different combinations of field groups for primary table keys and
construct data.

To create a field mapping using the Construction action on the
<span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page:

1.  Select the field to be mapped.

2.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Field Mappings
    page](../Page_Desc/Field_Mappings_H.htm)

3.  Select **Construction** from the **ACTION** list box.

4.  Click **Save**.
    
    **NOTE:** The <span style="font-weight: bold;">SOURCE TABLE</span>
    field displays the name of the table to be created in Construct,
    which begins with “dcs.” The <span style="font-weight: bold;">SOURCE
    FIELD</span> is updated with a field name that corresponds to the
    Target field.
    
    **NOTE:** In the table created in Construct, enter data that this
    field should contain for each primary key coming from the Source.

5.  Click <span style="font-weight: bold;">Submit</span> on the Page
    toolbar.
    
    **NOTE:** The platform creates a page in Construct that is named for
    the Wave-Source combination. A user does not have to use this page,
    and can make custom Construct pages if needed. The platform also
    creates the column in the table corresponding to the
    <span style="font-weight: bold;">SOURCE FIELD</span> and rules.
    
    **NOTE:** If the Auto Gen Level on the
    <span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page.htm)</span>
    page's <span style="font-style: italic;">Vertical</span> View is set
    to Off for the Target, the table and field are not created in the
    Target database and a page is not created in Construct.

The mapping must be approved by a Developer on the *Mapping
Approvals*page for documentation purposes and to help track progress of
the data migration project. Refer to
<span style="color: #0000ff;">[Mapping
Approvals](Approve_or_Reject_Mappings.htm)</span> and
<span style="color: #0000ff;">[Assign Developers to a Target or
Source](../../Design/Use_Cases/Add_Developers_and%20Business%20Contacts.htm)</span>
for more information.

Once the mapping has been created, the **Action, Source Table, Source
Field** and **Default Value** fields do not allow updates until one of
the following events occurs:

  - The Developer clicks **Reject** on the *Mapping Approval* page
  - The Mapper clicks **Reset** on the *Field Mappings* page

**NOTE**: When a user clicks Reset, Mapping By, Submitted By, Created By
and Approved By field will be reset to NULL values. The Rejected By
field does not update and contains the user ID of the Developer who
rejected the mapping on the <span style="font-style: italic;">[Mapping
Approval](../Page_Desc/Mapping_Approval_H.htm)</span> page. The Mapper
can contact the Developer with any questions.

Once the fields allow update, edit them, then click **Save** and click
**Submit**. This updated mapping is sent to the Developer for review on
the *Mapping Approval* page.
