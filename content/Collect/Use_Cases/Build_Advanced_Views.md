+++
title = 'Build Advanced Views'
solution = 'Platform'
+++

# Build Advanced Views

Advance build is used to store View Builds and to join in Transform
Param settings for runtime settings instead of using a hard-coded value
in a Where Clause. The Advance Build feature is primarily used for Data
Migration Teams that require a parameter table built into the process
and to retain views built.

To use the advance build feature:

1.  Select **Tools \> Advanced View Builder** in
    *<span style="font-size: 11.0pt;">Navigation</span>* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Advanced View Builder
    page](../Page_Desc/Advanced_View_Builder_H)

3.  Select a database where the rules will be created from **DATABASE
    FOR VIEWS** list box. This database cannot be the same as database
    selected for DATABASE FOR TABLES.

4.  Select a database where the views read table data from **DATABASE
    FOR TABLES** list box. This database cannot be the same as database
    selected for DATABASE FOR VIEWS.

5.  Click <span style="font-weight: bold;">TRANSFORM</span>**PARAM
    TABLE** check box if the table is a view or a table in the Database
    For Views database and SQL joins will be created in the view linking
    Transform Param to the source table.
    
    **NOTE:** If using SAP, the TRANSFORM PARAM TABLE must have the
    following columns: SAPCLIENT, SAPLANGUAGE and SAPINSTANCE. If these
    columns are not found, the table will be excluded from the Build
    View process. 

6.  Enter a client in **SAP CLIENT** field to add the Client to the
    Where clause.
    
    **NOTE:** The SAP CLIENT value is only used when TRANSFORM PARAM
    TABLE is unchecked.

7.  Enter a language in **LANGUAGE** field add the Language to the Where
    clause. Use “E” for English.
    
    **NOTE:** The <span style="font-weight: bold;">LANGUAGE</span> value
    is only used when <span style="font-weight: bold;">TRANSFORM PARAM
    TABLE</span> is unchecked.

8.  Select a value from **GROUP FOR VIEWS** list box where only the
    active tables in the group will have views created.
    
    **NOTE:** Leave the <span style="font-weight: bold;">GROUP FOR
    VIEWS</span> field blank to build a view for all tables in the
    <span style="font-weight: bold;">DATABASE FOR TABLES</span> field.

9.  Click **Save**.

10. Select the View.

11. Click **Build View** on Page toolbar; a confirmation message
    displays.

12. Click **Ok**.
