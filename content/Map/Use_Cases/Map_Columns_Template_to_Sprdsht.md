+++
title = 'Map Columns from the Template to Columns from the Excel File'
solution = 'Migration'
+++

# Map Columns from the Template to Columns from the Excel File

Once an external request scenario for an Excel-initiated request has
been created and the Excel file to be used with the scenario has been
uploaded and processed, the columns in that Excel file must be mapped to
columns in the staging table.

As a result of the mapping, when request data (submitted in an Excel
file by an external contact) is moved from the staging table to the
table used for the Data Entry role for the request, it is either:

Copied from the staging table to the table used for the Data Entry role
for the request or

Replaced by a fixed value

**NOTE**: An Excel file must have been successfully processed for the
scenario prior to performing these steps. Refer to [Create an External
Request Scenario for an Excel-initiated
Request](../../../Data_Quality/dspCompose/Use_Cases/Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel)
for more information.

**NOTE**: If a template uses an external request scenario that creates
Excel-initiated requests, that template cannot be activated until at
least one of the columns in the Excel file has been mapped to the
template columns on the *Template (External Request Scenario Column)*
page.

<span style="font-weight: bold;">NOTE</span>: Columns should always be
mapped for the role with the lowest priority. If columns have been
mapped to the Excel file, a new role with a lower priority than the role
for which columns have been mapped cannot be added. For example, the
Data Entry role has a priority of 20 on a template and template columns
have been mapped to the Excel file for the External Request Scenario for
this Data Entry role. A Template Administrator cannot add a role with a
lower priority than 20 to the template.

To map columns in an Excel file to template columns:

1.  Select **Team** in the *Navigation*<span>pane</span>.
2.  Click **Templates** for a team.
3.  Click **Vertical View** for a template that uses an external request
    scenario to produce Excel-initiated requests.
4.  Click **Configuration** tab.
5.  Click **External Request Scenarios**.
6.  Click **Vertical View** for a scenario that has the **EXCEL
    ALLOWED** check box enabled.
7.  Click the **Advanced** tab.
8.  Click **Map Sheet Columns**.

**NOTE**: The Map Sheet Columns icon is only active once the following
two criteria are met:

  - An Excel file has been successfully processed for this
    scenario.<span> </span> Refer to [Create an External Request
    Scenario for an Excel-initiated
    Request](../../../Data_Quality/dspCompose/Use_Cases/Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel)
    for more information.
  - The Template has been generated. Generate a template on the
    *Templates* page’s *Vertical* View on the General tab.

**NOTE**: See the following two sets of steps for instructions to map a
column from the Excel file to a column in the template or to map a fixed
value to the template column.

To map a column from the Excel file to a column in the template:

1.  From the *Template (External Request Scenario Column)* page, click
    **Edit** for a **COLUMN NAME**.
    
    [View the field descriptions for the *Template (External Request
    Scenario Column)*
    page](../../../Data_Quality/dspCompose/Page_Desc/Template_External_Request_Scenario)
    
    **NOTE:** The COLUMN NAME is the name of the table’s column in the
    template.

2.  Select a column from the **STAGING COLUMN NAME** list box.
    
    **NOTE:** The options in the STAGING COLUMN NAME list box are the
    column names from the Excel file.

3.  Click **Save**.

To map a column from the Excel file to a fixed value:

1.  From the *Template (External Request Scenario Column)* page, click
    **Edit** for a **COLUMN NAME**.
    
    [View the field descriptions for the *Template (External Request
    Scenario Column)*
    page](../../../Data_Quality/dspCompose/Page_Desc/Template_External_Request_Scenario_Column)
    
    **NOTE:** The COLUMN NAME is the name of the table’s column in the
    template.

2.  Click the **STAGING COLUMN NAME** list box.

3.  Enter the fixed value in the filter field that displays above the
    options.
    
    **NOTE:** A fixed value must be surrounded by single quotation marks
    (e.g., ‘10’).

4.  Press the Enter key.

5.  Click **Save**.

When submitting an Excel file for an Excel-initiated request, the
request uses the fixed value for this column in the table used for the
first Data Entry role for the request.
