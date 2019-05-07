+++
title = 'Add a Position'
solution = 'Master Data Management'
+++

# Add a Position

A Security Administrator can add a position to configure the business
processes, roles, and org units that a user assigned to that position
can access.

<span style="font-weight: bold;">NOTE:</span> A user must belong to the
Users Manager WebApp Group in <span>dspConduct™</span> to configure
security for <span>dspConduct™</span> users.

Position security is used to establish security for users in the Content
WebApp.

**NOTE:** When positions are changed in dspConduct™, the changes
automatically result in changes to what business processes, roles, and
data the users can access in the Content WebApp.

Before performing this task, design the governance elements in
dspConduct™ \> Design. Refer to <span>[dspConduct™ Design Process
Overview](dspConduct_Design_Process_Overview.htm)</span> for more
information.

To add a position in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Security \> Positions** in the *Navigation* pane.

2.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    *[View the field descriptions for the Position
    page.](../Page_Desc/Position.htm)*

3.  Enter a name for the position in the **NAME** field.

4.  Enter a description for the position in the **DESCRIPTION** field.

5.  Select a calendar from the **CALENDAR** list box.

6.  Enter an expiration date for the position in the **EXPIRATION DATE**
    field (optional).
    
    **NOTE:** When the date entered is past, the position is considered
    expired, and the security settings for the position are removed for
    the users assigned to the position.

7.  Click **Save**.

Next, [configure business processes in a
position](Configure_Business_Processes_in_a_Position.htm).
