+++
title = 'Set Up SLA Notifications'
solution = 'Master Data Management'
+++

# Set Up SLA Notifications

A Service Level Agreement (SLA) establishes a time constraint for
completing tasks within a request role when a request is processed in
dspConduct™. Users assigned to roles are notified through workflow
messages when a time constraint is not met. A Designer performs the
following tasks to set up SLA notifications for dspConduct™:

  - dspConduct™ is delivered with a default calendar named
    dspConduct. Before SLAs can be configured in dspConduct™, this
    calendar must be configured for working days, working hours, and
    holidays specific to a client site, and dspConduct™ users must be
    added to the calendar in Common. Refer to [Use a
    Calendar](../../../Platform/Common/Use_Cases/Use_a_Calendar) for
    more information.
  - Once the calendar is set up in Common, SLA settings can be
    configured in dspConduct™ at the following levels:
      - Role – Refer to [Add a Role in
        dspConduct™](../Use_Cases/Add_a_Role) for more
        information.
      - Scenario \> Role – The SLA settings are inherited from the
        settings at the role level, but can be configured for the
        scenario \> role combination. Refer to [Add a Role to a
        Scenario](../Use_Cases/Add_a_Role_to_a_Scenario) for more
        information.
      - Business Process \> Scenario \> Role – The SLA settings are
        inherited from the settings at the scenario \> role level, but
        can be configured for the business process scenario \> role
        combination. Refer to [Configure SLA settings at the Business
        Process Scenario Role
        Level](Configure_SLA_Settings_at_the_BPSR_Level) for more
        information.

<span style="font-weight: bold;">NOTE:</span> The work minutes, work
hours, and work days set at the role level, scenario \> role level or
business process \> scenario \> role level are used to calculate the
amount of time that a given role takes to process.<span> </span>When a
request is submitted and its first role becomes available for
processing, that role’s due date is calculated. When the role is
finished, the due dates for the next roles that were dependent upon that
role being finished are calculated. On a daily basis, a Service page
executes and determines which roles’ due dates are less than the current
time. All users for those late roles receive the Late Notification
email.

  - Once the dspConduct™ calendar is set up and the SLA settings are
    configured as needed in the Design hierarchy, Language-specific
    Workflow Messages for the LateSummary or LateNotify event are
    created, if needed. Refer to [Create Language-specific Workflow
    Messages](Create_Language-specific_Workflow_Messages_for_a_Category)
    for more information.

**NOTE:** The Request SLA Notification Service page, Request SLA
Notification Workflow Service, and Request SLA Summary Workflow page
must be configured properly to enable SLA notification to execute. Refer
to [Set Up Service Pages for Service Level Agreements
(SLA)](../../../Platform/Sys_Admin/Use_Cases/Set_Up_Service_Pages_for_Service_Level_Agreements_SLA_in_System_Administration)
in System Administration for more information.

Refer to [Configure Workflow Messages
Overview](Configure_Workflow_Messages_Overview) for general
information about working with workflow message in dspConduct™.
