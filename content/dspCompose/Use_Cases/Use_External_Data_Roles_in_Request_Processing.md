# Use External Data Roles in Request Processing

In addition to the Data, Review, and Post roles, dspCompose™ has a role
type called External Data.

A user assigned to an External Data role receives a spreadsheet with
columns for adding (or in the case of validation failures, updating)
request data.<span> </span> Using an External Data Role can streamline
request data entry: the user does not have to log in to dspCompose™,
<span> </span>but instead works in a spreadsheet that contains only the
required columns. When the spreadsheet is submitted, it has to pass
basic validations to reduce errors and processing time.

When a user creates a request based on a template with an External Data
role, dspCompose™ sends an email with an Excel file attached to the
external contact designated for the External Data role.

This file contains current request data. The user with the External Data
role updates the data in the spreadsheet and emails the file to the
External Data Email Account set up in dspCompose™. If the data in the
spreadsheet passes validations, dspCompose™ imports the data into the
request automatically and continues processing the request.

**NOTE:** An External Data role can also be used in External Request
Scenarios. Refer to [Use External Request
Scenarios](Use_External_Request_Scenarios.htm) and [Set External Role
Contacts for an External Request
Scenario](Set_External_Role_Contacts.htm) for more information.

To use External Data roles in request processing:

  - [Configure Settings for External Data
    Roles](Configure_Settings_for_External_Data_Roles.htm)
  - [Add External Data Role to Global
    Roles](Add_External_Data_Role_to_Global_Roles.htm)
  - [Add an External Data Role Type to a
    Template](Add_an_External_Data_Role_to_Template.htm)
  - [Update External Role Contacts](Update_External_Role_Contacts.htm)
  - [Complete the Spreadsheet as an External Data
    Role](Complete_the_Spreadsheet_as_as_External_Data_Role.htm)
  - [Finish the External Data Role](Finish_the_External_Data_Role.htm)
