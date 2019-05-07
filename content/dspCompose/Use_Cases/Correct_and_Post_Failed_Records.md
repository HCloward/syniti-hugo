+++
title = 'Correct and Post Failed Records'
solution = 'Data Quality'
+++

# Correct and Post Failed Records

dspCompose™ processes partial posts if one or more records error while
trying to post. The records without errors post successfully while the
failed records display on the Data Entry role page to be corrected. A
workflow email is generated notifying the data entry role that records
need processing.

For example if 100,000 records are posted and 10 fail, the successfully
posted records are filtered out thereby allowing the user to work with
and fix only the failed records.

<span style="font-weight: bold;">NOTE</span>: If the request was
initiated by an external request scenario that created an
Excel-initiated request and that request fails to post, the request will
be reset. dspCompose sends an email to the email address that originated
the request. The email has an Excel file attached that contains the data
entry records and information about why the request failed. The user
must correct the errors in the Excel file and send the corrected file to
the External Email Account to begin the process again.

There are three ways to edit or fix data whether making a change or
fixing errors.

Click **DATA ENTRY** for the Data Entry role on the *Request (Roles)*
page and edit the records on the data entry page. This is recommended
when only a few changes need to be made. Refer to [Manually Change
Data](Enter_Data_for_a_Request.htm#Manually_Change_Data)  for more
information.

Download the request data to a spreadsheet and make changes in Excel.
This is recommended when there are a lot of changes or calculations need
to be made. Refer to [Import a File at the Request-Role
Level](Import_a_File_at_the_Request%20Role_Level.htm)  for more
information.

Use the *MassChange* page in dspCompose™ to execute a mass change on the
remaining records on the *DataEntry* page. Refer to [Mass Change
Data](Enter_Data_for_a_Request.htm#Mass_Change_Data)  for more
information.

To correct and post the failed records:

1.  Select **Requests** on the *Navigation pane*.
    
    **NOTE: **The **STATUS** column displays **Posted with Errors** if a
    request contains failed records.

2.  Click **Roles** for a request with failed records.
    
    **NOTE:** The count on the **Roles** icon is the number of roles the
    current user can access, not the total number of roles for the
    request.

3.  Click **DATA ENTRY** for the Data Entry role.
    
    **NOTE: **The Post Message indicates why the record failed.

4.  Click **Edit** for the failed record.

5.  Correct the error.

6.  Click **Save**.

7.  Click the browser’s Back button.

8.  Click **Finish** for the **data entry ROLE ID**.

**NOTE:** A Workflow email is sent to the next role and the request is
processed like any other.

Refer to [Correct Rejected Records](Correct_Rejected_Records.htm) for
additional information.
