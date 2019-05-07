+++
title = 'Configure Process Template Loops for an RFC Template'
solution = 'Platform'
+++

# Configure Process Template Loops for an RFC Template

<span id="Post Data using an RFC Steps" class="popUpLink">\>Review the
steps in the process. </span>

A process based on an RFC templates will post data bi-directionally.
Data is uploaded to be posted into SAP, and downloaded into tables that
Integrate automatically creates.  Since processes based on RFC templates
often have return values, download registrations are often required for
RFC templates. 

**NOTE**: RFC template types can use transaction stringing to pass
return values to other templates assigned to a process. Refer to
[*<span style="color: #0000ff;font-style: normal;">Post Data Using
Transaction
Stringing</span>*](Post_Data_Using_Transaction_Stringing.htm) for more
information.

Once the RFC template has been created and added to a process, the
process template loops and database objects must be configured.

Perform these tasks manually or use the optional Auto Generate Database
Objects feature to perform them automatically.

  - Populate the **VIEW NAME** with the view containing the data to
    upload during the post

  - Populate the **PRIMARY KEY COLUMN NAME** with the column in the
    **VIEW NAME** that uniquely identifies a record being uploaded
    
    **NOTE**<span style="color: #1F497D;">:</span> The primary key
    column must be an auto-incrementing Identity column in the database.

<!-- end list -->

  - Populate the **DOWNLOAD TABLE NAME** with the table that will
    receive the return values from the BAPI/RFC execution

  - Populate the **DOWNLOAD PRIMARY KEY** column with the auto
    incrementing identity column in the database that serves as the
    primary key of the Download table

  - Populate the Field Mappings with the fields from the **VIEW NAME**
    for upload loop and Download Table for download loops where data
    should be read from/written to respectively
    
    **NOTE**: Refer to [View and Configure Field Mappings for a Process
    Based on an RFC](VwConfigureFldMappingsProcRFC.htm) for more
    information.

  - Configure the relationships for the all of the loops
    
    **NOTE**: Refer to [View and Configure Relationships for a Process
    Bases on an RFC](VwConfigureRshpsProcRFC.htm) for more information.

**NOTE**: If a process template contains a loop with more than 655
columns (which may occur when working with a BAPI/RFC template type),
select only a few columns to add data to the table corresponding to the
loop when working in SQL. SQL will generate an error if a user attempts
to open a table with more than 655 columns.

Integrate adds a process template loop for each loop in the BAPI
Definition. The loop contains the fields in the definition.

To configure process template loops:

1.  Click **Categories** in the *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click the **Templates** icon for a process

4.  Click the **Loops** icon for a process template.
    
    *[View the field descriptions for the Process Template Loop
    page.](../Page_Desc/Process_Template_Loop.htm)*

**NOTE**: The number of loops displays on the **Loop** icon. 

If creating database objects manually, create the views and tables in
the database before adding the process that will use the BAPI/RFC
template. When adding the process, select the view in the **View Name**
list box on the **General** tab of the *Process* page’s *Vertical* View.
This view name will display for all loops on the *Process Template Loop*
page.

If using the optional Auto Generate Database Objects feature, before
auto generating the database objects, the **VIEW NAME**, **PRIMARY KEY
COLUMN NAME**, **DOWNLOADTABLE** and **DOWNLOADPRIMARYKEY** columns are
blank.  One loop exists for each BAPI/RFC definition.

**NOTE**: The **LOOP NAME** for the first loop is blank and the
**DOWNLOAD TABLE** and **DOWNLOAD PRIMARY KEY** columns are blank. These
columns will remain blank for the primary loop even after the Auto
Generate Database Objects feature is used.

**NOTE**: The **LOOP NAME** for each loop should match the loop names on
the *BAPI/RFC Definitions* page.

To use the optional Auto Generate Database Objects feature:

1.  Click **Auto Generate Database Objects** on the Page toolbar; a
    confirmation message displays.
    
    **NOTE**: Auto Generate Database Objects will create tables in the
    data source mapped to the process to serve as data staging for
    upload and return value targets. It will also create Upload views
    based on the data staging tables. The created objects will be auto
    registered to the Process Template Loops. Auto Generating Database
    Objects will drop and re-create all objects that were previously
    automatically generated.

2.  Click **Ok**.

**NOTE**: The Auto Generate Database Objects feature: 

  - Creates tables and views in the database for all process template
    loops for a process, including download tables that contain the
    unique identifier Posting ID. Names the tables tt\[Process
    Name\]\[Template Name\]\[Loop Name\]\_Upload and tt\[Process
    Name\]\[Template Name\]\[Loop Name\]\_Download
    
    **NOTE**: Database objects may need to be tweaked to align with
    specific data elements in the
    postings.
    
    **<span style="font-size: 10.0pt;font-family: Arial, sans-serif;color: #000000;">NOTE</span>**<span style="font-size: 10.0pt;font-family: Arial, sans-serif;color: #000000;">:
    If a loop does not have Download Fields, Integrate will not create
    a</span> tt\[Process Name\]\[Template Name\]\[Loop Name\]\_Download
    in the database for this loop.

<!-- end list -->

  - Populates the **VIEW NAME** for each process template with
    tx\[Process Name\] \[Template Name\] \[Loop Name\]Int

  - Sets the **PRIMARY KEY COLUMN NAME** to **ID**  
    **NOTE**: The primary key column must be an auto-incrementing
    Identity column in the database. 

  - Automatically maps the fields for the process template loop. The
    **TEMPLATE FIELD UNIQUENAME** and the **MAPPING VALUE** column will
    have the same value on the *Process Template Loop Fields Mappings*
    page.
    
    **NOTE**: Refer to [View and Configure Field Mappings for a Process
    Based on an RFC](VwConfigureFldMappingsProcRFC.htm) for more
    information.

<!-- end list -->

  - Configures relationships for process template loops
    
    **NOTE**: Refer to [View and Configure Relationships for a Process
    Bases on an RFC](VwConfigureRshpsProcRFC.htm) for more information.

<!-- end list -->

  - Sets the **DOWNLOAD PRIMARY KEY** column to **ID**

  - Populates the **DOWNLOAD TABLE** column with tt\[Process Name\]
    \[Template Name\] \[Loop Name\]\_Download
    
    **NOTE**: If creating database objects manually, use the **DOWNLOAD
    TABLE** and **DOWNLOADPRIMARYKEY** fields to configure the
    destination tables for the output from SAP.  The **DOWNLOADTABLE**
    column contains the name of the table to which data will be written
    and the **DOWNLOADPRIMARYKEY** is the Primary Key Column on that
    table.  Neither of these columns is populated for the first loop.
    
    **NOTE**: The **DOWNLOADPRIMARYKEY** column must be set up in the
    database to be auto-incrementing Identity column
