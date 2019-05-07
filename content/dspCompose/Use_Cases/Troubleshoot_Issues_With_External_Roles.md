+++
title = 'Troubleshoot Issues with External Roles'
solution = 'Data Quality'
+++

# Troubleshoot Issues with External Roles

dspCompose™ generates a spreadsheet with request data and sends it to a
user designated as an external contact for an External Data role. The
user updates the spreadsheet and mails it to an external data email
account configured in dspCompose™.

To troubleshoot issues with sending data to and receiving data from an
External Data role, use the *[Roles
(Execute)](../Page_Desc/Roles_Execute.htm)* page.

To troubleshoot issues with sending spreadsheets to External Data roles:

1.  Select **Configuration \> Roles (Execute)** on the *Navigation*
    pane.
    
    **NOTE:** Only **ROLE IDs** from External Data role types display.
    
    **NOTE:** The value in the **REQUEST ID** field on the *Request*
    page identifies the request.

2.  Click the **Process External Role** icon for a request.

**NOTE:** dspCompose™ generates a spreadsheet and sends it to the user
designated as the external contact for the External Data role. The user
receives an email and a notification that the spreadsheet is available.
When the process is complete, the **STATUS** updates to **EmailSent**.

To troubleshoot issues with processing spreadsheets sent from External
Data roles:

1.  Select **Configuration \> Roles (Execute)** on the *Navigation*
    pane.
    
    **NOTE:** Only **ROLE IDs** from External Data role types display.
    
    **NOTE:** The value in the **REQUEST ID** field on the
    *[Request](../Page_Desc/Request_H.htm)* page identifies the request.

2.  Click the **Process Inbound File** icon for a request.

**NOTE:** If the External Data role has sent a spreadsheet to the
external data email account, dspCompose™ will process the spreadsheet
and finish the role, then notify the next role in the workflow.

Refer to [Use External Data Roles in Request
Processing](Use_External_Data_Roles_in_Request_Processing.htm) for more
information.
