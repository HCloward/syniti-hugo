# Report Delivery Filters

Filters are used to restrict the data on a report so that only relevant
information displays to the user. Multiple columns can be used to
broaden the filter criteria.

The filter applies when the report is viewed in the DSP and does not
apply when it is downloaded.

**NOTE:** Since columns not applicable to a given report are ignored,
one filter can be configured to apply to many different reports.

Once Report Delivery filters are created in Transform, users can then be
assigned. A user can only be assigned to one filter at a time.

This topic contains the following sections:

  - [Create Report Delivery Filters](#Create_Report_Delivery_Filters)
  - [Assign a User to a Report Delivery
    Filter](#Assign_a_User_to_a_Report_Delivery_Filter)
  - [Copy a Report Delivery
Filter](#Copy_a_Report_Delivery_Filter)

## <span id="Create_Report_Delivery_Filters"></span>Create Report Delivery Filters

To create a report filter in Transform:

1.  Select **Configuration \> User Filter \> User Filter (By Filter)**
    in the *Navigation* pane.

2.  If no records exist, the *Filters* page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Filters
    page](../Page_Desc/Filters.htm)

3.  Enter a unique name for the filter in the **NAME** field.

4.  Enter a description for the filter in the **DESCRIPTION** field.

5.  Click **Save**.

6.  Click **Add** on the *Filter Column and Values* page.
    
    [View the field descriptions for the Filter Column and Values
    page](../Page_Desc/Filter_Column_and_Values.htm)

7.  Enter the **COLUMN NAME** to be filtered.
    
    **NOTE:** If an invalid column name is used, it is ignored.

8.  Select a value from the **OPERATOR** list box.

9.  Enter a value in the **CONSTANT** field.
    
    **NOTE:** If the value is not present in the column, the filter is
    ignored.

After creating a filter, assign a user to
it.

## <span id="Assign_a_User_to_a_Report_Delivery_Filter"></span>Assign a User to a Report Delivery Filter

A user can only be assigned to one filter at a time. If the user
selected is assigned to another filter, the current filter assignment
will be removed before a new filter assignment is made.

To add a user to a filter by filter in Transform:

1.  Select **Configuration \> User Filter \> User Filter (By Filter)**
    in the *Navigation* pane.
2.  Click the **Business User Assignment** icon for a filter.
3.  Select the user(s) on the *[User Filter User
    Assignment](../Page_Desc/User_Filter_User_Assignment.htm)* page.
4.  Click the **Assign Business User** (the **+** sign) icon in the Page
    toolbar to assign the user(s) to the selected filter; a confirmation
    message displays.

To add a user to a filter by user in Transform:

1.  Select **Configuration \> User Filter \> User Filter (By User)** in
    the *Navigation* pane.
2.  Select a user on the *[User Filters By User
    Parent](../Page_Desc/User_Filters_By_User_Parent.htm)* page.
3.  Select a filter on the *[Assign Filters By
    User](../Page_Desc/Assign_Filters_By_User.htm)* page.
4.  Click the **Assign Business User** (the **+** sign) icon in the Page
    toolbar to assign the user(s) to the selected filter; a confirmation
    message displays.
5.  Click **OK**; a check mark displays in the **MEMBER** column for the
    filter selected.

**NOTE:** The browser must be refreshed in order for the Assign User
Filter column for the user count to change to
1.

## <span id="Copy_a_Report_Delivery_Filter"></span>Copy a Report Delivery Filter

When copying a filter, the user has two options:

  - Copy the filter only.
  - Copy the filter and move the assigned user(s) from the original
    filter to the new filter. Because the assigned user(s) are moved
    from the original filter, the original filter will lose its user
    assignments. A user can be assigned to only one filter at a time.

To copy a filter in Transform:

1.  Select **Configuration \> User Filter \> User filter (By Filter)**
    in the *Navigation* pane.
2.  Select a filter.
3.  Click the **Copy Filter** icon in the Page toolbar.
4.  Click **Edit**.
5.  Enter a filter name in the **New Filter Name** field.
6.  Enter a description in the **New Filter Description** field.
7.  Click the **Copy User** check box to check it.
8.  Click **Save**.
9.  Click **Copy Filter**.

**NOTE:** Simply saving the filter does not complete the copy process.
The user must click Copy Filter to complete the process.
