+++
title = 'Set up Table Download with a CranPort Package'
solution = 'Platform'
+++

# Set up Table Download with a CranPort Package

A CranPort package is the method to import data from and to export data
to SQL Server, Oracle, ODBC/OleDB databases, fixed width and delimited
text files, and Excel spreadsheets.

CranPort is the recommended package type to refresh targets tables with
source data because it is SQL Server version independent. Additionally,
SSIS and DBMoto® package types require additional components to be
installed in order to function correctly.

**NOTE:** To receive a workflow email that a table download has failed
in Collect, a user must be assigned to a security role that has the
Collect WebApp group WorkFlowFailureAll or WorkFlowFaiureByTargetAccess
assigned. Refer to [Set
Security](../../Sys_Admin/Use_Cases/Setting_security.htm) in System
Administration for more information.

There are two types of CranPort packages:

  - **[CranPort](#Set_up_Download_with_CranPort_Package)** – a CranPort
    package will be created automatically in Assemble and registered to
    the table.

  - **[ManualCranPort](#Set_up_Download_with_ManualCranPort_Package)** –
    a CranPort package must be manually created in Assemble and
    registered to the table. A ManualCranPort package is used to load
    flat files or sources for which Collect cannot read the schema
    information.

## <span id="Set_up_Download_with_CranPort_Package"></span>Set up Download with CranPort Package

To set up a table download with a CranPort package:

1.  Click **Tables** in
    *<span style="font-size: 11.0pt;">Navigation</span>* pane to view
    all tables registered to all sources.

2.  Click **Add**.
    
    [View the field descriptions for the Tables
    page](../Page_Desc/Tables_H.htm)

3.  Select target database from **TARGET** list box.

4.  Select source database from **SOURCE** list box.

5.  Enter the name in **TABLE** field.

6.  Select **CranPort** from **PACKAGE TYPE** list.

7.  Update **PRIORITY** field if the default value is not applicable.
    
    **NOTE:** The PRIORITY field determines the order in which tables
    are processed.

8.  Click **Save**.
    
    **NOTE:** Refer to the [Register Tables to
    Source](Register_Tables_to_Source.htm) section to configure package
    fields.

9.  Select table record.

10. Click **Build And Refresh** on Page toolbar to build CranPort
    package and download table from source; a confirmation message
    displays.

11. Click **Ok**.
    
    **NOTE:** If the CranPort package for the table already exists, it
    is only refreshed (i.e., data is downloaded from the source
    database). If the CranPort package for the table does not exist, the
    package is built and the table is refreshed. To view details about
    the CranPort package, select Assemble \> Packages from the
    <span style="background: #ffffff;font-style: italic;">Navigation</span>
    pane.
    
    **NOTE:** The component is referred to as Assemble in the help. The
    package type is still
CranPort.

## <span id="Set_up_Download_with_ManualCranPort_Package"></span>Set up Download with ManualCranPort Package

To set up a table download with a ManualCranPort package:

1.  [Create CranPort package](../../Assemble/Create_Packages.htm).

2.  Click **Tables** in *Navigation* pane to view all tables registered
    to all sources.

3.  Click **Add**.
    
    [View the field descriptions for the Tables
    page](../Page_Desc/Tables_H.htm)

4.  Select target database from **TARGET** list box.

5.  Select source database from **SOURCE** list box.

6.  Enter the table name used in the CranPort package in **TABLE**
    field.

7.  Select **ManualCranPort** from **PACKAGE TYPE** list box if a
    package has already been created in CranPort.

8.  Update **PRIORITY** field if the default value is not applicable.
    
    **NOTE:** The PRIORITY field determines the order in which tables
    are processed.

9.  Click **Save**.

10. Click **Vertical View** for table

11. Click **Advanced Settings** tab.

12. Click **Edit**.
    
    [View the field descriptions for the Tables
    page](../Page_Desc/Tables_H.htm)

13. Select the CranPort package from **Package Name** list box.
    
    **NOTE:** If the package name does not display in the list box,
    confirm that the package has been named following naming
    conventions. Refer to [Create
    Packages](../../Assemble/Create_Packages.htm) for more information.
    
    **NOTE:** Refer to [Register Tables to
    Source](Register_Tables_to_Source.htm) to configure package fields.

14. Click **Action** tab.

15. Click **Refresh**; a confirmation message displays.

16. Click **Ok**.
