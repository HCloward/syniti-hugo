+++
title = 'Add a Role'
solution = 'Master Data Management'
+++

# Add a Role

Before performing these steps, [Create a
Category](Create_a_Category).

This task is performed by a Designer.

Refer to [Manage Roles](Manage_Roles) for general information about
roles.

To add a role in dspConduct™:

1.  Select **dspConduct \> Design** in the *Navigation* pane.

2.  Click the **Roles** icon for a category.

3.  Click **Add**.
    
    *[View the field descriptions for the Role
    page.](../Page_Desc/Role_H_dspConduct)*

4.  Enter a unique name for the role in the **NAME** field.

5.  Enter a brief description of the role in the **DESCRIPTION** field.

6.  Enter the order the role displays on the Role page in the
    **PRIORITY** field.

7.  Click **Save**; *Vertical* View displays.

8.  Select an owner of the role in the **Owner** list box.

9.  Select a type from the **Role Type** list box.
    
    **NOTE**: Values are:
    
      - **Application** – Gathers, enters or makes changes to data using
        pages in the Content WebApp for preparation to send to the
        system(s) of record
      - **Display** – Views data but is unable to make changes. Users
        assigned to a role with a Display role type are not active
        participants in the process.
      - **Review** – Evaluates and reviews data, either approving or
        rejecting all changes made within the execution of a request.
        Data can be viewed but not modified. A role with this role type
        can also review the tasks of their dependent application roles
        within a scenario. Refer to [Review a Request
        Overview](Post_a_Request) for more information.
      - **Post** – Posts data to a target system after the roles with
        Application and Review role types have been completed. Refer to
        [Post a Request](Post_a_Request#Post_a_Request) for more
        information.
      - **ManualPost** – Performs work outside of dspConduct™ by using a
        custom posting process or performing a physical task. Refer to
        [Use Manual Post](Post_a_Request#Use_Manual_Post_) for more
        information.

10. Click the **Send Workflow** check box to disable or enable it as
    needed.
    
    **NOTE**: If enabled, the users assigned to the role receive message
    and notifications as the request moves through the workflow. Refer
    to [Enable or Disable Messages for a
    Role](Enable_or_Disable_Messages_for_a_Role) for more
    information.

11. Click the **Auto Extend Display** check box to disable or enable it
    as needed.
    
    **NOTE**: If enabled, the tasks within the role display as read only
    to all other users within the scenario who are not assigned to this
    role.

12. Enter the number of days to execute all of the tasks in this role in
    the **Work Days** field.
    
    **NOTE**: This value is tracked for time tracking against a Service
    Level Agreement (SLA). Refer to [Set up SLA notifications in
    dspConduct™](../Config/Set_Up_SLA_Notifications) for more
    information.

13. Enter the number of hours to execute all of the tasks in this role
    in the **Work Hours** field.

14. Enter the number of minutes to execute all of the tasks in this role
    in the **Work Minutes** field.

15. Click the **Documentation** icon to upload documentation regarding
    the role.
    
    **NOTE**: Documentation can be attached to the role to provide
    additional instructions for the role. A document can also be
    uploaded and exposed during execution of the role. Refer to [Upload
    Documentation at the Role
    Level](Download_Documentation_at_the_Role_Level) for more
    information.

16. Enter text in the Com**ment field.**
    
    **NOTE**: This field is a free-form text field and is not validated.

Click **Save**.

Continue with [Add a Task to a Role](Add_a_Task_to_a_Role) or [Add a
Scenario](Add_Scenario).
