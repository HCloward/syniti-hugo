+++
title = 'Complete the Spreadsheet as an External Data Role'
solution = 'Data Quality'
+++

# Complete the Spreadsheet as an External Data Role

Once the request is active, dspCompose™ sends an email from the External
Data Email Account to the external contact for the External Data role.
The spreadsheet contains current request data.

Refer to [Set up an External Data Email
Account](../Config/Set_up_an_External_Data_Email_Account) for more
information.

To complete the spreadsheet as an External Data role:

1.  Download the email attachment.
    
    **NOTE:** Do not change the spreadsheet’s file name when saving it.

2.  Open the file.
    
    **NOTE:** The spreadsheet will reflect the formatting configured for
    the template role. Refer to [Configure Columns for File Generation
    and Data Entry](Configure_Columns_for_File_Generation) for more
    information.
    
    **NOTE:** The first three lines of the spreadsheet that appear with
    a red or black background cannot be updated. The first two rows
    contain column names and other information. The third row contains
    sample request data to use as an example when completing the
    spreadsheet. Do not change or delete these rows of data.

3.  Update data as needed.

4.  Save the spreadsheet.

5.  Reply to the email from the External Data Email Account that sent
    the spreadsheet, attaching the updated file.

**NOTE:** Do not include any text in the body of the email.

**NOTE:** The reply email address is the one configured on the External
Data Email Account page in the USERNAME field, and on the Workflow
Message page, in the EMAIL FROM field, for the ExternalData Event. Both
of these pages are accessed by clicking Configuration on the Navigation
pane.

dspCompose™ will run validations on the spreadsheet. If custom
validations have been added to the template role and the data fails
those validations, dspCompose™ sends the spreadsheet back to the
External Data role for correction.

Refer to Set up Email Validations[Set up Email
Validations](Set_up_Email_Validations) and [Add Custom Email
Validation
Rules](Set_up_Email_Validations#Add_Custom_Email_Validations) for
more information.

dspCompose™ polls the External Data Email Account, collects emails, and
gets the attached Excel file. It then validates the request data and
either replies to the external contact with validation errors or imports
the data into the request and finishes the External Data role.
