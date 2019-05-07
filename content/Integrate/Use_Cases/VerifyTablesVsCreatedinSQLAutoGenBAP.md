+++
title = 'Verify the Tables and Views were Created in SQL by the Auto Generate Process for a BAPI'
solution = 'Platform'
+++

# Verify the Tables and Views were Created in SQL by the Auto Generate Process for a BAPI

<span id="Post Data using a BAPI Steps" class="popUpLink">\>Review the
steps in the process. </span>

If the Auto Generate Database Objects feature was used, confirm that
database objects were created. Access the SQL database to view the views
and tables Integrate created during the auto-generation process.

1.  Log in to SQL Management Studio.

2.  Locate the database assigned to the process.

3.  Locate the views and tables created in the database.
    
    **NOTE:** Integrate creates tables and views in the database for all
    process template loops for a process, including download tables that
    contain the unique identifier Posting ID for those loops that
    contain download fields. It names the tables tt\[Process
    Name\]\[Template Name\]\[Loop Name\]\_Upload and tt\[Process
    Name\]\[Template Name\]\[Loop Name\]\_Download. The View Name for
    each process template is tx\[Process Name\] \[Template Name\] \[Loop
    Name\]\_Int.

4.  Open the Download tables in Design mode and verify that each has a
    PostingID column.
