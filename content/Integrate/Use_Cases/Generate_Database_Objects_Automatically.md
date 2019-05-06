# Generate Database Objects Automatically

Use Integrate’s optional Auto Generate Database Objects feature to
quickly configure process template loops, relationships, and field
mappings and to create views and tables in the designated database.

**NOTE**: The Auto Generate Database Objects feature is optional. Users
can create and configure database objects manually.

This section provides an overview of the feature. Refer to specific use
case topics describing process template loop configuration, field
mappings, and relationships for more information.

For process template loops for all process templates, regardless of the
template type, Integrate:

  - Populates the **VIEW NAME** column on the *Process Template Loop*
    page for a process template with a single loop with tx\[Process
    Name\] \[Template Name\]Int

  - Populates the **VIEW NAME** column on the *Process Template Loop*
    page for a process template with multiple loops with tx\[Process
    Name\] \[Template Name\] \[Loop Name\]Int

  - Creates a table for a process template with a single loop with the
    name tt\[Process Name\] {Template Name\]\_Upload

  - Creates tables for a process template with multiple  loops with the
    name tt\[Process Name\] {Template Name\] \[Loop Name\]\_Upload

  - Sets the **PRIMARY KEY COLUMN NAME** to ID on the *Process Template
    Loop* page

  - Automatically maps the fields for the process template loop. The
    **TEMPLATE FIELD UNIQUE NAME** and the **MAPPING VALUE** column will
    have the same value on the *Process Template Loop Field Mappings*
    page.

Additionally, for process template loops based on certain template
types, Integrate:

  - Creates a table called tt\[Process Name\] {Template Name\] \[Loop
    Name\]\_Download for a process template based on a BAPI/RFC template

  - Configures relationships for process template loops for BAPI/RFC
    templates and for looped templates (BDC Script and GUI Script)

  - Sets the **DOWNLOAD PRIMARY KEY** column to **ID** for a process
    template based on a BAPI/RFC template

  - Populates the **DOWNLOAD TABLE** column with tt\[Process Name\]
    \[Template Name\] \[Loop Name\]\_Download for a process
    template  based on a BAPI/RFC template

  - Populates the **FLAT FILE OBJECT KEY** column with the text
    FlatFileObjectKey for process templates based on User Defined
    Delimited and Fixed Width templates

**NOTE**: The Flat File Object Key is a unique identifier for an object
that Integrate uses to join the data stored in different tables to make
a complete data set for the object. The data set has two loop levels,
the header and the details. For example, Integrate uses the flat file
object key of 1 in the first loop (the header) to join the header with
detail records stored in tables that also have the flat file object key
of 1. When posting, batch sizes are based on the number of header
records as set by the flat file object key.

**NOTE**: When creating a process that will use the Auto Generate
Database Objects feature, do not select a **View Name** on the *Process*
page’s *Vertical* View. Refer to [Create a
Process](Create_a_Process.htm) for more information.

**NOTE**: Deleting a process that has auto-generated database objects
will also delete those tables and views from the database.

To use the Auto Generate Database Objects feature:

1.  Select **Categories** in *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click the **Templates** icon for a process.

4.  Click the **Loops** icon for a process template.

5.  Click **AutoGenerate Database Objects** on the Page toolbar; a
    confirmation message displays.
    
    **NOTE**: **Auto Generate Database Objects** create stables in the
    data source mapped to the process to serve as data staging for
    Upload and return value targets. It will also create Upload views
    based on the data staging tables. The created objects will be auto
    registered to the Process Template Loops. Auto Generating Database
    Objects will drop and re-create previously auto created objects.

6.  Click **Ok.**

7.  View the updates to the columns on the *Process Template Loop* page.

8.  Click **Relationships** on the Page toolbar if the process template
    is based on a BAPI/RFC template or a BDC Script or GUI Script
    template that has looping enabled to view the relationships.

9.  Navigate to the *Process Template Loop* page.

10. Click the **Field Mappings** icon for a loop.

11. Verify that the **MAPPING VALUE** column is complete for all
    records. The **MAPPING VALUE** and the **TEMPLATE FIELD UNIQUE
    NAME** should be identical.
