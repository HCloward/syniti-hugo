+++
title = 'Create Groups'
solution = 'Data Quality'
+++

# Create Groups

Create a group to control report access by user. Reports are configured
by group to allow report settings to differ by group.

To create a group:

1.  Select **Configuration \> Groups** in *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Groups
    page](../Page_Desc/Groups_H.htm)

3.  Enter a group name (without spaces) in **GROUP ID** field. 

4.  Enter a brief description about group in **GROUP DESCRIPTION**
    field.

5.  Select an owner from **GROUP OWNER** list box.
    
    **NOTE:** The Group Owner manages reports registered to the group
    and defines the report-level parameters. Only users created and
    registered in System Administration display in the GROUP OWNER list
    box. When the group is created, the Group Owner is automatically
    registered as a user for the group.

6.  Select schedule from **GROUP SCHEDULE ID** list box to determine how
    often reports are run for each user in the group.
    
    **NOTE:** Schedules are maintained in Common. Refer to [Create
    Schedules](../../../Platform/Common/Use_Cases/Create_Schedules.htm)
    for detailed information.

7.  Select a schedule from **WORKFLOW SCHEDULE ID** list box to
    determine how often workflow emails are sent to every user in the
    group.
    
    **NOTE:** Workflow schedules can be overridden at the group user
    level to increase the frequency of workflow emails. These schedules
    are configured in Common \> Tools \> Schedules.

8.  Click **Save**.

9.  Click **Vertical View** to enter a threshold ID for data quality
    scoring (optional).

10. Click **Edit**.
    
    [View the field descriptions for the Groups page's Vertical
    View](../Page_Desc/Groups_H.htm#Groups_V_All_Tabs)

11. Select a threshold from the **Threshold ID** list box.

12. Click **Save**.
