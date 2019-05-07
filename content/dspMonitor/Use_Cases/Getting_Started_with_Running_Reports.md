+++
title = 'Getting Started with Running Reports'
solution = 'Data Quality'
+++

# Getting Started with Running Reports

dspMonitor™ is the analytical component of the DSP® that facilitates
reporting on and maintaining high quality master data. dspMonitor™ is
delivered with a set of over 500 reports to help clients report on the
quality of their data in SAP and to find errors, inconsistencies and
referential integrity issues in master data. In addition, dspMonitor™
supports the ability to add custom reports.

**NOTE:** SAP is a highly configurable application that is implemented
in a unique manner for each client. To allow for the required
flexibility, many of the reports are built upon configurable tables that
must be maintained in order for the reports to run properly.

To get started with running reports in dspMonitor™, verify the following
steps have been completed.

1.  Set up security to
    [Collect](../../../Platform/Collect/Use_Cases/Register_and_Use_Targets.htm#Assign_Target_Security)
    and [dspMonitor™](../Config/Set_Up_Security_for_dspMonitor.htm).

2.  Create a database for the source. Refer to SQL Server documentation
    for detailed information.

3.  [Create and register a report
    repository](../../../Platform/Common/Use_Cases/Data_Sources_in_Common.htm),
    which is referred to as a data source in Common, for the database.
    This step is performed by an Administrator.

4.  [Create report view(s) in the database.](Create_Reports.htm)

5.  [Register the Report Repository in
    dspMonitor™](Register_Report_Repositories.htm).

6.  <span>[Set up group owners](Group_Owner_Responsibilities.htm) and
    [user
    filters](Configure_User_Settings_Reports_and_Filters.htm#Define_Filters)
    in dspMonitor™.</span>

7.  If necessary, download the delivered .zip file for Information
    Steward registrations and load those into IS. Refer to SAP
    Information Steward Integration for detailed information.
