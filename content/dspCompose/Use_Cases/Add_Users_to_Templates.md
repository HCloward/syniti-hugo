# Add Users to Templates

Add dspCompose™ users to templates so that the user can process request
data using the template.

A Template Administrator can grant users access to a template at the
global level or at the template level:

These two methods produce the same result. At the global level, a
Template Administrator can grant users access to multiple templates from
one page. At the template level, user access is granted to the selected
template only.

When a user creates a template, that user has access to all roles
associated with the template and can grant access to template roles at
the template level.

**NOTE**: If a template uses Org Units, a user must also be assigned to
those Org Units to access the request data. Refer to [Assign Users to
Org Units](Set_up_Org_Units.htm#Assign_Users_to_Org_Units) for more
information.

This topic contains the following sections:

  - [Grant Template Access at the Global
    Level](#Grant_Template_Access_at_the_Global_Level)
  - [Grant Template Access at the Template
    Level](#Grant_Template_Access_at_the_Template_Level)
  - [Create Review
Filters](#Create_Review_Filters)

## <span id="Grant_Template_Access_at_the_Global_Level"></span>Grant Template Access at the Global Level

To grant a user access to a template at the global level:

1.  Select **Configuration \> Users** from *Navigation
    <span style="font-style: normal;">pane</span>*.
2.  Click **Templates** for a user.
3.  Grant or deny a user access to a template
role.

## <span id="Grant_Template_Access_at_the_Template_Level"></span>Grant Template Access at the Template Level

To grant user access to a template at the template level:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">p</span><span style="font-style: normal;">ane</span>*.

2.  Click **Templates** for a team.

3.  Click **Users** for a template.

4.  Click **Add**.
    
    *[View a field descriptions of the Template (Users)
    page.](../Page_Desc/Template_Users_H.htm)*

5.  Select an option from the **USERID** list box.
    
    **NOTE**: The USER ID list box displays users who have been granted
    access to dspCompose™. Refer to [Add Users to
    dspCompose™](../Config/Add_Users_to_dspCompose.htm) for more
    information.

6.  Click **Save**.

7.  Click **Roles** for a user.

8.  Click **Grant** for a role.

**NOTE**: A user that is granted the Review role can also have a review
filter set on this page.

## <span id="Create_Review_Filters"></span>Create Review Filters

A Review filter allows a Template Administrator to set column,
conditional, and value combinations at the template user level to limit
the data displayed to a user for approval. On the *[*User Template
Filter*](../Page_Desc/User_Template_Filter.htm)* page, a Template
Administrator can create a Review filter for each user with access to
the review role for a request based on a template. This set up allows
multiple users to each view and approve a different subset of request
data because there may not be one user who is suitable to approve all
the request data.

The filter limits the data the Review role can view, approve, and reject
for the request. If a user does not have a Review filter, all request
data displays and a user will be able to fully approve all requests
entered for the template. If a Review filter is set, the user will only
be able to approve the records that match the Review filter parameters.

Review filters can affect how a request moves through the posting
process. For a request to move to the Review role, the Review filters
must allow all records to be reviewable by at least one user. For the
request to be completely approved, a user must have access to all
records to approve the request.

**NOTE**: Review filters only apply to dspCompose™-generated
Review/Approve pages. If a custom page is assigned to a Review role,
then the Review filters do not apply to that page.

**NOTE**: If the template has Org Unit assignments, these assignments
will also affect the request data that a user can access. Refer to [Set
up Org Units](Set_up_Org_Units.htm) for more information.

To create a Review filter at the template level:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Users** for a template.

4.  Click **Review Filter** for a user.
    
    <span style="font-weight: bold;">NOTE:</span> If no records exist,
    the page displays in add mode. Otherwise, click Add on Toolbar.
    
    [View the field descriptions for the User Template Filter
    page](../Page_Desc/User_Template_Filter.htm)

5.  Select a column from the **COLUMN NAME** list box.
    
    <span style="font-weight: bold;">NOTE:</span>The COLUMN NAME is used
    in the comparison operation to limit data within the view being
    changed.  

6.  Select an operator from the **CONDITIONAL** list box.
    
    <span style="font-weight: bold;">NOTE:</span>A CONDITIONAL is
    selected if a comparison between two fields is required.

7.  Enter a value in the **VALUE** field.

8.  Click **Save**.

**NOTE**: If a Review Filter is set up for a user such that certain
records cannot be reviewed, the records can be accessed by the Template
Administrator who can then adjust the review filter.

To view these records for this scenario:

1.  Select **Request** from *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Roles** for a request.

3.  Click **Vertical View** for the Data role.

4.  Click **Non Review Page ID**.
    
    <span style="font-weight: bold;">NOTE</span>: The Non Review Page ID
    icon is active for the highest priority Data Entry role, the last
    role that needs to be finished before the request moves to the
    Review role.

5.  View the records and adjust the Review filter so that the records
    can display for the Review user and can move through the request
    process.
