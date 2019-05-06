# External Request Scenarios that Create Information Steward-initiated Requests

<span style="font-weight: bold;">NOTE</span>: Information Steward (IS)
is SAP’s software for data profiling and metadata management. The
Information Steward Accelerator by Back Office Associates® (ISA)
extracts data that failed IS rules, then distributes the data to groups
of users via reports.

An external request scenario can be configured to remediate failed data
from IS reports using dspCompose™. Refer to [Create a Request in
dspCompose™ From the ISA Report Data Viewer
Page](Create_a_Request_in_dspCompose_From_ISA.htm) for more information.

During the request creation process, the report data is copied to a
staging table where dspCompose™ maps the columns and runs any custom
rules (registered as template-level events) on the data. The data is
then moved to the Data Entry table for the dspCompose™ template, and can
be corrected by the first Data Entry role to begin the request posting
process.

To use this type of external request scenario:

1.  Run rules in IS. Refer to Information Steward documentation for more
    information.
2.  Configure the ISA to distribute failed data to users in project
    distributions. Refer to [Work with
    Projects](Work_with_Projects_ISA.htm) for more information.
3.  [Create an External Request Scenario for an Information
    Steward-initiated
    Request](Create_an_External_Request_Scenario_for_an_Information_Steward%20initiated_Request.htm)
    in dspCompose™.
4.  [Map Columns from the Template to Columns from the ISA
    Report](Map_Columns_from_the_Template_to_Columns_from_the_ISA_Report.htm).
5.  [Create Custom Rules for Information Steward-initiated
    Requests](Create_Custom_Rules_for_Information_Steward%20initiated_Requests.htm),
    if needed.

The request is automatically created and dspCompose™ sends a
notification to the user assigned to the first Data Entry role for the
template. At this point, the request moves through the request process
normally.
