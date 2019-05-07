+++
title = 'Create Custom Pages and Views for the BAPI Process'
solution = 'Data Quality'
+++

# Create Custom Pages and Views for the BAPI Process

Before performing these steps:

1.  [Post Data Using A
    BAPI](../../../Platform/Integrate/Use_Cases/Post_Data_Using_a_BAPI.htm)
2.  [Create all tt Tables and Views for the BAPI
    Process](Create_tt_Tables_and_Views_for_the_BAP_Process.htm)
3.  [Create rt Tables From the tt Tables and Create Views for the BAPI
    Process](CreatertTblsttTableCreateVwsBAPI.htm)

Once all the necessary tables and **tx** views are prepared, create the
following custom pages and views:

  - [Create Data Entry Page and View for the BAPI
    Process](#Create_Data_Entry_Page_and_View_for_the_BAPI_Process)

  - [Create Approval Page and View for the BAPI
    Process](#Create_Approval_Page_and_View_for_the_BAPI_Process)

  - [Create Archive Page for the BAPI
    Process](#Create_Archive_Page_for_the_BAPI_Process)

<span style="font-weight: bold;">NOTE</span>: If the custom page should
allow a user to perform a mass change, refer to [Add a Mass Change
Custom Link to a Custom
Page](Add_a_Mass_Change_Custom_Link_to_a_Custom_Page.htm) for more
information.

After creating custom pages, continue with [Use the Custom Pages in
dspCompose™ for the BAPI
Process](Use_the_Custom_Pages_in_dspCompose_for_the_BAPI_Process.htm).

## <span id="Create_Data_Entry_Page_and_View_for_the_BAPI_Process"></span>Create Data Entry Page and View for the BAPI Process

Create a Data Entry page that will use the main **tt** table and name
this page 'xxx' where 'xxx' describes the page activity.

**NOTE**: Most column properties do not need to be specified on this
page.

Add column properties to the page to hide ID, LockReject, PostError,
RejectedBy, RejectReason, RequestID, and ViewName.

Disable Severity and ValidationErrorMessage.

Create a Horizontal view for the Data Entry page named web'xxx'Hor
<span>where xxx describes the page activity</span>.

<span style="font-weight: bold;">NOTE</span>: Page Table should have an
ID column that is set as the
PrimaryKey.

## <span id="Create_Approval_Page_and_View_for_the_BAPI_Process"></span>Create Approval Page and View for the BAPI Process

Create an Approval page that will also use the main **tt** table. Name
this page 'xxx - Review'
<span style="font-family: Arial, sans-serif;">where xxx describes the
page activity</span>.

Add column properties to the page to hide ID, LockReject, PostError,
RejectedBy, RequestID, and ViewName.

Disable Severity and ValidationErrorMessage. Enable RejectReason.

Create a Horizontal view for the Approval page and name this view
web'xxx'ApproveHor <span style="font-family: Arial, sans-serif;">where
xxx describes the page
activity</span>.

## <span id="Create_Archive_Page_for_the_BAPI_Process"></span>Create Archive Page for the BAPI Process

Create an Archive page that will use the main **rt** table and name this
page 'xxx - Archives'
<span style="font-family: Arial, sans-serif;">where xxx describes the
page activity</span>.

Add column properties to the page to hide ArchiveID, ID, LockReject,
Reject, RejectedBy, RejectReason, RequestID, and Severity.

Disable Connection and PostedOn.

Create a Horizontal view for the Archive page and name this view
web'xxx'ArchiveHor <span>where xxx describes the page activity</span>.

<span style="font-weight: bold;">NOTE</span>: Page Table should have
ArchiveID column that is set as the PrimaryKey.
