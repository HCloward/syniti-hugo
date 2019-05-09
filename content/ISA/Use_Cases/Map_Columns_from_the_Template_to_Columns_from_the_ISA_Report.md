# Map Columns from the Template to Columns from the ISA Report

<span style="font-weight: bold;">NOTE</span>: Information Steward (IS)
is SAP’s software for data profiling and metadata management. The
Information Steward Accelerator by Back Office Associates® (ISA)
extracts data that failed IS rules, then distributes the data to groups
of users via reports.

<span style="font-weight: bold;">NOTE</span>: During the request
creation process, columns from the ISA report are mapped to columns in
the staging table. The template must have already been recorded and
generated to map columns. Generate a template on the
<span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">Templates</span> page on the General
tab.

Once an external request scenario for an Information Steward-initiated
request has been created and the staging table has been built, the
columns in the template must be mapped to columns in the staging table;
staging table columns are the same columns as in the ISA report.

As a result of the mapping, when the ISA report is processed and the
request data is moved from the staging table to the table used for the
Data Entry role for the request, it is either:

Copied from the staging table to the table used for the Data Entry role
for the request or

Replaced by a fixed value

<span style="font-weight: bold;">NOTE</span>: If a template uses an
external request scenario that creates Information Steward-initiated
requests, that template cannot be activated until at least one of the
columns in the staging table has been mapped to a template column on the
<span style="font-style: italic;">Template (External Request Scenario
Column)</span> page.

To map columns in the staging table to template columns:

1.  Select <span style="font-weight: bold;">Team</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Templates</span> for a team.

3.  Click <span style="font-weight: bold;">ISA External Request
    Scenarios</span> for a template.

4.  Click <span style="font-weight: bold;">Vertical View</span> for the
    scenario.

5.  Click <span style="font-weight: bold;">Map Columns</span>.
    
    <span style="font-weight: bold;">NOTE</span>: The Map Columns icon
    is only active after the template has been generated. Generate a
    template on the <span style="font-style: italic;">Templates</span>
    page’s <span style="font-style: italic;">Vertical</span> View on the
    General tab.
    
    <span style="font-weight: bold;">NOTE</span>: See the following two
    sets of steps for instructions to map a column from the staging
    table to a column in the template or to map a fixed value to the
    template column.

To map a column from the staging table to a column in the template:

1.  From the <span style="font-style: italic;">Template (External
    Request Scenario Column)</span> page, click
    <span style="font-weight: bold;">Edit</span> for
    a<span style="font-weight: bold;"> COLUMN NAME</span>.
    
    [View the field descriptions for the Template (External Request
    Scenario Column)
    page](../../dspCompose/Page_Desc/Template_External_Request_Scenario_Column)

<!-- end list -->

1.  The COLUMN NAME is the name of the table’s column in the template.

2.  Select a column from the <span style="font-weight: bold;">STAGING
    COLUMN NAME</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: The options in the
    STAGING COLUMN NAME list box are the column names from the ISA
    report.

3.  Click <span style="font-weight: bold;">Save</span>.

To map a column from the staging table to a fixed value:

1.  From the <span style="font-style: italic;">Template (External
    Request Scenario Column)</span> page, click
    <span style="font-weight: bold;">Edit</span> for a
    <span style="font-weight: bold;">COLUMN NAME.</span>
    
    [View the field descriptions for the Template (External Request
    Scenario Column)
    page](../../dspCompose/Page_Desc/Template_External_Request_Scenario_Column)
    
    <span style="font-weight: bold;">NOTE</span>: The COLUMN NAME is the
    name of the table’s column in the template.

2.  Click the <span style="font-weight: bold;">STAGING COLUMN
    NAME</span> list box.

3.  Enter the fixed value in the filter field that displays above the
    options.
    
    <span style="font-weight: bold;">NOTE</span>: A fixed value must be
    surrounded by single quotation marks (e.g., ‘10’).

4.  Press the <span style="font-weight: bold;">Enter</span> key.

5.  Click <span style="font-weight: bold;">Save</span>.

When processing data from an ISA report for an Information
Steward-initiated request, the request uses the fixed value for this
column in the table used for the first Data Entry role for the request.

Refer to [Create a Request in dspCompose™ from the ISA Report Data
Viewer Page](Create_a_Request_in_dspCompose_From_ISA) for more
information.
