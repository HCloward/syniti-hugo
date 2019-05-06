# Review Request Changes

To assist in the review process, a Designer can configure a list of
Content WebApp tables and columns that can be audited. The changes
tracked in these audits display for a request for the Review role. The
Review role can then view all the changes that have occurred within the
Application role(s) that the Review role is dependent on.

Before a Role Processor with the Review role can view all changes for a
request, an Administrator must configure settings in System
Administration and a Designer must configure settings in dspConduct™.

For data to display for the Review role on the
<span style="font-style: italic;">Review Role Audit Details</span> page,
auditing must be enabled in System Administration and the tables and
columns to be audited must be configured at the category level in
dspConduct™.

This section contains the following topics:

  - [Enable Auditing for the Content WebApp tables in System
    Administration](#Enable_Auditing_for_the_Content_WebApp_Tables)
  - [Configure the tables and columns to be audited at the category
    level in dspConduct™](#Register_Tables_and_Columns_to_be_Audited)
  - [View Request Changes as a Review
    Role](#View_Request_Changes_as_the_Review_Role)

## <span id="Enable_Auditing_for_the_Content_WebApp_Tables"></span>Enable Auditing for the Content WebApp Tables

For the Review role to view the changes for a request, an Administrator
must enable auditing for a table for the Content WebApp data source. The
table contains the data that is used in the request and any updates to
this data display for the Review role on the
<span style="font-style: italic;">[Review Role Audit
Details](../Page_Desc/Review_Role_Audit_Details_H.htm)</span> page.

To enable auditing for a table in the Content WebApp’s data source:

1.  Click **Admin** \> **Data Sources** in the *Navigation* pane.

2.  Click the **Audit** icon for the Content WebApp’s data source.

3.  Click **Edit**.

4.  Select the data source from **Audit Data Source ID** list box.

5.  Click <span style="font-weight: bold;">Save</span>.
    
    **NOTE**: The tables to be audited must be added.

6.  Click the **Tables** icon.

7.  Select the table from **Table Name** list box.

8.  Verify **Enable Auditing** check box is enabled.

9.  Click <span style="font-weight: bold;">Save</span>.
    
    These buttons become enabled on the *Horizontal* View.
    
      - **Build Audit Tables** – Creates the audit tables in the
        specified data source. Once the tables are built, the **Snapshot
        Data** button is enabled.
      - **Snapshot Data** – Creates a copy of the tables when the
        snapshot is taken. When a record is edited, the audit trail
        records both the before and the after values. However, the trail
        only shows values that are edited. Snapshot Data can be viewed
        as an insert for existing records. If the audit is enabled after
        the table has values in it, the trail has no way of telling
        where the data came from, so the snapshot is a way of verifying
        that some data existed prior to auditing.
      - **Check Columns** – Reports any differences between the columns
        in the table and the audit table. When the audit tables are
        built, all the columns from the table that are being audited are
        included. However, it is possible to have a case where the
        columns in the table and the audit tables do not match. There
        can be two reasons for the misalignment: 1) the Designer removed
        some columns from the audit table because those values should
        not be audited or 2) the Designer added columns to the table
        after the audit tables were built and did not manually update
        the audit tables.

10. Click **Build Audit Tables** button, a validation message displays.

11. Click **OK**.

12. Click **Snapshot** button, a validation message displays.

13. Click **OK**.

Once auditing is enabled, the table(s) displays on the
<span style="font-style: italic;">[Audit Table
Registration](../Page_Desc/Audit_Table_Registration.htm)</span> page in
dspConduct, where individual tables and columns can be enabled or
disabled for auditing.

Continue with Register Tables and Columns to be Audited in
dspConduct

## <span id="Register_Tables_and_Columns_to_be_Audited"></span>Register Tables and Columns to be Audited

A Designer configures which Content WebApp tables and columns are
audited in dspConduct. Changes to requests based on the data in these
tables and columns is then tracked and displayed for a user with the
Review role.

<span style="font-weight: bold;">NOTE:</span> Data that was updated
before auditing was enabled is not included in the audited changes.

To register tables and columns to be audited:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Vertical View</span> for a
    category.

3.  Click the <span style="font-weight: bold;">Rules and Actions</span>
    tab.

4.  Click the <span style="font-weight: bold;">Table Registration</span>
    icon.
    
    **NOTE:** The <span style="font-style: italic;">[Audit Table
    Registration](../Page_Desc/Audit_Table_Registration.htm)</span> page
    displays any tables that have had auditing enabled for the Default
    WebApp ID (the Content WebApp) in System Administration.

5.  Click the <span style="font-weight: bold;">ENABLED</span> check box
    to disable it if a table should not be audited.
    
    **NOTE:** By default, all tables are audited.
    
    **NOTE:** If tables are not audited, updates to this table’s data
    for a request do not display for the Review role on the Review Role
    Audit Details page.

6.  Click the <span style="font-weight: bold;">Columns</span> icon for a
    table.
    
    **NOTE:** All columns in the table selected on the [Audit Table
    Registration](../Page_Desc/Audit_Table_Registration.htm) page
    display. These columns are enabled for auditing by default.

7.  Click the <span style="font-weight: bold;">ENABLED</span> check box
    to uncheck it if changes to a column’s data must not be audited.  

8.  Click the **PRIMARY KEY** check box.
    
    **NOTE:** This check box must be checked for the Key to Record field
    to display on the *[Review Role Audit
    Details](../Page_Desc/Review_Role_Audit_Details_H.htm)* page.

9.  Click the <span style="font-weight: bold;">INCLUDE IN RECORD
    KEY</span> check box to display the column name in the Key to Record
    field on the <span style="font-style: italic;">[Review Role Audit
    Details](../Page_Desc/Review_Role_Audit_Details_H.htm)</span> page.

Adding additional columns can provide more information to the Review
role when evaluating updates in a request.

Key fields are not affected by this setting, with the exception of the
RequestID. Key fields display in the Key to Record field, even if this
check box is unchecked. However, the display of the RequestID column can
be controlled using this option. For example, the user disables this
option for the key fields DATE\_FROM and RequestID. In the Key to Record
field, the DATE\_FROM field still displays. The RequestID field does
not.

Audit data for tables or columns that were updated is loaded into
staging tables, and can then be viewed by the Review role for requests
based on the data in the table(s) or column(s).

Audit data is automatically loaded to the staging tables when table or
column registrations are updated. If the audit data must be loaded
immediately, click the Load Audit Data icon.

After this task is complete a user with the Review role can view changes
for a
request.

## <span id="View_Request_Changes_as_the_Review_Role"></span>View Request Changes as the Review Role

When the Application role with the highest priority is finished and the
Review role becomes available for the request, the Review role can view
all of the request’s changes for all Application role(s) the Review role
is dependent on.

<span style="font-weight: bold;">NOTE:</span> If auditing is enabled for
the category’s Default WebApp ID, a workflow message is sent to the
Review role when the Application role is finished and the Review role
becomes available. The message lists the changed data records for the
request. The Review role receives these workflow messages based on
workflow receipt preferences. Refer to [Set User Workflow Receipt
Preferences](../Config/Set_User_Workflow_Receipt_Preferences.htm) for
more information.

To view the changes for a request:

1.  Click <span style="font-weight: bold;">dspConduct \> Requests</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Roles</span> for a request.

3.  Click the <span style="font-weight: bold;">Tasks</span> icon for the
    Review role.

4.  Click the <span style="font-weight: bold;">Review Changes</span>
    icon for a task.
    
    **NOTE:** The Review role must be active (i.e., the Application role
    with the highest priority must be finished) for the Review Changes
    icon to be active.
