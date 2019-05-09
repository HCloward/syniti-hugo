+++
title = "dspCompose Overview"
weight = 3
layout = "single"
solution = "Data Quality"
+++

# dspCompose™ Overview

dspCompose™ is a generic governance engine used with SAP Master Data
Governance (MDG). It provides industry-specific content and workflows to
initiate process governance scenarios for data domains not already
handled by SAP MDG, such as Human Capital Management (HCM), Bill of
Materials (BOMs), and routings. This strategy results in reduced
development cycle time and faster achievement of master data objectives
while fully leveraging SAP MDG.

dspCompose™ is a workflow-enabled application to govern the entry,
review and approval of a proposed mass change. Users are assigned to
*roles*, which are associated with *templates*. A *template* aligns with
a single BDC or GUI script, an Integrate template, or a custom template,
and can be reused for multiple *requests.* A *request* drives the
workflow process to mass change a single object in SAP.

Refer to [Requests vs. Templates](Config/Requests_vs_Templates) for
more information.

Highly customizable, dspCompose™ can be configured to control user
access to request data and how a request is processed from request data
entry through review and posting to a target system.

A change can be based on a database view utilizing a Where clause, an
Excel spreadsheet, or manual input by the user. BDC and GUI scripts can
be used to update data in a target ERP system such as SAP. Messages are
returned from the target system to show which objects were successfully
updated.

dspCompose™ supports mass change data to be posted to SAP via Integrate,
a BackOffice component used as the posting mechanism and script
repository. Integrate contains all the commands for every BDC and GUI
script used to load data into SAP. Each script represents a mass update
process. Refer to
[Integrate](../../Platform/Integrate/Integrate_Overview) for
detailed information.

## Setup and Configuration for dspCompose™

There are several elements of dspCompose™ that can be configured before
executing a mass change process. These steps should only be completed by
a developer or a system administrator and are dependent upon the
client's setup.

Before getting started with dspCompose™, verify the following steps have
been completed:

1.  [Set Up Security for dspCompose™](Config/Set_Up_Security)
2.  [Configure dspCompose™
    Parameters](Config/Configure_dspCompose_Parameters)
3.  [Configure Global Roles](Config/Configure_Global_Roles)
4.  [Assign a Catalog to a Custom WebApp for Use with
    dspCompose™](Config/Assign_Catalog_Custom_WebApp_for_dspCompose)
5.  [Enable Role Validations](Config/Enable_Role_Validations)
6.  [Update Validation Messages](Config/Update_Validation_Messages)
7.  [Configure Workflow
    Messages](Config/Configure_Workflow_Messages)
8.  [Set up Workflow Messages](Config/Set_up_Workflow_Messages)
9.  [Configure Request Statuses](Config/Configure_Request_Statuses)
10. [Configure Columns to Exclude from Mass
    Change](Config/Configure_Columns_to_Exclude_from_Mass_Change)
11. [Display Posting Options on
    Requests](Config/Display_Posting_Options_on_Requests)
12. [Configure Settings for External Data Processing and External
    Request
    Scenarios](Config/Configure_Settings_for_External_Data_Processing)

When the platform is installed, an Integrate category called
**dspCompose** is created that will act as the repository in Integrate
for all the templates created in dspCompose™.

The category is listed on the *Parameters* page. In dspCompose™, select
**Configuration \> Setup \> Parameters**. The name displays in the
**Integrate Category** field.
