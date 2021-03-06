+++
title = 'Create Pages and Views in Custom WebApp'
solution = 'Data Quality'
+++

# Create Pages and Views in Custom WebApp

Once all the necessary tables and **tx** views are prepared, create the
following custom pages and views:

  - [Create Data Entry Page and View](#Create_Data_Entry_Page_and_View)
  - [Create Approval Page and View](#Create_Approval_Page_and_View)
  - [Create Archive Page](#Create_Archive_Page)

**NOTE:** If the custom page should allow a user to perform a mass
change, refer to [Add a Mass Change Custom Link to a Custom
Page](Add_a_Mass_Change_Custom_Link_to_a_Custom_Page) for more
information.

## <span id="Create_Data_Entry_Page_and_View"></span>Create Data Entry Page and View

Create a Data Entry page that will use the main **tt** table and name
this page 'xxx' where 'xxx' describes the page activity.

**NOTE:** Most column properties do not need to be specified on this
page.

Add column properties to the page to hide ID, LockReject, PostError,
RejectedBy, RejectReason, RequestID, and ViewName.

Disable Severity and ValidationErrorMessage.

Create a Horizontal view for the Data Entry page named web'xxx'Hor where
xxx describes the page activity.

**NOTE:** Page Table should have an ID column that is set as the
PrimaryKey.

## <span id="Create_Approval_Page_and_View"></span>Create Approval Page and View

Create an Approval page that will also use the main **tt** table. Name
this page 'xxx - Review' where xxx describes the page activity.

Add column properties to the page to hide ID, LockReject, PostError,
RejectedBy, RequestID, and ViewName.

Disable Severity and ValidationErrorMessage. Enable RejectReason.

Create a Horizontal view for the Approval page and name this view
web'xxx'ApproveHor where xxx describes the page activity.

## <span id="Create_Archive_Page"></span>Create Archive Page

Create an Archive page that will use the main **rt** table and name this
page 'xxx - Archives' where xxx describes the page activity.

Add column properties to the page to hide ArchiveID, ID, LockReject,
Reject, RejectedBy, RejectReason, RequestID, and Severity.

Disable Connection and PostedOn.

Create a Horizontal view for the Archive page and name this view
web'xxx'ArchiveHor where xxx describes the page activity.

**NOTE:** Page Table should have ArchiveID column that is set as the
PrimaryKey
