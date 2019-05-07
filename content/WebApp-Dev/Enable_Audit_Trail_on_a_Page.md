+++
title = 'Enable Audit Trail on a Page'
solution = 'Platform'
+++

# Enable Audit Trail on a Page

There are two options to select when adding a new table:

  - **Enable Auditing** – If checked, any additions or changes made to
    data in the table are maintained in the audit tables.
  - **Audit Procedures** – If checked, a record of every stored
    procedure that runs against a record as part of a DSP Page Event is
    maintained in the audit tables.

Refer to [Enable Audit Trail & Electronic
Signature](Enable_Audit_Trail_Electronic_Signature.htm) for general
information.

To enable Audit Trail on a page:

1.  Click **Admin**<span style="font-weight: bold;">\> Data
    Sources</span> on the *Navigation* pane.

2.  Click **Audit** for the WebApp’s data source.

3.  Click **Edit**.

4.  Select the data source from **Audit Data Source ID** list box.
    
    **NOTE:** The **Audit Data Source ID** is the database where the
    three audit tables are stored once the tables are built. This can be
    the same as the data source being audited; however, using a
    secondary database and data source can provide benefits in data
    management.

5.  Click **Save**.
    
    **NOTE:** The tables to be audited must be added.

6.  Click **Tables**.

7.  Select the table from **Table Name** list box.

8.  Verify **Enable Auditing** check box is enabled.

9.  Click **Save**.
    
    **NOTE:** These buttons become enabled on the *Horizontal* View.
    
      - **Build Audit Tables button** – Creates the audit tables in the
        specified Data Source. Once the tables are built, the **Snapshot
        Data** button is enabled.
      - **Snapshot Data** **button** – Creates a copy of the tables when
        the snapshot is taken. When a record is edited, the audit trail
        records both the before and the after values. However, the trail
        only shows values that are edited. Snapshot Data can be viewed
        as an insert for existing records. If the audit is enabled after
        the table has values in it, the trail has no way of telling
        where the data came from, so the snapshot is a way of verifying
        that some data existed prior to auditing.
      - **Check Columns** **button** – Reports any differences between
        the columns in the table and the audit
        table<span style="color: #0000ff;">.</span> When the audit
        tables are built, all the columns from the table that are being
        audited are included. However, it is possible to have a case
        where the columns in the table and the audit tables do not
        match. There can be two reasons for the misalignment: 1) the
        Designer deliberately removed some columns from the audit table
        because those values should not be audited or 2) the Designer
        added columns to the table after the audit tables were build and
        forgot to manually update the audit tables.

10. Click **Build Audit Tables** button, a validation message displays.

11. Click the **OK** button.

12. Click **Snapshot** button to take a snapshot of the data in the
    table if necessary.

13. A validation message displays, click the **OK** button.
