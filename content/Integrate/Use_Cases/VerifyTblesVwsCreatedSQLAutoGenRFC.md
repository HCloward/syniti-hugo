# Verify the Tables and Views were Created in SQL by the Auto Generate Process for an RFC

<span id="Post Data using an RFC Steps" class="popUpLink">\>Review the
steps in the process. </span>

If the Auto Generate Database Objects feature was used, confirm that
database objects were created.

<span style="font-weight: bold;">NOTE:</span> This use case provides an
example of posting using the
<span style="font-weight: bold;">RFC</span>**BOA/ZRFC\_READ\_TABLE –
External access to R/3 tables via RFC**, but does not supply
comprehensive instructions to suit all RFCs.

Access the SQL database to view the views and tables Integrate created
during the auto-generation process.

1.  Log in to SQL Management Studio.

2.  Locate the database assigned to the process.

3.  Locate the views and tables created in the database.
    
    **NOTE**: Integrate creates tables and views in the database for all
    process template loops for a process, including download tables that
    contain the unique identifier Posting ID for those loop s that
    contain download fields. It names the tables tt\[Process
    Name\]\[Template Name\]\[Loop Name\]\_Upload and tt\[Process
    Name\]\[Template Name\]\[Loop Name\]\_Download. The View Name for
    each process template is tx\[Process Name\] \[Template Name\] \[Loop
    Name\]Int.

4.  Open the Download tables in Design mode and verify that each has a
    PostingID column.

5.  Open the table created for the primary loop.

6.  Add records to the table. In the example, the following fields were
    populated.
    
      - ID – Leave blank as this will be auto-created.
    
      - Cross\_Client – Enter a single space
    
      - Delimiter – Enter **|**
    
      - No\_Data – Enter a single space
    
      - Query\_Table – Enter T001W
    
      - Rowcount – Enter 0
    
      - Rowskips – Enter 0
        
        In the example, the step above is repeated for Query\_Table –
        KNA1.and for Query\_Table – TVKO.

7.  Close the table.
