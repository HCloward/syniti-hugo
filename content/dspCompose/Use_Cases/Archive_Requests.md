+++
title = 'Archive Requests'
solution = 'Data Quality'
+++

# Archive Requests

Requests are archived based on retention intervals that are tied to
<span id="dspCompose Request Status" class="popUpLink">\>request
status</span>.

Retention intervals are set at the global level, but can also be
configured for a template. Refer to [Configure Request
Statuses](../Config/Configure_Request_Statuses) and [Configure
Retention Parameters](Configure_Retention_Parameters) for more
information.

Once the retention interval for a request’s request status has been met,
requests are archived when:

  - A service page runs
  - A user clicks **Archive Requests** on the *Archive Requests* page

**NOTE**: If a request is deleted, it is not archived.

To view all archived requests, select **Reports \> Archived Requests**
on the *Navigation* pane.

To archive requests:

1.  Select **Configuration \> Archives \> Archive Requests** on the
    *Navigation* pane.
2.  Click **Archive Requests**; a confirmation message displays.
3.  Click **OK**.

## <span id="Delete_Archived_Requests"></span>Delete Archived Requests

The delete archive feature permanently removes archived requests from
the system.

To delete archived requests:

1.  Select **Configuration \> Archives \> Archive Delete** on the
    *Navigation <span style="font-style: normal;">pane</span>*.

2.  Click **Edit**.
    
    <span class="ListNumber">*[View the field descriptions for the
    Archive Delete page.](../Page_Desc/Archive_Delete)*</span>

3.  Select a date in **DELETE ARCHIVE BEFORE** field.

4.  Use the sliders to select a time.

5.  Click **Done**.

6.  Click **Save.**

7.  Click **Delete Archives**; a confirmation message displays.

8.  Click **Ok**.

**NOTE:** All requests added on or before the date entered are deleted
from the archives.
