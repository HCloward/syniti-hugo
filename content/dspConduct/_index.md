+++
title = "dspConduct Overview"
weight = 3
layout = "single"
solution = "Master Data Management"
+++

# dspConduct™ Overview

dspConduct™ provides an Application Data Management solution for
governing data business processes across disparate applications and
infrastructures.

dspConduct™ provides the ability to design, execute, and monitor
business processes within an organization as they relate to the creation
and maintenance of data within the enterprise architecture of an
organization. A Designer creates the governance elements hierarchy,
where tasks, roles, scenarios, business processes and their dependencies
are defined.

dspConduct™ enables users to manage the creation of master data. Master
data is collected, validated, reviewed, approved and posted through a
request process that dspConduct™ provides.  A request is comprised of
tasks, roles, and scenarios within a business processes. The processes
are grouped by category (e.g., Material, Customer, Vendor). Users of
dspConduct™ can create their own custom applications and request pages
for any object necessary. The Content WebApp is registered at the
category level within dspConduct™.

A task is a Content WebApp page designed to collect and validate
information required to support the business process. Not all pages are
tasks as some pages can be navigated to as child pages from the main
task page header. Tasks and pages can be enabled to use Microsoft Excel
Interoperability so that they can create or update data for the tasks
within Excel. Refer to [Use Excel
Integration](../../Platform/Excel_Int/Use_Excel_Integration) for
more information.

A role is a collection of tasks and a unit of security where an
individual or groups of individuals perform their duties during a step
or role within the workflow of the business process.

A scenario is a collection of roles that outlines a single sub-process
that can either be an entire business process on its own or just a step
within that business process, containing its own dependencies.  For
example, a user can create a Basic Data for a Finished Good scenario,
while other scenarios within the business process can be created to
extend that same material to plants or sales organizations. 

A business process is a compilation of scenarios that allows a series of
linked scenarios to be created.

A category is a collection of the tasks, roles, scenarios and business
process governance elements and is created to organize the elements by
the category (for example, line of business, business unit or division,
or data domain).

Security setup in dspConduct™ uses positions, which are security
templates defined by a Security Administrator, to which multiple users
can be assigned. With positions, a Security Administrator can create a
template for security once and assign multiple users to the template as
needed. The position security set up is used to establish security for
users in the Content WebApp.

Content WebApps use the governance elements and security setup from
dspConduct™ to manage the process of coordinating data collection,
validating the data and posting information. dspConduct™ also provides
the ability to ensure that only resources that have been explicitly
given access can create, read, update and delete data.

dspConduct™ supports mass change data to be posted via Integrate, a
BackOffice Associates® component used as the posting mechanism and
script repository. Refer to
[Integrate](../../Platform/Integrate/Integrate_Overview) for
detailed information.

Documents can be attached to governance elements to provide instructions
and supporting documentation that communicates information to users of
the governance process about how to work with certain elements. Refer to
[Upload and Download Element
Documentation](Use_Cases/Upload_and_Download_Element_Documentation)
for more information.

A dashboard is available in dspConduct™ with charts that show metrics
for velocity and efficiency in roles processing. Refer to [View Charts
in dspConduct™](Use_Cases/View_Charts) for more information.

## Setup and Configuration for dspConduct™

Before using dspConduct™, ensure the following tasks are completed, if
applicable.

  - [Set Up Security for
    dspConduct™](Config/Set_Up_Security_for_dspConduct)
  - [Assign a Backup User](Config/Assign_a_Backup_User)
  - [Set User Workflow Receipt
    Preferences](Config/Set_User_Workflow_Receipt_Preferences)
  - [Configure Workflow Messages
    Overview](Config/Configure_Workflow_Messages_Overview)
  - [Set up SLA Notifications in
    dspConduct™](Config/Set_Up_SLA_Notifications)
  - [Configure SLA settings at the Business Process Scenario Role
    Level](Config/Configure_SLA_Settings_at_the_BPSR_Level)
  - [Set Up Service Pages for Service Level Agreements (SLA) in
    dspConduct™](Config/Set_Up_Service_Pages_for_SLAs)
  - [Set Preceding Weeks Count for
    Dashboards](Config/Set_Preceding_Weeks_Count_for_Dashboards)
  - [Set Currency Display Label](Config/Set_Currency_Display_Label)
  - [Set Calendar Used For Business Value
    Calculations](Config/Set_Calendar_Used_For_Business_Value_Calculations)
  - [Manage Request Statuses](Config/Manage_Request_Statuses)

<span style="font-weight: bold;">NOTE:</span> A new data source named
DGE\_ElementDocument\_FilePath whose data source type is “Local File” is
shipped with dspConduct™. Once dspConduct™ has been installed the Path
value must be populated for that DataSource. The Path value is a folder
that already exists on the web server and is the "root" of the path
where all Element Documents are stored on the web server.
