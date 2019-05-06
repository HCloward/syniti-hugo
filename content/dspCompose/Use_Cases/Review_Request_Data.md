# Review Request Data

The primary responsibility of the Review role is to evaluate the work of
the Data Entry role(s) for accuracy and completion.

**NOTE**: Templates in dspCompose™ are highly customizable and can be
configured to have multiple Role IDs with the Role Type of Data. Users
assigned to these roles add or update request data. A template can have
multiple Data Entry roles. The generic term “Data Entry role” is used
throughout this use case, and can refer to one or multiple Role IDs with
the Role Type of Data.

**NOTE:** The data available to specific users for review can be
controlled using Review filters. Refer to [Create Review
Filters](Add_Users_to_Templates.htm#Create_Review_Filters) for more
information.

**NOTE:** Review filters only apply to dspCompose™-generated
Review/Approve pages. If a custom page is assigned to a Review role,
then the Review filters do not apply to that page.

**NOTE:** When the Data Entry role user clicks **Finish** for the role,
the user assigned to the Review role for the request will receive an
email if the **SEND WORKFLOW** check box is enabled for that user on the
*[User](../Page_Desc/User_H.htm)* page. If multiple Data Entry roles
exist for the template, the Review role will receive the notification
when the final Data Entry role in the workflow clicks **Finish**.

**NOTE:** If the request has Org Units assigned, dspCompose™ will only
send workflow emails to users who have Org Unit security for values on
the request.

This topic contains the following sections:

  - [Review the Data](#Review_the_Data)
  - [Reject a Role](#Reject_a_Role)
  - [Perform a Partial Approval](#Perform_a_Partial_Approval)

## <span id="Review_the_Data"></span>Review the Data

To review the request data:

1.  Click the Workflow link in the email to be directed to the request
    
    *Or*
    
    Select **Requests** on the *Navigation* pane.

2.  Click **Roles** for a request.
    
    **NOTE:** The count on the **Roles** icon is the number of roles the
    current user can access, not the total number of roles for the
    request.

3.  Click **DATA ENTRY** for the **ReviewROLE ID**.

4.  Review the data for accuracy.
    
    **NOTE:** If the parameter **Allow Partial Approval** is enabled on
    the **Template** tab of the
    *[Parameters](../Page_Desc/Parameters.htm)* page, the Review role
    can approve or reject each record separately. Refer to [Perform a
    Partial Approval](#Perform_a_Partial_Approval) for further
    information.
    
    **NOTE**: If the **Use Comparison Approval Page** check box is
    enabled for the Template, the review page displays both the current
    target system’s values and the values changed. Refer to [Use
    Comparison Approvals](Use_Comparison_Approvals.htm) for more
    information.

5.  Click Back button on the browser to return to the
    <span style="font-style: italic;">[<span style="font-style: italic;">Request
    (Role)</span>](../Page_Desc/Request_Roles_H.htm)</span>page.

6.  Click **Approve** to confirm the data is correct. This process
    initiates the workflow email to users assigned to the Post role.
    
    *Or*
    
    Click **Reject** if there are errors in the data. This process
    resets the role.

## <span id="Reject_a_Role"></span>Reject a Role

If a mistake is made or if information is incomplete after the Data role
has been finished, the Review role may reject some or all of the records
in a request. Rejecting a role resets all dependency and workflow emails
for all users assigned to the roles and dependent roles. Any completed
information remains and can be edited.

**NOTE**: To target a role for request rejection from a Review role,
refer to [Set Target Role for Request Rejections from a Review
Role](Set_Target_Role_for_Request_Rejections.htm) for more information.

**NOTE**: When the Review role user clicks **Reject** for any records on
the request, the user assigned to the initial Data Entry role for the
request will receive an email if the **SEND WORKFLOW** check box is
enabled for that user on the *[User](../Page_Desc/User_H.htm)* page.

<span style="font-weight: bold;">NOTE</span>: If another role is
specified on the *[*Template
(Role)*](../Page_Desc/Template_Role_H.htm)*page *Vertical* View,
**Approve and Finish Settings** tab, in the **Reject Role Target** list
box, that role receives the email instead of the initial Data Entry
role. <span>The Reject Role Target list box only displays when a user
clicks Vertical View on
the</span><span style="font-style: italic;">Template
(Role)</span><span>page for the Review Role.</span> Refer to [Set Target
Role for Request
Rejections](Set_Target_Role_for_Request_Rejections.htm) for more
information.

**NOTE**: If the request has Org Units assigned, dspCompose™ only sends
workflow emails to users who have Org Unit security for values on the
request.

<span style="font-weight: bold;">NOTE</span>: If the request was
initiated by an external request scenario that created an
Excel-initiated request and the request is rejected by the Reviewer,
dspCompose™ sends an email to the email address that originated the
request. The email has an Excel file attached that contains the data
entry records with the Reviewer's Reject Reason. The user must correct
the errors in the Excel file and send the corrected file to the External
Email Account to begin the process again.

To reject a role:

1.  Click the **Workflow** link in the email to be directed to the
    request.
    
    Or
    
    Select **Requests** on the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Roles** for a request.:
    
    **NOTE** The count on the **Roles** icon is the number of roles the
    current user can access, not the number of roles for the request.

3.  Click **Reject** for the Review role; the *Reject* page displays.

4.  Click **Edit**.
    
    *[View the field descriptions for the Reject
    page.](../Page_Desc/Reject.htm)*

5.  Enter a justification for the role rejection in **REJECTION
    REASON**.

6.  Click **Save**.

7.  Click **Reject**.

**NOTE:** The user assigned to the initial Data Entry role is notified
that the role must be completed. The rejection reason is included in the
Reject email notification and can be viewed from the *Vertical* View of
the request via the **Rejection Archive**
icon.

## <span id="Perform_a_Partial_Approval"></span>Perform a Partial Approval

If the template was configured to Allow Partial Approval, the Review
role user can reject only the data that is not correct instead of
rejecting all of the records in the request.

**NOTE**: To allow partial approval, select the *Vertical* View for the
Review role on the *[*Template
(Roles)*](../Page_Desc/Template_Role_H.htm)* page. On the **Approve and
Finish Settings** tab, click the **Allow Partial Approval** check box to
enable it. To set this globally, on the
*[Parameters](../Page_Desc/Parameters.htm)* page, on the **Template**
tab, click **Allow Partial Approval.**

**NOTE**: If the request has Org Units assigned, dspCompose™ only sends
workflow emails to users who have Org Unit security for values on the
request.

To partially approve a role:

1.  Click the **Workflow** link in the email to be directed to the
    request.

OR

2.  Select **Requests** on the *Navigation* pane.

3.  Click **Roles** for a request.
    
    **NOTE:** The count on the **Roles** icon is the number of roles the
    current user can access, not the total number of roles for the
    request.

<!-- end list -->

4.  Click **DATA ENTRY** for the **Review** role.

5.  Review the data.

6.  Click the **REJECT** check box for each row of data to reject.

7.  Click **Edit**.
    
    *[View the field descriptions for the Reject
    page.](../Page_Desc/Reject.htm)*

8.  Enter a justification for the role rejection in **REJECTION REASON**
    field.

9.  Click **Save**.

10. Navigate to the *Request (Roles)* page.

11. Click **Approve** to move the approved records to the Post role.

12. Click **Reject**.

13. Enter a justification for the role rejection in **REJECTION
    REASON**.

14. Click **Save**.

**NOTE:** The records that were rejected are entered into a new request
with the description **\[Original Request Description\] (Rejected
Records)**. The initial role users of the new request are sent a
workflow email. The non-rejected records are then carried over for
posting as part of the original request.

**NOTE**: If a role has been selected in the **Partial Approval Reject
Request Role Target** list box (accessible on the *Template (Role)*
page’s *Vertical* View on the **Approve and Finish Settings** tab for
the Review role), that role is assigned the new request and the one that
receives the email that the request is ready for processing. Refer to
[Set Target Role for Request
Rejections](Set_Target_Role_for_Request_Rejections.htm) for more
information

**NOTE:** If the original request had Org Unit values assigned, those
Org Unit values are also assigned to the new request that contains the
rejected records.

**NOTE:** The role rejection reason is included in the Reject email
notification and can be viewed from the *Vertical* View of the Request
via the **Rejection Archive** icon. The rejection reasons entered on the
individual data records will be visible on those records on the Data
Entry role for the new request.
