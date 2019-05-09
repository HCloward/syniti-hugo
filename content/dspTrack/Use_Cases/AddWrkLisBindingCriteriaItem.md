+++
title = 'Add Work List Binding Criteria to a Work List Item or Plan Task'
solution = 'Platform'
+++

# Add Work List Binding Criteria to a Work List Item or Plan Task

**NOTE**: Users can add binding criteria to Work List Items and Plan
Tasks. Throughout this topic, “item" refers to both Work List Items and
Plan Tasks. Refer to [Plan Tasks v. Work List
Items](../Page_Desc/Plan_Tasks_Versus_Work_List_Items) for more
information.

An item can be bound to a specific set of data, such as a table.

A user assigned to the Sample Project Level Role or the Sample Plan
Level Role creates Work List Binding Criteria for an item by:

1.  Linking the item to a page on the *[Work List
    Setup](../Page_Desc/Work_List_Setup_H)* page’s *Vertical* View.
2.  Selecting a key description and key value for that page’s available
    keys on the *[Work List Binding
    Criteria](../Page_Desc/Work_List_Binding_Criteria)* page.

When a Business User clicks the link for the page on the Work List, the
Work List Binding Criteria passes the selected key’s description and
value to the page. The page opens with only the data associated with the
binding criteria displayed.

**NOTE**: A Business User must be assigned to the item to access it on
the Work List.

Refer to [Use Template Security
Roles](../Config/Use_Template_Security_Roles) for more information
about roles available in dspTrack™.

For example, a user assigned to the Sample Project Level Role can add
binding criteria to the Work List Item Confirm Mapping Freeze that binds
the item to the ttMARA table on Target Design's
*[Targets](../../../Migration/Design/Page_Desc/Targets_H_Design)*
page. To accomplish this, on the *[Work List
Setup](../Page_Desc/Work_List_Setup_H)* page’s *Vertical* View,the
user links the Confirm Mapping Freeze Work List Item to the *Targets*
page by selecting Target Design: Targets in the LinkToPage field.

Next, the user clicks the Keys icon for the Confirm Mapping Freeze Work
List Item to display the *[Work List Binding
Criteria](../Page_Desc/Work_List_Binding_Criteria)* page. The key
fields for the *Targets* page display in the KEY NAME field. To bind the
Confirm Mapping Freeze Work List Item to the ttMARA table, the user
selects Name for the <span style="text-transform: uppercase;">Key
Description</span> and ttMARA for the
<span style="text-transform: uppercase;">Key Value</span> for the
WaveProcessAreaObjectTargetID

Once the binding criteria is set up, a Business User can click the Page
ID icon on the Work List for the Confirm Mapping Freeze Work List Item,
and the selected key field’s description and value are passed to the
*Targets* page allowing only data for ttMARA to display on the *Targets*
page.

Before Work List Binding Criteria can be added:

  - [Add Work List Items](Add_Work_List_Items_Overview) if none
    exist
  - [Add Users to a Work List Item](Add_Users_to_an_Item)
  - [Add a Plan Task Manually](Add_a_Plan_Task_Manually) if none
    exist
  - [Add Users to Plan Tasks
    Manually](Add_Users_to_Plan_Tasks_Manually)

Refer to [Work with Work List Items](Work_with_Work_List_Items) and
[Work With Plan Tasks](Work_with_Plan_Tasks) for more information.

**NOTE:** Work List Binding Criteria can only be set up for items that
are not finished. The Planned Finish Date must be a future date.

To add or edit Work List Binding Criteria in dspTrack™:

1.  Select **Configuration \> Work List** in the Navigation pane.

2.  Click the **Vertical View** for the item.

3.  Click **Edit**.
    
    [View the field descriptions for the Work List Setup
    page](../Page_Desc/Work_List_Setup_H)

4.  Select the page in the **LinkToPage** list box.

5.  Click **Save**.

6.  Close <span style="font-style: italic;">Vertical</span> View.

7.  Click the **Keys** icon for an item on the *Work List Setup* page.
    
    **NOTE:** The number that displays on the icon denotes the number of
    key fields for the page selected in the LinkToPage list box on the
    *Work List Setup* page’s *Vertical* View. The *Work List Binding
    Criteria* page may display a single key or multiple keys.

8.  Click **Edit** on the *Work List Binding Criteria* page.
    
    [View the field descriptions for the Work List Binding Criteria
    page](../Page_Desc/Work_List_Binding_Criteria)

9.  Select a Work List Binding Criteria.
    
    **NOTE:** The KEY NAME field is view only. dspTrack™ uses the key
    fields from the underlying table of the page selected in the
    LinkToPage list box on the *Work List Setup* page’s *Vertical* View
    to display the key names These are the key names for the tables that
    are displayed on the selected page.

10. Select a description in the **KEY DESCRIPTION** list box.
    
    **NOTE:** The KEY DESCRIPTION list box lists the available fields in
    the table.

11. Select a value in the **KEY VALUE** list box.
    
    **NOTE:** The KEY VALUE list box lists the specific values available
    in the field selected in the KEY DESCRIPTION list box.

12. Click **Save**.

Once the binding is set up, when the user clicks the PAGE ID icon on the
Work List for the selected item, the page displays only the records for
the binding criteria that is set up.

**NOTE:** If no key value is selected, the page opens when the user
clicks the PAGE ID icon on the *Work List* page. However, the page is
not bound by any value and all records display.

If binding criteria has been set up for an item, the Business User can
access the page associated with an item without passing the binding
criteria to the page by using the <span>Unbound Page Link icon</span>.

The Unbound Page Link icon opens the page associated with an item
without passing the binding criteria to it. For example, a target name
has been set as binding criteria for a page in Target Design for the
selected item. If a user clicks the Unbound Page Link icon, the Target
Design page opens with data for all targets that the user can access,
and is not restricted to the target name. The Unbound Page Link icon is
disabled if Work List binding criteria is not set for the page.

To access the page without passing binding criteria:

1.  Click the blue tab on the Quick Panel to access the Work List.
2.  Click **Vertical View** for an item.
3.  Click **Unbound Page Link**<span>.</span>

Refer to [Work with Work List Items](Work_with_Work_List_Items) and
[Work With Plan Tasks](Work_with_Plan_Tasks) for a list of other
tasks available.
