# Create a Request in dspCompose™ From ISA

Report data generated after a rule runs in Information Steward can be
used as the basis for a request in dspCompose™.

<span style="font-weight: bold;">NOTE</span>: To use this feature
dspCompose™ must be installed and licensed and an external request
scenario must exist in dspCompose™. Refer to [Create an External Request
Scenario for an Information Steward-initiated
Request](Create_an_External_Request_Scenario_for_an_Information_Steward%20initiated_Request)
for more information.

<span style="font-weight: bold;">NOTE</span>: The template must be
active in dspCompose™ for the request to be created. Refer to [Activate
the Template](../../dspCompose/Use_Cases/Activate_the_Template) for
more information.

<span style="font-weight: bold;">NOTE</span>: The current user must
belong to the Project Distribution in the ISA that contains the report
to generate requests based on the report in dspCompose™. Refer to
[Activate Users in a Project
Distribution](Add_Users_to_a_Project_Distribution) for more
information.

The data from the report can only be used as the basis for a request one
time after it is run. To create a new request, the report must be
processed again in the ISA.

To generate the request from the ISA:

1.  Select **Information Steward Accelerator \>**
    <span style="font-weight: bold;">Report Data Viewer</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Reports</span> for the
    <span style="font-weight: bold;">PROJECT DISTRIBUTION ID</span>
    configured for the external request scenario. Refer to [Create an
    External Request Scenario for an Information Steward-initiated
    Request](Create_an_External_Request_Scenario_for_an_Information_Steward%20initiated_Request)
    for more information about adding a project to a template’s external
    request scenario.

3.  Click <span style="font-weight: bold;">Create Compose Request</span>
    for the report assigned to the scenario; a confirmation message
    displays.
    
    **NOTE:** This icon does not display if dspCompose™ is not installed
    and licensed.
    
    **NOTE:** If a request has already been created for this run for
    this rule and binding, an error displays. Only one request can be
    created per run.
    
    **NOTE:** If a request that was created from an Information Steward
    Report is subsequently deleted, the Create Compose Request button in
    ISA becomes active for that report, and a new request may then be
    created.

4.  Click <span style="font-weight: bold;">OK</span>.
    
    **NOTE:** The Create Compose Request button is disabled if an
    external request scenario has not been created using the report. In
    this case, the hover text above the icon reads “No Template Mapped.”
    
    **NOTE:** The Create Compose Request button is active if an external
    request scenario has been created using the report but the template
    is not active. In this case, the hover text above the button reads
    “Template Inactive” and an error message displays if the user
    clicks the Create Compose Request button.

5.  Click<span style="font-weight: bold;"> dspCompose Request</span> for
    the report.

<span style="font-weight: bold;">NOTE</span>: This icon does not display
if dspCompose™ is not installed and licensed.

**NOTE:** The
<span style="font-style: italic;">[Request](../../dspCompose/Page_Desc/Request_H)</span>
page in dspCompose™ displays the newly created request. The user
assigned to the first Data Entry role is notified that work can begin on
the request.

<span style="font-weight: bold;">NOTE</span>: An ISA user can create a
dspCompose™ request even though the ISA user is not a user granted
access to the dspCompose™ template. However, once the request is
created, the dspCompose Request button is disabled if the ISA user
doesn’t have access to the dspCompose™
<span style="font-style: italic;">Request</span> page (i.e., the ISA
user’s User ID is not in a WebAppGroup that has access to that page).
