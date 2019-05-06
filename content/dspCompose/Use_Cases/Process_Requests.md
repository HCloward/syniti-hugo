# Process Requests

A *request* is a mass change data process object that is created,
approved and posted in a single batch.

A request is based on a template. Refer to [Create
Templates](Create_Templates.htm) and [Configure
Templates](Configure_Templates.htm) for more information.

Processing a request is the act of entering, reviewing and posting data
to a target ERP system using dspCompose™.

There are three methods to update request data in dspCompose™: manual
change, mass change, or external change. Refer to [Enter Data for a
Request](Create_Requests.htm) for more information.

To process a request, a user must be:

  - Assigned to a role or roles for the template the request is based
    on. Refer to [Add Users to Templates](Add_Users_to_Templates.htm)
    for more information.

  - Assigned to an Org Unit that is also assigned to the request’s
    template if the template uses Org Units. Refer to [Assign Users to
    Org Units](Set_up_Org_Units.htm#Assign_Users_to_Org_Units) for more
    information.

  -  Assigned to Org Unit values assigned to the request if the template
    uses Org Units. Refer to [Set Org Unit Assignment Security for a
    Request](Request_Org_Unit_Assignments.htm#Set_Org_Unit_Assignment_Security_for_a_Request)
    for more information.

**NOTE**: If the Org Unit values assigned to a user are not assigned at
the request level, the user will not be able to process the request. If
the user entered the request, the request still displays on the
*Request* page for the user, but the user cannot process it <span>until
org unit values are assigned to the user.</span>

**NOTE**: If the request uses an External Data role or Org Units or
both, the user must click **Confirm Org Units** or **Confirm External
Contacts** or both before processing requests. These buttons display on
the Page toolbar of the *Request* page. The **Roles** icon is disabled
on the <span style="font-style: italic;">Request</span> page and
processing cannot begin for a request until Org Units and External
Contacts are confirmed.

**NOTE**: Templates in dspCompose™ are highly customizable and can be
configured to have multiple Role IDs with the Role Type of Data. Users
assigned to these roles add or update request data. A template can have
multiple Data Entry roles. The generic term “Data Entry role” is used
throughout this use case, and can refer to one or multiple Role IDs with
the Role Type of Data.

To process a request:

  - [Create Requests](Create_Requests.htm)

  - [Enter Data for a Request](Enter_Data_for_a_Request.htm)

  - [Review Request Data](Review_Request_Data.htm)

  - [Post Request Data to the Target ERP
    System](Post_Request_Data_to_a_Target_ERP_System.htm)

A user can also:

  - [Add a Mass Change Custom Link to a Custom
    Page](Add_a_Mass_Change_Custom_Link_to_a_Custom_Page.htm)

  - [Import a View at the Request-Role
    Level](Import_a_View_at_the_Request%20Role_Level.htm)

  - [Import a File at the Request-Role
    Level](Import_a_File_at_the_Request%20Role_Level.htm)

  - [Validate a Role](Validate_a_Role.htm)

  - [Reset a Role](Reset_a_Role.htm)

  - [Correct Rejected Records](Correct_Rejected_Records.htm)

  - [Review Posting Messages](Review_Posting_Messages.htm)

  - [Correct and Post Failed
    Records](Correct_and_Post_Failed_Records.htm)

  - [View Data from the Finish Download
    Process](View_Data_from_the_Finish_Download_Process.htm)

  - [Change Request Status](Change_Request_Status.htm)

  - [Archive Requests](Archive_Requests.htm)

  - [Monitor Requests](Monitor_Requests.htm)
