+++
title = 'Register the CompareIns Stored Procedure'
solution = 'Data Quality'
+++

# Register the CompareIns Stored Procedure

Before performing this task, [Configure the Comparison Approval
Setting](Configure_the_Comparison_Approval_Setting).

Next, register the CompareIns stored procedure to the Finish event for
the Data Entry Role. The procedure will then run when the Data role user
clicks the **Finish** button on the *Request (Roles)* page.

Refer to [Sample Stored Procedure For Comparison
Approval](Sample_Stored_Procedure_for_Comparison_Approval)  for more
information.

To register the CompareIns stored procedure:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Events** for the Data role.

5.  Click **Rules** next to the Finish event.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click Add.
    
    [View the field descriptions for the Template (Role Event Rule)
    page](../Page_Desc/Template_Role_Event_Rule)

6.  Enter a number in the **PRIORITY** field.
    
    **NOTE**: If multiple template role events are assigned, the
    priority determines the order the rules are run.

7.  Select <span style="font-weight: bold;">dspCompose\_Data</span> from
    the **DATA SOURCE ID** list box.

8.  Select
    <span style="font-weight: bold;">web\[dspComposetemplatename\]CompareIns</span>
    from the **RULE** list box.

9.  Click **Save**.

Continue with [Create a Request for Comparison
Approval](Create_a_Request_for_Comparison_Approval).
