+++
title = 'Configure Settings for External Request Scenarios that Create Excel-initiated Requests'
solution = 'Data Quality'
+++

# Configure Settings for External Request Scenarios that Create Excel-initiated Requests

External Request Scenarios that Create Excel-initiated requests require
additional configuration compared to other external request scenarios.
Refer to [Configure Settings for External Data Processing and External
Request
Scenarios](../Config/Configure_Settings_for_External_Data_Processing.htm)
for more information.

### Excel-initiated Template Role Configuration

For the template that uses the external request scenario that creates an
Excel-initiated request, the lowest priority template role cannot have
the same priority as any other role. For the template that uses the
external request scenario that creates an Excel-initiated request, there
cannot be an External Data role defined.

Refer to [Add and Configure Template
Roles](Add_and_Configure_Template_Roles.htm) for more information.

### Excel File Format

Before creating an external request scenario that creates an
Excel-initiated request, a sample Excel file must be created.

This Excel file is added to a template for an external request scenario
that creates an Excel-initiated request. External contacts enter request
data into an Excel file based on this sample Excel file.

A sample Excel file in the proper format must exist, where

  - The first row contains the column names that should be mapped to the
    column names of the table that will be created for the Data Entry
    role for the request.
  - The second row is ignored, and could contain column descriptions to
    assist users when entering data.
  - The third row is the first data record imported into the staging
    table.

After the sample Excel file’s worksheet name has been specified for the
template, the sample Excel file is uploaded and processed. Refer to
[Create an External Request Scenario for an Excel-initiated
Request](Configure_External_Rqst_Scenario_for_Excel_Initiated_Request.htm)
for more information.

### ALLOW EXCEL Check Box

When creating the external request scenario, the ALLOW EXCEL check box
must be enabled on the *Template (External Request Scenario)* page.
Refer to [Create an External Request Scenario for an Excel-initiated
Request](Configure_External_Rqst_Scenario_for_Excel_Initiated_Request.htm)
for more information.

### Map Columns in the Worksheet to Template Columns

As part of the process of creating an external request scenario that
creates an Excel-initiated request, worksheet columns must be mapped to
template columns so that request data can move from the template’s
staging table to the table used for the Data Entry role for the request.

As a result of the mapping, when data is moved from the staging table to
the table used for the Data Entry role for the request, it is either:

  - Copied from the staging table to the table used for the Data Entry
    role for the request <span> </span>or
  - Replaced by a fixed value

Refer to [Map Columns from the Template to Columns from the Excel
File](../../../Migration/Map/Use_Cases/Map_Columns_Template_to_Sprdsht.htm)
for more information.

### Use Custom Rules on Imported Data

Custom rules can be registered to a template-level event that runs on
request data once the request data is imported into the template’s
staging table and before it is moved to the table used for the Data
Entry role for the request.

Custom rules are an optional feature.

Refer to [Create Custom Rules for Excel-initiated
Requests](Create_Custom_Rules_for_Excel_Initiated_Requests.htm) for more
information.
