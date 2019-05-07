+++
title = 'Configure SLA settings at the Business Process Scenario Role Level'
solution = 'Data Quality'
+++

# Configure SLA settings at the Business Process Scenario Role Level

A Designer can configure SLA settings at the Business Process Scenario
Role level. The SLA settings are inherited from the settings at the
scenario \> role level, but can be configured for the business process
scenario \> role combination. Refer to [Setting up SLA notifications in
dspConduct™](Set_Up_SLA_Notifications.htm) for more information about
the prerequisites for setting up SLAs and how the SLAs work at the
various levels for dspConduct™ elements.

**NOTE**: When a role is imported from IGC™ and the SLA fields are blank
in dspConduct™, the values entered in IGC™ are used at the scenario role
level and the business process scenario role level. If the fields
already contain values in dspConduct™, the SLA values are not updated at
these levels. At the role level, the SLA values are updated when a role
is imported from IGC™ with SLA data whether the fields have values in
dspConduct™ or not.

dspConduct™ default Calendar’s Work Days, Work Hours, and Exceptions are
used in the calculations of these due dates. Refer to [Use a
Calendar](../../../Platform/Common/Use_Cases/Use_a_Calendar.htm) for
more information on configuring dspConduct™ default calendar.

To configure SLA settings:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Design** in the *Navigation* pane; the Category page
    displays.

2.  Click the **Business Processes** icon for a category.

3.  Click the **Scenarios** icon.

4.  Click **Roles SLA**.

5.  Click **Edit**.
    
    *[View the field descriptions for the Business Process (Scenarios
    Roles) page](../Page_Desc/Business_Process_Scenario_Roles.htm)*

6.  Enter the number of days to execute all of the tasks in this
    business process \> scenario \> role combination in the **Work
    Days** field.

7.  Enter the number of hours to execute all of the tasks in this
    business process \> scenario \> role combination in the **Work
    Hours** field.

8.  Enter the number of minutes to execute all of the tasks in this
    business process \> scenario \> role combination in the **Work
    Minutes** field.

9.  Click **Save**.
