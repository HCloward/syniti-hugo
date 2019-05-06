# Search for Scenario Role Task Column Assignments while Reviewing a Request

A Role Processor can view which columns are enabled for a request and
which roles have update access to a column. This information can assist
the reviewer when researching which role \> task combination to reject.

For example, if only one role has access to a column and that column
contains an incorrect value, only that role \> task combination must be
rejected.

These steps are performed as part of the review process. Refer to
[Reject a Request](Reject_a_Request.htm) for more information.

The [Enabled Columns by Application
Role](../Page_Desc/Enabled_Columns_by_Application_Role.htm) page
displays the Scenario Role Task Column configuration for enabled columns
for the task selected on the [Request
Role](../Page_Desc/Request_Role_H.htm) page.

<span style="font-weight: bold;">NOTE</span>: The Role Processor can
also view column variants for a task if applicable. Refer to Activate
and Configure Column Variants for more information.

To search for column assignments in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    Requests</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.

3.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    Review role.

4.  Click the <span style="font-weight: bold;">Reviewer Workbench
    </span>icon on the Page toolbar.

5.  Click the <span style="font-weight: bold;">Column Search</span> icon
    for a task.
    
    <span style="font-weight: bold;">NOTE</span>: All enabled columns
    for the task display.

6.  Use the page’s search feature to locate the column name and review
    the ROLE ID (s) that can access the column.
