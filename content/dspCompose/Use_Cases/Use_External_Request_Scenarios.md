# Use External Request Scenarios

An external request scenario tells dspCompose™ to create a request when
an external data email account configured in dspCompose™ receives an
email sent from a valid email account.

While an external request scenario can be configured to simply create a
request when an email is received, templates may also be configured to
use an external request scenario that creates an Excel-initiated
request. In this case, dspCompose™ accepts an Excel file attached to the
email. The Excel file provides data for the first Data Entry role in the
workflow. Not only will the request be created, but the worksheet data
from the Excel file will be inserted into the table used by the first
Data Entry role (after certain conditions are met).

This section contains the following topics:

  - [External Request Scenarios and Org
    Units](#External_Request_Scenarios_and_Org_Units)
  - [External Request Scenarios and External Data
    Roles](#External_Request_Scenarios_and_External_Data_Roles)
  - [Set up Email Validations](Set_up_Email_Validations.htm)
  - [External Request Scenarios](External_Request_Scenarios.htm)
  - [External Request Scenarios that Create Excel-initiated
    Requests](External_Request_Scenarios_that_Create_Excel_Initiated_Requests.htm)
  - [Add Email Addresses for a
    Scenario](Add_Email_Addresses_for_a_Scenario.htm)

Additionally, an external request scenario can be configured to create
requests using data from Information Steward (IS) reports.

Refer to [External Request Scenarios that Create Information
Steward-initiated
Requests](../../ISA/Use_Cases/External_Request_Scenarios_that_Create_Information_Steward%20initiated_Requests.htm)
for more information about this type of external request
scenario.

## <span id="External_Request_Scenarios_and_Org_Units"></span>External Request Scenarios and Org Units

When a template uses Org Units and an external request scenario,
dspCompose™ works with Org Units differently than it does when a request
does not use Org Units.

When the template is activated, dspCompose™ displays a message warning
that requests created from the external request scenario will be
assigned Org Unit values based upon the **Org Unit Security Level** and
**Only Show Org Unit Values Assigned to Requester** values assigned to
the template. Access this list box and  check box on the *Templates*
page’s *Vertical* View on the **Advanced** tab. Refer to [Set Org Unit
Assignment Security for a
Request](Request_Org_Unit_Assignments.htm#Set_Org_Unit_Assignment_Security_for_a_Request)
for more information.

When a user with a valid email account for the external request scenario
sends an email to the external data email account, dspCompose™ creates
and activates the request. The request is assigned to the lowest
priority role in the workflow and the **Confirm Org Units** icon on the
Page toolbar is disabled. In all other cases in which Org Units are used
with a template, a user must click **Confirm Org Units** on the *Request
(Roles)* page before the request roles are activated.

If the check box **Only Show Org Unit Values Assigned to Requester** is
enabled for the template, dspCompose™ does not copy Org Unit values into
the request created by an external request scenario, regardless of how
Org Unit security is set on the template. Access the check box on the
*Templates* page’s *Vertical* View on the **Advanced**
tab.

## <span id="External_Request_Scenarios_and_External_Data_Roles"></span>External Request Scenarios and External Data Roles

A user assigned to an External Data role receives a spreadsheet with
columns for adding (or in the case of validation failures, updating)
request data. Using an External Data Role can streamline request data
entry: the user does not have to log in to dspCompose™, but instead
works in a spreadsheet that contains only the required columns. When the
spreadsheet is submitted, it has to pass basic validations to reduce
errors and processing time.

Refer to [Use External Data Roles in Request
Processing](Use_External_Data_Roles_in_Request_Processing.htm) for more
information.

External Data roles can be used with external request scenarios.

If the External Data role is the first role in the template, the
External Data role will receive an email with a blank Excel file
attached when the request for the external request scenario is created.
At this point, the External Data role enters data in the Excel file and
sends it to the external data email account configured for dspCompose™.
Refer to [Complete the Spreadsheet as an External Data
Role](Complete_the_Spreadsheet_as_as_External_Data_Role.htm) for more
information.

External Data roles can also be used with external request scenarios
that create Excel-initiated requests with one exception: An External
Data role cannot be the first role in the scenario’s associated template
