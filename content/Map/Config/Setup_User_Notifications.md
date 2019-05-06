# Set Up User Notifications

Users can be configured to receive a weekly summary email of changes in
Map and notifications about changes to field mappings, value mappings
and Target and rule creation.  

Users will only receive notifications about changes to Targets and
Sources to which they have access.

  - [Set up Workflow Message Summary
    Users](#Set_up_Workflow_Message_Summary_Users)
  - [Set up Notifications for Map
    Updates](#Set_up_Notifications_for_Map_Updates)

## <span id="Set_up_Workflow_Message_Summary_Users"></span>Set up Workflow Message Summary Users

Users can receive emails detailing a weekly summary of mapping status.

The Map Summary notification is auto-generated on a weekly schedule.

Users can also be set up to receive notifications about changes to field
mappings, value mappings and Target and rule creation. Notifications can
be sent in the form of an email, a message displayed in the Platform, or
both. Refer to [Set up Notifications for Map
Changes](#Set_up_Notifications_for_Map_Updates) for more information.

To set up a user for Map Summary notifications in Console:

1.  Select **Advanced Configuration \> Workflow Message Summary** in the
    *Navigation* pane.

2.  Click the **Users** icon for **Map Summary**.

3.  If a record does not already exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [*View the field descriptions for the Workflow Message Summary User
    page*](../../Console/Page_Desc/WorkFlow_Message_Summary_User.htm)

4.  Select an ID from **User ID** list box.

5.  Click **Save**.

To create custom messages, refer to [Create Custom Workflow
Messages](../../Console/Use_Cases/Create_Custom_Workflow_Messages.htm)
in
Console.

## <span id="Set_up_Notifications_for_Map_Updates"></span>Set up Notifications for Map Updates

Notifications can be sent in the form of an email, a message displayed
in the Platform, or both. Users can receive notifications on errors or
successes only.

Users can also be set up to receive weekly summary notifications of
changes in Map. Refer to for more information.

For Map to send notifications:

  - The Source must be marked for tracking changes in the Target Source
  - The user settings must be configured on the *[User Track
    Changes](../Page_Desc/User_Track_Changes.htm)* page.

**NOTE**: A user can receive messages regarding changes to field
mappings only, value mappings only, Target and rule creation only, or
any combination of the three.

To set up notification settings for users in Map:

1.  Select **Configuration \> User Track Changes** in the *Navigation*
    pane.

2.  Click **Add**.
    
    [View the field descriptions for the User Track Changes
    page](../Page_Desc/User_Track_Changes.htm)

3.  Select the user ID of the user who should receive the notification
    from the **USER ID** list box.
    
    **NOTE**: All users display, regardless of whether they are granted
    security to the current context.

4.  Select the method and type of notifications sent regarding changes
    to field mappings in the **MAPPING CHANGES** list box, if
    applicable.
    
    **NOTE**: Refer to the table below for information about each
    option.
    
    **NOTE**: Notifications are sent when a user clicks Submit on the
    *[Field Mappings](../Page_Desc/Field_Mappings_H.htm)* page.

5.   Select the method and type of notifications sent regarding changes
    to value mappings in the **VALUE MAPPING CHANGES** list box, if
    applicable.
    
    **NOTE**: Refer to the table below for information about each
    option.
    
    **NOTE**: Notifications are sent when a user clicks Save on the
    *[Value Mapping (Legacy to
    Target)](../Page_Desc/Value_Mapping_Legacy_to_Target_H.htm)* page

6.  Select the method and type of notifications sent regarding table and
    rule creation in the **TABLE AND RULE CREATION** list box, if
    applicable.
    
    **NOTE**: Refer to the table below for information about each
    option.
    
    **NOTE**: Notifications are sent when a user clicks Save on the
    *[Target
    Sources](../../Design/Page_Desc/Target_Sources_H_Design.htm)* or the
    *[Targets](../../Design/Page_Desc/Targets_H_Design.htm)* page in
    Target Design.

7.  Click **Save**.

The following options are available when sending notifications for
changes.

|                                    |                                                                                                                                                                                                                                      |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Option                             | Description                                                                                                                                                                                                                          |
| Error.DisplayNoAction              | Users receive a notification via email and a message displayed in the Platform when there is an error related to updates depending on the list box selected.                                                                         |
| Error.DisplayWithAction            | Users receive a notification via email and a message displayed in the Platform when there is an error related to updates depending on the list box selected. The message displays until the user closes it or refreshes the browser. |
| Notification.EmailAndMessage       | Users receive an email and a message displayed in the Platform when there are updates depending on the list box selected.                                                                                                            |
| Notification.EmailOnly             | Users receive an email when there are updates depending on the list box selected.                                                                                                                                                    |
| Notification.MessageOnly           | Users receive a message displayed in the Platform when there is are updates depending on the list box selected.                                                                                                                      |
| Notification.MessageOnlyWithAction | Users receive a message displayed in the Platform when there are updates depending on the list box selected, the message displays until the user closes it or refreshes the browser.                                                 |
| Success.DisplayNoAction            | Users receive a notification via email and a message displayed in the Platform when there are updates depending on the list box selected.                                                                                            |
| Success.DisplayWithAction          | Users receive a notification via email and a message displayed in the Platform when there is an error related to updates depending on the list box selected. The message displays until the user closes it or refreshes the browser. |
