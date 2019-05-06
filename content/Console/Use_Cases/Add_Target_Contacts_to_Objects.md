# Add Target Contacts to Objects

A user can quickly assign Developers or Business Users contacts to many
or all Objects at one time.

When assigned at the Object level, the contact is added to every Target
and Source that belongs to the Object, and can be viewed and edited in
Target Design.

<span style="font-weight: bold;">NOTE</span>: Individual users can also
be assigned to an Object as Developers or Business Users in Console and
Target Design. Refer to [Add Developers and Business Contacts to a
Target or
Source](../../Design/Use_Cases/Add_Developers_and%20Business%20Contacts.htm)
for more information about adding users as contacts in Target Design.

Developers approve mappings on the
<span style="font-style: italic;">[Mapping
Approval](../../Map/Page_Desc/Mapping_Approval_H.htm)</span> page
submitted for a Target-Source in Map on the
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page. Refer
to [Approve or Reject
Mappings](../../Map/Use_Cases/Approve_or_Reject_Mappings.htm) for more
information.

Business User contacts are used for reporting purposes and automatically
receive published reports and Data Services reports for the target in
Transform. Refer to [Report
Delivery](../../Transform/Use_Cases/Report_Delivery_Overview.htm) for
more information.

<span style="font-weight: bold;">NOTE</span>: A user cannot be assigned
as a Business User and a Developer for the same Object using this method
in Console. In Target Design, a user can be added as a Developer for one
Target and a Business User for another.

To view the contacts assigned to each Object,
select<span style="font-weight: bold;"> Elements \> Objects \>
Contacts</span>.

A user can:

  - [Add Individual Target Contacts](#Add2)

  - [Add Multiple Target Contacts](#Add3)

## <span id="Add2"></span>Add Individual Target Contacts

An individual user can be assigned as a Business Contact or a Developer
at the Target or Source level in Target Design and at the Object level
in Console.

When assigned at the Object level, the contact is added to every Target
and Source that belongs to the Object, and can be viewed and edited in
Target Design.

When a Target is added to an Object in Target Design, any Object
contacts with positions of Business User (Target Contact) or Developer
(Target Contact) in Console will be automatically added to the
appropriate target contacts and Target Source contacts in Target Design.

If the contact is deleted or removed from the Object’s Business User
(Target Contact) or Developer (Target Contact) position in Console, the
contact is also removed from the target contacts or Target Source
contacts in Target Design.

While changes in Object contacts cascade down to Target Design, changes
to contacts in Target Design do not affect contacts at the Object level.
Removing a target or source contact in Target Design does not affect
target contact assignments at the Object level.

To add the contact to an Object in Console that will be used in Target
Design:

1.  Select **Elements \> Object** in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the **Contacts** icon for an Object.

3.  Click **Add**.
    
    [View the feild descriptions for the Object Contacts
    page](../Page_Desc/Object_Contacts.htm)

4.  Select the contact name in the **CONTACT** list box.
    
    **NOTE**: These users are registered in the platform.
    
    **NOTE**: Users who are not registered in the platform but who
    should receive workflow messages can be added. Type the user’s name
    in the CONTACT list box and proceed with the steps.

5.  Select **Business User (Target Contact)** or **Developer (Target
    Contact)** from the **POSITION** list box.
    
    **NOTE:** A user cannot be added as both a Business User and a
    Developer to the same object in Console. A user can be added as a
    Business User to a target, and a Developer to a different target in
    the same object. Refer to [Add Developers and Business Contacts to a
    Target or
    Source](../../Design/Use_Cases/Add_Developers_and%20Business%20Contacts.htm)
    for more information about adding users as contacts in Target
    Design.

6.  Add contact information as needed.

7.  Click **Save**.

The contact is added as a Developer or Business Contact to all targets
and sources associated with the Object in Target Design.

## <span id="Add3"></span>Add Multiple Contacts to an Object

From a high level, to add multiple users to an Object:

1.  [Add many or all users to the bulk contact staging area.](#Add)
2.  [Assign a position to many or all users](#Assign)
3.  Assign many or all contacts to many or all objects.

### <span id="Add"></span>Add Users to the Staging Area

Console allows a user to add multiple Developer and Business User
contacts to Objects at the same time.

To begin the process, add users to the bulk contact staging area on the
<span style="font-style: italic;">[Users](../../../Platform/Sys_Admin/Page_Desc/Users_H.htm)</span>
page.

To add many or all registered users to the bulk contact staging area:

1.  Select <span style="font-weight: bold;">Advanced Configuration \>
    Object Contact Configuration</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Select the users to assign to Objects on the
    <span style="font-style: italic;">Users</span> page.
    
    **NOTE**: To select a contiguous range of users, hold down the
    **Shift** key and select the first and last users in the range. To
    select a non-contiguous range of users, hold down the **Ctrl** key
    and select each user.
    
    **NOTE**: Users who display on the
    <span style="font-style: italic;">Users</span> page are registered
    in the platform.  

3.  Click <span style="font-weight: bold;">Add User</span> in the Page
    toolbar.

The <span style="font-style: italic;">[Bulk Contact Staging
Area](../Page_Desc/Bulk_Contact_Staging_Area.htm)</span> page updates
and lists all users who can be assigned to Objects. The contact
information that displays for users was added when the user’s account
was created.

**NOTE**: Removing users from the Bulk Contact Staging Area does not
affect contact assignments to Objects.

To remove a user from the Bulk Contact Staging Area:

1.  Select <span style="font-weight: bold;">Advanced Configuration \>
    Object Contact Configuration</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Select the users to remove from the Bulk Contact Staging Area on the
    <span style="font-style: italic;">[Users](../../../Platform/Sys_Admin/Page_Desc/Users_H.htm)</span>
    page.
    
    **NOTE**: To select a contiguous range of users, hold down the
    **Shift** key and select the first and last users in the range. To
    select a non-contiguous range of users, hold down the **Ctrl** key
    and select each user.

3.  Click the <span style="font-weight: bold;">Remove User</span> icon
    on the page toolbar.

To remove all users from the Bulk Contact Staging Area:  

1.  Select **Advanced Configuration \> Object Contact Configuration** in
    the *Navigation* pane.
2.  Click the **Reset Staging Area** icon in the Page toolbar.   

After adding users, continue with Assign a Position to Users.

### <span id="Assign"></span>Assign a Position to Users

Positions are Developers or Business Users contacts.

Developers approve mappings on the Mapping Approval page submitted for a
target-source in Map on the Field Mappings page. Refer to [Approve or
Reject Mappings](../../Map/Use_Cases/Approve_or_Reject_Mappings.htm) for
more information.

Business User contacts are used for reporting purposes and automatically
receive published reports and Data Services reports for the target in
Transform.

To continue the process, assign a Developer or Business User contact to
users.

To assign a position to many or all users:

1.  Select<span style="font-weight: bold;"> Advanced Configuration \>
    Object Contact Configuration</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Select one or many users on the
    <span style="font-style: italic;">[Bulk Contact Staging
    Area](../Page_Desc/Bulk_Contact_Staging_Area.htm)</span> page.
    
    **NOTE**: To select a contiguous range of users, hold down the
    **Shift** key and select the first and last users in the range. To
    select a non-contiguous range of users, hold down the **Ctrl** key
    and select each user.

3.  Click the <span style="font-weight: bold;">Set As Business
    User</span> icon or the <span style="font-weight: bold;">Set As
    Developer</span>icon.

Continue with Assign Contacts to Objects.

### <span id="Assign2"></span>Assign Contacts to Objects

To assign multiple contacts to multiple Objects:

1.  Select <span style="font-weight: bold;">Advanced Configuration \>
    Object Contact Configuration</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Bulk User Object
    Assignment</span> icon in the Page toolbar.
    
    **NOTE**: If more than one user record is selected on the
    <span style="font-style: italic;">[Bulk Contact Staging
    Area](../Page_Desc/Bulk_Contact_Staging_Area.htm)</span> page, this
    icon is disabled.
    
    **NOTE**: All users on the <span style="font-style: italic;">Bulk
    Contact Staging Area</span> page display on
    the<span style="font-style: italic;">[Staged
    Contacts](../Page_Desc/Staged_Contacts.htm)</span> page.

3.  Select one, many or all users on the
    <span style="font-style: italic;">Staged Contacts</span> page.
    
    **NOTE**: To select a contiguous range of users, hold down the
    **Shift** key and select the first and last users in the range. To
    select a non-contiguous range of users, hold down the **Ctrl** key
    and select each user.

4.  Select one, many or all Objects on the
    <span style="font-style: italic;">[All
    Objects](../Page_Desc/All_Objects.htm)</span> page.

5.  Click the <span style="font-weight: bold;">Add Contact to
    Object</span> icon in the Page toolbar on the
    <span style="font-style: italic;">All Objects</span> page.

The contacts selected on the <span style="font-style: italic;">Bulk
Contact Staging Area</span> page are assigned to the objects selected on
the <span style="font-style: italic;">All Objects</span> page.

To view the contacts assigned to each Object,
select<span style="font-weight: bold;"> Elements \> Objects \>
Contacts</span>.

To remove a contact from an object, click the
<span style="font-weight: bold;">Remove Contact From Object</span> icon
in the Page toolbar on the <span style="font-style: italic;">All
Objects</span> page.
