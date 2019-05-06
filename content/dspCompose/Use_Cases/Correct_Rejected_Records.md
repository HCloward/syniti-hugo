# Correct Rejected Records

When the Review role rejects all or some of the records for a request,
that request is sent back to the Data Entry role for correction.

**NOTE**: Templates in dspCompose™ are highly customizable and can be
configured to have multiple Role IDs with the Role Type of Data. Users
assigned to these roles add or update request data. A template can have
multiple Data Entry roles. The generic term “Data Entry role” is used
throughout this use case, and can refer to one or multiple Role IDs with
the Role Type of Data.

**NOTE:** The user assigned to the Data Entry role is notified that the
role assigned to the new request must be completed (if the records were
rejected using partial approval) or that the role has been reset (if all
records in the request were rejected). The rejection reason is included
in the Reject email notification and stored on the *Vertical* View of
the Request via the **Rejection Archive** feature.

There are three ways to fix rejected records:

  - Download the records into the dspCompose™ generated Excel
    spreadsheet, edit the records and upload the spreadsheet. Refer to
    [Import a File at the Request-Role
    Level](Import_a_File_at_the_Request%20Role_Level.htm)  for more
    information.

  - Make the change on the *Mass Change* page. Refer to  [Mass Change
    Data](Enter_Data_for_a_Request.htm#Mass_Change_Data) for more
    information.

  - Manually edit the records on the data entry page. Refer to
     [Manually Change
    Data](Enter_Data_for_a_Request.htm#Manually_Change_Data)  for more
    information.

To view the rejected records:

1.  Click the **Workflow** link in the email to be directed to the
    request.
    
    *Or*  
    
    Select **Requests** on the *Navigation* pane.

2.  Click **Roles** for the request containing the rejected records.

3.  Click **DATA ENTRY** for the Data Entry role.

**NOTE**: The rejected records display; if rejection reasons were
entered for individual records, those will display for the appropriate
records.

**NOTE**: Manually edit the records on this page, or, if the rejected
records are for a mass change, click **Mass Change** on the Page toolbar
and correct the data on the *Mass Change* page.

**NOTE**: The Data Entry role for the template must have the **Excel
Import Allowed** check box enabled to allow a user to import a
spreadsheet with updated request data. Navigate to the *Template (Role)*
page’s *Vertical* View for the Data Entry role. On the **Import
Settings** tab, click the check box to enable it.

To download the records into the spreadsheet for correction:

1.  Click the **Workflow** link in the email to be directed to the
    request.
    
    *Or*
    
    Select **Requests** on the *Navigation* pane.

2.  Click **Roles** for the request containing the rejected records.

3.  Click **Vertical View** for the **Data Entry** role.

4.  Click **Download Request Data<span style="font-weight: normal;">; a
    notification displays with a link to download the file.</span>**

5.  Click the <span style="font-weight: bold;">download</span> link to
    download the file.

6.  Locate the file and correct the data.

7.  Save the file.

8.  Return to the *Vertical* View of the *Request (Roles)* page in
    dspCompose™.

9.  Verify **Delete Data Before Import –File** check box is checked.

10. Click **Import**.

11. Locate the Excel file.

12. Click **Open**, a confirmation displays.

13. Click **Ok** to confirm import.

14. Navigate back to the *Request (Roles)* page's
    <span style="font-style: italic;">Horizontal</span><span>View.</span>

15. Click **DATA ENTRY** for the Data Entry role to confirm the data
    imported correctly.

16. Navigate to the *Request (Roles)* page.

17. Click **Finish** for the Data Entry role to send the request data to
    the Review role.
