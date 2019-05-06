# Grant Users Access to Reports and Sensitive Data

An Administrator <span id="User Report Access" class="popUpLink">must
grant a user access</span> to the Report Delivery pages.

Additionally, some reports may contain sensitive data. Access to view
the data in a sensitive report must be granted by an Administrator.

If the user does not have access to the sensitive data, the record
counts for the report still display.

Report Delivery pages are secured via report business user assignment at
the report levels (Target, Target Data Services, and Source) in
Transform. Role-based security is not applied to the report delivery
pages because a business user who does not have role-based access to,
for example, a Wave Process Area Object Target may still need to view a
report written against that target.

This section includes:

  - 
  - [Assign a User to a
    Report](#Assign_a_User_to_a_Report_on_Report_Delivery_Pages)

  - [Grant a User Access to Sensitive
    Data](#Grant_a_User_Access_to_Sensitive_Data_on_Report_Delivery_Pages)

## <span id="Assign_a_User_to_a_Report_on_Report_Delivery_Pages"></span>Assign a User to a Report on Report Delivery Pages

A user must be assigned to a report to view it on Report Delivery pages
and to receive a workflow notification for report readiness.

An Administrator must
<span id="User Report Access" class="popUpLink">grant a user
access</span> to the Report Delivery pages.

**NOTE:** When a report is registered, users assigned to the object
under which it is registered and users assigned to the Target under
which it is registered are automatically synced over and assigned to the
newly registered report and report segments. If a Business user is
removed from the target level, that user can no longer view the target’s
reports.

To assign a user to a report on Report Delivery pages in Transform:

1.  Click the **Targets** icon in the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the **Reports** icon for a **TARGET** and **OBJECT** grouping.

3.  Click **Vertical View** for a **TARGET REPORT** where the
    **PUBLISH** check box is checked.

4.  Click the **Business User Settings** tab.

5.  Click the **Business User Assignment** icon.
    
    **NOTE:** All users display on the [All Reports All
    Users](../Page_Desc/All_Reports_All_Users.htm) page except for
    Anonymous, process, search, and translator users.

6.  Select a user by highlighting the name.

7.  Click **Add User**; a check mark displays in the **IS MEMBER**
    column for the selected user.

**NOTE:** To assign multiple users to the report, press the **CTRL** key
while selecting users. Once all users are selected, click **Add User**.

Once the user is assigned to the report, the report displays on the
*[All Reports](../Page_Desc/All_Reports.htm)* page. Refer to [View All
Reports](View_Reports.htm#View_All_Reports) for more information.

When a report is registered, users assigned to the object under which it
is registered and users assigned to the target under which it is
registered are automatically synced over and assigned to the newly
registered
report.

## <span id="Grant_a_User_Access_to_Sensitive_Data_on_Report_Delivery_Pages"></span>Grant a User Access to Sensitive Data on Report Delivery Pages

To grant a user additional access to sensitive data in a target, source,
or target Data Services report in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.
2.  Click the **Reports** icon for a target.

OR

1.  Click the**Targets** icon on the *Process Area Launch* page.
2.  Click the **Sources** icon for a target.
3.  Click the **Reports** icon for a source.

OR

1.  Click the **Targets** icon on the *Process Area Launch* page.
2.  Click the **Data Services Reports** icon for a target.

After accessing the report:

1.  Click **Vertical View** for the report.

2.  Click the **Business User Settings** tab.

3.  Click the **Sensitive** check box to check it.
    
    **NOTE:** The Sensitive check box and the Business User Segment
    Assignment icon only display when the Publish check box is checked.

4.  Click the **Business User Assignment** icon.

5.  Select the **USER NAME** to add or grant access to the report.

6.  Click the **Add User** icon (or the + sign) in the Page toolbar to
    give the user access to the report.

7.  Click the **Grant Access to Sensitive Data** (the open lock icon) to
    grant the user access to sensitive data.
    
    **NOTE:** The IS MEMBER and ALL ACCESS columns should be checked for
    the USER NAME.
    
    **NOTE:** A user must have access (IS MEMBER) to the report to be
    granted access to sensitive data. In other words, the ALL ACCESS
    column cannot be checked unless the IS MEMBER column has been
    checked.
    
    **NOTE:** If only the IS MEMBER column is checked, the user does not
    have access to sensitive data in the report.
