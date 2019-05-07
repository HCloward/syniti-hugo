+++
title = 'Create Custom Pages and Views'
solution = 'Data Quality'
+++

# Create Custom Pages and Views

Before performing this task:

1.  Create a looped template and process in Integrate. Refer to
    [Configure Process Template Loops for a BDC Script Template with
    Looping
    Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTempLoopsBDCLoopEn.htm)
    or [Configure Process Template Loops for a GUI Script Template with
    Looping
    Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTemplLoopsGUILoopgEn.htm)
    in Integrate for more information.
2.  [Create all tt Tables and tx Views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process.htm)
3.  [Create rt Tables from the tt
    Tables](Create_rt_Tables_from_the_tt_Tables.htm)

Once all of the necessary tables and **tx** views are created, create
the custom pages and views in dspCompose™ outlined in the following
sections. Create the views in the same database where the **tt** tables
and **tx** views were created.

  - [Create Data Entry Pages and
    Views](#Create_Data_Entry_Pages_and_Views)
  - [Create Approval Pages and Views](#Create_Approval_Pages_and_Views)
  - [Create Archive Pages](#Create_Archive_Pages)

After creating custom pages and views, continue with [Create a Template
that Uses the Custom Pages in
dspCompose™](Create_a_Template_that_uses_the_Custom_Pages.htm).

## <span id="Create_Data_Entry_Pages_and_Views"></span>Create Data Entry Pages and Views

Create Data Entry pages for each of the **tt** tables and name these
pages 'xxx' where 'xxx' describes the page activity.

**NOTE:** Most column properties do not need to be specified on these
pages.

Add column properties to the page to hide the following columns: ID,
LockReject, PostError, RejectedBy, RejectReason, PostMessage, Reject,
RequestID, and ViewName.

Disable Severity and ValidationErrorMessage.

Create Horizontal views for each Data Entry page named web'xxx'Hor
<span>where xxx describes the page activity</span>. Register each view
to the corresponding Data Entry page.

**NOTE:** Page Table should have an ID column that is set as the
PrimaryKey.

## <span id="Create_Approval_Pages_and_Views"></span>Create Approval Pages and Views

Create an Approval page for each Data Entry page. These pages will use
the **tt** table used by the corresponding Data Entry page. Name these
pages 'xxx - Review' where xxx describes the page activity.

Add column properties to the page to hide the following columns: ID,
LockReject, PostError, RejectedBy, PostMessage, RequestID and ViewName.

Disable Severity and ValidationErrorMessage. Enable Reject and
RejectReason.

Create Horizontal views for the Approval pages and name the views
web'xxx'ApproveHor <span>where xxx describes the page activity</span>.
Register each view to the corresponding Approval page.

**NOTE:** Page Table should have an ID column that is set as the
PrimaryKey.

## <span id="Create_Archive_Pages"></span>Create Archive Pages

Create Archive pages for each **rt** table and name these pages 'xxx -
Archives' where xxx describes the page activity.

Add column properties to the page to hide ArchiveID, LockReject, Reject,
RejectedBy, RejectReason, RequestID, and Severity.

Disable Connection and PostedOn.

Create Horizontal views for each of the Archive pages and name these
views web'xxx'ArchiveHor <span>where xxx describes the page
activity</span>. Register each view to the corresponding Archive page.

**NOTE:** Page Table should have ArchiveID column that is set as the
PrimaryKey.
