# Support Regulatory Compliance

The DSP assists clients with regulatory and corporate compliance by:

  - Restricting access to personal data (any data that can be used to
    identify a person), handled through DSP security and through purging
    data after a retention date has passed. Purging data is configured
    in Common and Collect.
  - Tracking and logging user access to this data throughout the
    product, which is configured in System Administration.

Settings must be configured before compliance can begin.

  - An Administrator must enable the logging feature in System
    Administration. By default, the DSP tracks access to all pages;
    however, an Administrator can control which pages are tracked. Refer
    to [Log Access to Personal Data
    i](../../Sys_Admin/Use_Cases/Log%20Events%20and%20Access%20to%20Personal%20Data.htm)n
    System Administration for more information.
  - At the client site, an Administrator must also set up auditing for
    these specific tables in the DataSource named “DataGarage”.
      - dgTarget
      - dgTargetSource
      - dgTargetSourceTable

When a Data Controller updates any retention expiration date, an
e-signature is required and captured in the audit records.

  - At the client site, an Administrator should also set up auditing for
    any tables that contain regulated data. Refer to [Enable Auditing
    for Tables with Personal
    Information](../../Sys_Admin/Use_Cases/Enable%20Auditing%20for%20Tables%20with%20Personal%20Information.htm)
    in System Administration for more information.
  - A Collect Administrator must [configure data
    protection](#Configure_Data_Protection) for Targets, Sources and
    Tables.

Additionally a Common Administrator can:

  - [Add custom data classifications and information
    types](../../Common/Use_Cases/Add%20Custom%20Data%20Classifications%20and%20Information%20Types.htm)
    as needed
  - [Update Retention Expiration Warning
    Period](../../Common/Use_Cases/Update%20Retention%20Expiration%20Warning%20Period.htm)
  - [Update the Retention Expiration
    Email](../../Common/Use_Cases/Update%20the%20Retention%20Expiration%20Email.htm)

Any user who has access to the target can:

  - [Update the Retention Expiration
    Date](#Update_the_Retention_Expiration_Date)
  - [Purge Data](#Purge_Data)

**NOTE:** Once the data is purged from a table, the table is
deactivated. It cannot be refreshed either manually or automatically.

## <span id="Configure_Data_Protection"></span>Configure Data Protection

A Collect Administrator configures data protection settings at the
target, target source, and table level.

The settings configured at the target level are set by default for any
target sources and tables added to the target. The settings can then be
updated at the target source and table level.

The most specific data protection settings are used, and the earliest
Retention Expiration Date takes precedence. For example, if the
retention date for a table is the first of the month and the retention
date for the target is the fifteenth, data from the table is purged on
the first. Data in the rest of the target is purged two weeks later. In
the reverse case, where the target expires on the first of the month and
the table is set to expire on the fifteenth, the specific table will
still be purged with the rest of the tables in the target on the first.

To configure data protection for a target, target source, or table in
Collect:

1.  Select **Targets** in the *Navigation* pane.
    
    OR
    
    Select **Targets** in the *Navigation* pane, then click the
    **Sources** icon.
    
    OR
    
    Select **Targets** in the *Navigation* pane, click the **Sources**
    icon, then click the **Tables** icon.

2.  Click **Vertical View** for a target, target source, or table.

3.  Click the **Data Protection** tab.

4.  Click **Edit**.
    
    View the field descriptions for the Data Protection tab for
    [Targets](../Page_Desc/Targets_H_Collect.htm#Data), [Target
    Sources,](../Page_Desc/Target_Sources_H_Collect.htm#Data_Protection)
    or [Tables](../Page_Desc/Tables_H.htm#Data)

5.  Select the user or group responsible for processing personal data
    for the object from the **Data Controller** list box.
    
    **NOTE:** Only those users or groups that have access to the target
    through a security role and security key display.
    
    **NOTE:** The Collect Administrator must check the WORK FLOW SUMMARY
    check box for the target and Data Controller on the *[Workflow
    Summary User
    Settings](../Page_Desc/Workflow_Summary_User_Settings.htm)* page.
    The Data Controller is added to this page automatically. If the
    check box is not checked, the Data Controller will not receive a
    warning email that data is going to be purged.

6.  Select an option in the **Data Classification** list box.
    
    **NOTE:** Options are:
    
    • **Personal** — This object contains data that must be purged by a
    certain date. The Retention Expiration Date field must be completed
    for this object (e.g., Customer Addresses, Employee Records,
    Business Partner Tax IDs).
    
    • **Public** — This object contains data that does not need to be
    purged (e.g., Units of Measure, Material Descriptions, Country
    Codes).
    
    • **Restricted** — This data does not need to be purged, but is
    marked as restricted access (e.g., Company Chart of Accounts,
    Recipes, Work Orders).
    
    • Custom data classifications also display in this list box.

7.  Select the date when the object’s data is deleted from a table(s) in
    the **Retention Expiration Date** field.
    
    **NOTE:** Updates to this field are audited (if auditing has been
    enabled for the table(s) in System Administration). An e-signature
    is required.

8.  Enter your **user ID** and **password**.

9.  Enter the reason for update in the **Comment** field.

10. Click **Sign Record**.

11. Enter the reason for extracting the data.
    
    **NOTE:** Any time the table is processed, the data should only be
    used for the reason identified in this field.

12. Click **Save**.

## <span id="Purge_Data"></span>Purge Data

Data in a target, target source, or table with the data classification
Personal (or with a custom classification where the Retention Period
Warning feature is enabled) is purged on the retention expiration date.

The most specific data protection settings are used, and the earliest
Retention Expiration Date takes precedence. For example, if the
retention date for a table is the first of the month and the retention
date for the target is the fifteenth, data from the table is purged on
the first. Data in the rest of the target is purged two weeks later. In
the reverse case, where the target expires on the first of the month and
the table is set to expire on the fifteenth, the specific table will
still be purged with the rest of the tables in the target on the first.

When data is purged at the target level, all data in all tables
(including check tables) at the target and target source levels is
deleted. When data is purged at the target source level, data in all
tables (including check tables) in that target source are deleted. Data
purged at the table level deletes date for that table only.

The purge is preformed automatically on the retention expiration date by
a Service page that runs once daily.

The purge can also be performed manually.

**NOTE:** Once the data is purged from a table, the table is
deactivated. It cannot be refreshed either manually or automatically.
The Refresh and Build and Refresh icons on the Targets, Target Sources,
and Tables pages are inactive.

To purge data at the target level and delete all tables in the target
and target sources in Collect:

1.  Select **Targets** in the *Navigation* pane.
2.  Click **Vertical View** for a target.
3.  Click the **Data Protection** tab.
4.  Click the **Purge Data** icon.

To purge data at the target source level and delete all tables in the
target source in Collect:

1.  Select **Targets** in the *Navigation* pane.
2.  Click the **Source** icon.
3.  Click **Vertical View** for a target source.
4.  Click the **Data Protection** tab.
5.  Click the **Purge Data** icon.

To purge data at the table level, use the Truncate Table feature in
Collect:

1.  Select **Targets** in the *Navigation* pane.
2.  Click the **Source** icon.
3.  Click the **Tables** icon.
4.  Click **Vertical View** for a table.
5.  Click the **Action** tab.
6.  Click the **Truncate Table**
icon.

## <span id="Update_the_Retention_Expiration_Date"></span>Update the Retention Expiration Date

Any user with security access to the target can update the date by which
data is purged from a target, target source or table. However, an
e-signature is required.

To update the retention expiration date in Collect:

1.  Select **Targets** in the *Navigation* pane.
    
    OR
    
    Select **Targets** in the *Navigation* pane, then click the
    **Sources** icon.
    
    OR
    
    Select **Targets** in the *Navigation* pane, click the **Sources**
    icon, then click the **Tables** icon.

2.  Click **Vertical View** for a target, target source, or table.

3.  Click the **Data Protection** tab.

4.  Click **Edit**.
    
    View the field descriptions for the Data Protection tab for
    [Targets](../Page_Desc/Targets_H_Collect.htm#Data), [Target
    Sources](../Page_Desc/Target_Sources_H_Collect.htm#Data_Protection)
    or [Tables](../Page_Desc/Tables_H.htm#Data)

5.  Select the date when the object’s data is deleted from a table(s) in
    the **Retention Expiration Date** field.
    
    **NOTE:** Updates to this field are audited. An e-signature is
    required.

6.  Enter your **user ID** and **password**.

7.  Enter the reason for update in the **Comment** field.

8.  Click **Sign Record**.

9.  Click **Save**.
