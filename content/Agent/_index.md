+++
title = "Agent Interface Overview"
weight = 3
layout = "single"
solution = "Platform"
+++

# Agent Interface Overview

The Migration dashboard, visible in the IGC™, provides visibility into
progress and status associated with enterprise Data Migration efforts by
giving you access to the most important migration project metrics.

Using this dashboard you can:

  - Understand the current status of migration waves
  - Identify any waves that are running behind schedule
  - Ascertain go-live readiness for a wave

Before waves, milestones and threshold data can display on the Migration
dashboard, each must be configured in the DSP®.

If there are multiple DSP instances, these steps must be performed on
all instances. The data displays on the same Migration dashboard in the
IGC. Contact [support](http://support.boaweb.com/) for assistance if
setting up the dashboard for this setup.

Data is sent to the Migration dashboard when:

  - A wave has been created and added to the Migration dashboard by
    following the steps in [Configure the IGC™ Migration
    Dashboard](Use_Cases/Configure_the_Migration_Dashboard.htm)
  - A wave that has been added to the Migration dashboard has the name,
    description, start date or end date updated on the
    *[Waves](../../Migration/Console/Page_Desc/Waves_H.htm)* page
  - A wave is deleted in Console
  - A Start Date or End Date milestone is created by the system when a
    wave is added to the dashboard when the Send Wave and Milestone
    Metrics check bock is checked on the [Wave
    Identification](Page_Desc/Wave_Identification_H.htm) page
  - A milestone is created by the user
  - A milestone is updated by the user
  - A user-created milestone is deleted

**NOTE:** You need an additional license to access the Agent Interface
and the Migration dashboard. Contact your BOA Sales contact for more
information. If you do not have contact information, then submit a
request in the [Product Support site](http://support.boaweb.com/) or the
[Data Insiders Community](../../Data%20Insiders%20Community.htm).

**NOTE:** To access the Agent Interface,  a user must belong to the
Agent Interface WebApp Group. Refer to [WebApp
Groups](../Sys_Admin/Use_Cases/WebApp_Groups.htm) and [Assign Users to
WebApp Groups](../Sys_Admin/Use_Cases/Assign_Users_to_WebApp_Groups.htm)
for more information.

**NOTE:** The Agent Interface, used to configure the dashboard, must be
installed. Refer to [Set up and Configuration for a BackOffice IGC
Agent](Config/Set_up_and_Configuration_for_a_BackOffice_IGC_Connector_Agent%20Interface.htm)
for more information.

To install and configure the Agent Interface:

  - [Install a BackOffice IGC
    Agent](Config/Install_the_BackOffice_IGC_Connector_Agent_Service.htm)
  - [Add a BackOffice IGC Agent URL in
    DSP](Config/Add_a_BackOffice_IGC_Connector_Agent_URL_in_DSP.htm)
  - [Test a BackOffice IGC Agent Connection in
    DSP](Config/Test_a_BackOffice_IGC_Agent_Connection_in_DSP.htm)
