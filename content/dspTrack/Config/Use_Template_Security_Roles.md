# Use Template Security Roles

dspTrack™ is installed with four template security roles that are
configured to different types of users.

The following template security roles are delivered with dspTrack™:

  - **Application Administrator** – Users assigned to this template
    security role perform administrative functions in dspTrack™.
  - **Business User Role** – Users assigned to this template security
    role interact primarily with the Work List.
  - **Sample Project Level Role** – Users assigned to this template
    security role manage an assigned project and all of that project’s
    plans and tasks and have full access (read, write, edit, and delete
    as permitted by the page) to all pages in the project.
  - **Sample Plan Level Role** – Users assigned to this template
    security role manage an assigned plan and all of that plan’s tasks,
    and have full access (read, write, edit, and delete as permitted by
    the page) to all pages in the plan.

An Administrator assigns users to security roles.

The delivered template security roles control access to the pages
outlined in the following table.<span> </span>

**NOTE**: Users can access the pages in the Pages column, as well as all
pages accessed from that page. For example, the security settings set
for the *Tag* page also apply to the *Tag - All Types* page, the *Plan
Tag* page, the *Plan Task Tag* page, and so on, which are accessible
from the *Tag* page.

<table>
<tbody>
<tr class="odd">
<td><p>Pages</p></td>
<td><p>Application<br />
Administrator</p></td>
<td><p>Sample Project<br />
Level Role</p></td>
<td><p>Sample Plan<br />
Level Role</p></td>
<td><p>Business User</p></td>
</tr>
<tr class="even">
<td><p>Dashboard</p></td>
<td><p>Read-only</p></td>
<td><p>Read-only</p></td>
<td><p>Read-only</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="odd">
<td><p>Project and all pages accessed from this page</p></td>
<td><p>No Access</p></td>
<td><p>Write</p></td>
<td><p>Read-only</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="even">
<td><p>Plan, Plan Task and all pages accessed from this page</p></td>
<td><p>No Access</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>Read-only</p></td>
</tr>
<tr class="odd">
<td><p>Reports</p></td>
<td><p>No Access</p></td>
<td><p>Read-only</p></td>
<td><p>Read-only</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="even">
<td><p>All pages accessed from Configuration &gt; Tag</p></td>
<td><p>No Access</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="odd">
<td><p>Configuration &gt; Task List</p></td>
<td><p>No Access</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="even">
<td><p>All pages accessed from Configuration &gt; Work List</p></td>
<td><p>No Access</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="odd">
<td><p>Configuration &gt; Work List Event Rules</p></td>
<td><p>No Access</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="even">
<td><p>Configuration &gt; Work List Event Validations</p></td>
<td><p>No Access</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="odd">
<td><p>Configuration &gt; Task Status</p></td>
<td><p>No Access</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="even">
<td><p>Configuration &gt; Late Comment Codes</p></td>
<td><p>No Access</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="odd">
<td><p>Configuration &gt; Parameters</p></td>
<td><p>Write</p></td>
<td><p>Read-only</p></td>
<td><p>Read-only</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="even">
<td><p>Configuration &gt; Workflow &gt; User Preference</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
</tr>
<tr class="odd">
<td><p>Configuration &gt; Workflow &gt; Log</p></td>
<td><p>Read-only</p></td>
<td><p>No Access</p></td>
<td><p>No Access</p></td>
<td><p>No Access</p></td>
</tr>
<tr class="even">
<td><p>Work List</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
<td><p>Write</p></td>
</tr>
</tbody>
</table>

In addition, certain functionality in dspTrack™ is restricted by
additional factors:

  - Only users who are assigned the template security role of Sample
    Plan Level Role or Sample Project Level Role can activate or
    deactivate a plan on the
    <span style="font-style: italic;">Plan</span> page’s *Vertical* View
    on the Action tab.
  - A user assigned to the Business User role cannot copy a plan or
    import a project into a plan.

**NOTE**: Depending on the needs of each client, security can be
configured in a variety of ways. For example, a user could be assigned
to multiple template<span> </span>security roles to have access to more
pages and functionality. An Administrator can also create WebApp Groups,
assign dspTrack™-specific security definitions to the WebApp Groups, and
assign Security Roles to the WebApp Groups.
