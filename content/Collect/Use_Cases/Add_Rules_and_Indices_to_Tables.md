+++
title = 'Add Rules and Indices to Tables'
solution = 'Platform'
+++

# Add Rules and Indices to Tables

Rules and indices are added to tables to clean data (rules) and improve
performance (indices) in the target system.

The rule and index administration includes the following topics:

  - [Register Rules to Tables](#Register_Rules_to_Tables)

  - [Create Indices for Tables](#Create_Indices_for_Tables)

  - [Drop and Recreate an Index](#Drop_and_Recreate_an_Index)

## <span id="Register_Rules_to_Tables"></span>Register Rules to Tables

Rules are registered to a Target Source to change or customize the
Target Source tables. Create new rules using the following naming
convention:
**\[Database\].\[dbo\].\[RulePrefix\]\[TableName\]\_\[FieldName\]\_\[Description\]\[Action\]**,
where

  - **\[Database\]** is the database name. This is required in front of
    each rule name; otherwise, the rule points to the target database,
    e.g., dgSAP.dbo.irMyRuleIsIndgSapDatabase.

  - **\[dbo\]** is the schema owner

  - **\[RulePrefix\]** is the Action Filter stored in the Common \>
    Configuration \> Modules \> Parameters-Collect

  - **\[TableName\]** is the name of the table impacted by the rule.

  - **\[FieldName\]** is the name of the field within TableName impacted
    by the rule.

  - **\[Description\]**is a brief description of the rule’s function.

  - **\[Action\]** is Update (Upd), Insert (Ins) or Delete (Del).

Register the rule after data has been downloaded by the package.

**NOTE:** Collect rules require database and a schema owner prefix for
the rule to process correctly.

To register a rule to a table:

1.  Click **Targets** in
    *<span style="font-size: 11.0pt;">Navigation</span>* pane.

2.  Click **Sources** for Target.

3.  Click **Tables** for Source. 

4.  Click **Rules** for Table.

5.  Click **Add**.
    
    [View the field descriptions for the Table (Rule)
    page](../Page_Desc/Table_Rule_H)

6.  Enter order in which rule runs in **PRIORITY** field.

7.  Enter a rule name in **RULE** field.

8.  Update **RULE TYPE** list box if the default value is not
    applicable. Values are:
    
      - **Rule** – Performed after the data has been downloaded by the
        package
    
      - **Action** – Generic and performed at the field level, where
        rules are customized and can be performed against an entire
        table or single column

9.  Update **PRECEDENCE** list box if the default value is not
    applicable. This field controls the execution order of the rule or
    action. Values are:
    
      - **After –** Rule runs after table is downloaded
      - **Before –** Rule runs before table is downloaded

10. Select a name from **FIELD NAME** list box to control the field
    impacted by action.

11. Click **ADD TARGET DB PARAM** check box to enable it, adding a
    database parameter when running the rule
    
    **NOTE:** Activating the ADD TARGET DB PARAM field is helpful when
    rules are stored in the Collect database and run in another database
    – users are able to clearly see the originating database. 

12. Enter a value in **WHERE CLAUSE** field to limit rule to run on only
    part of the table data.

13. Click **Save**.

14. Click **Vertical View**.

15. Click **Edit**.
    
    [View the field descriptions for the Table (Rule) page's Vertical
    View](../Page_Desc/Table_Rule_H)

16. Enter notes about rule in **Comment** field.

17. Enter client specifications for a custom rule in **Spec ID** field.

18. Click **Save**.

## <span id="Create_Indices_for_Tables"></span>Create Indices for Tables

Indices built during the Create Package process are registered to a
Target Source to improve performance. For the download process to
perform better for large tables, drop and build the indices and/or the
primary key.

Collect has the ability to build indices and primary keys for the target
tables. Indices and primary keys are built with general SQL statements
without considering space allocation or clustering. To use these
features, create a customized rule containing the required SQL view and
run it after a data download. For large tables, it is recommended to
drop the index before downloading the data and to recreate the index
after the data has been reloaded.

**NOTE:** Collect builds SAP Primary Keys during the Build Package
process. Primary keys for source systems are automatically created if
**Download Indices Keys** is enabled for the source. To build keys and
indices for non-SAP sources, verify the Download Keys Indexes check box
on the *[Target Sources](../Page_Desc/Target_Sources_H_Collect)*
page's *Vertical* View is enabled.

To build indices or primary keys for SAP:

1.  Click **Targets** in *Navigation* pane.

2.  Click **Sources** for Target.

3.  Click **Tables** for Source. 

4.  Click **Indices** for Table.

5.  Click **Add**.
    
    [View the field descriptions for the Table (Indices)
    page](../Page_Desc/Table_Indices_H)

6.  Enter a name in **INDEX ID** field.

7.  Click **UNIQUE INDEX** check box to build a unique index.
    
    OR
    
    Click **PRIMARY KEY** check box to build the index as a primary key
    for the tables.

8.  Click **CLUSTERED INDEX** check box to mark the index as
    *clustered*.
    
    **NOTE:** CLUSTERED INDEX can be used with PRIMARY KEY to create a
    clustered or non-clustered primary key.

9.  Click **Save**.

10. Click **Columns** for Indices.

11. Click **Add**.
    
    [View the field descriptions for the Target Source Table Index
    Columns page](../Page_Desc/Target_Source_Table_Index_Columns)

12. Select a value from **COLUMN** list box to indicate the table column
    impacted by the index.

13. Update **COLUMN ORDER** field if the default value is not
    applicable.
    
    <span style="font-weight: bold;">NOTE:</span> The
    <span style="font-weight: bold;">COLUMN ORDER</span> field controls
    the sort order of the column.

14. Click **Save**.

15. Click **Back** button on Browser to return to *Table (Indices)*
    page.

16. Click **Build Indices** icon to schedule the rebuild process for all
    index in Target Source Table index; a confirmation message displays.
    
    **NOTE:** Only indices and keys registered to the table are rebuilt.

17. Click **Ok**.

**NOTE:** Indices are built in the background and may take several
minutes.

## <span id="Drop_and_Recreate_an_Index"></span>Drop and Recreate an Index

In order to fine tune performance of an index, the index must be dropped
and recreated.

To recreate an index:

1.  Click **Targets** in *Navigation* pane.
2.  Click **Sources** for Target.
3.  Click **Tables** for Source. 
4.  Click **Indices** for Table.
5.  Select Indices to rebuild.
6.  Click **Build Indices** icon on Page toolbar to schedule the rebuild
    process for all index in Target Source Table index; a confirmation
    message displays.

**NOTE:** Only registered indices and keys are rebuilt. Indices are
built in the background and may take several minutes.
