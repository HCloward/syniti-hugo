# Use Org Units

Organizational Units (Org Units) are used to set request data security
by restricting data a user can access. They are based on a type of data
that defines access within an organization, such as plant, company code,
sales organization, division or department (though Org Units can be used
to represent any data type).

Org Units are:

  - Set up in dspCompose™

  - Assigned to users

  - Assigned to templates.

Once the template is generated, dspCompose™ creates an Org Unit table
that contains the Org Unit, request ID and user ID.

***Beyond this, no other Org Unit functionality is included or automated
in dspCompose™.***

Org Units are used to create customized solutions. An advanced user,
usually a BackOffice Consultant, could implement this feature to
restrict list box values, to limit access to a role during the request
process, or to set role dependencies. ***Users can implement Org Units
however they wish. It is up to the implementer to create solutions based
on this tool.***

This section describes how to set up Org Units and includes best
practices while using them.

Org Units remove the need to create duplicate templates for specific
user groups. Users can create one template and segment it by Org Unit
values, configuring one set of validations, one set of dependencies and
configuration options. For example, a template to perform a material
change can be segmented by plant. At the request level, the Org Unit
values, or the specific plants, can be assigned so that only users who
are assigned to those plants can view or add request data.

Org Units are not required to use dspCompose™. Even if a template has
Org Units assigned, a request based on that template does not have to
use them.

To use Org Units:

  - [Create Org Units](Set_up_Org_Units.htm#Create_Org_Units)
  - [Assign Users to Org
    Units](Set_up_Org_Units.htm#Assign_Users_to_Org_Units)
  - [Add Org Units to a
    Template](Set_up_Org_Units.htm#Add_Org_Units_to_a_Template)
  - [Set Org Unit Assignment Security for a
    Request](Request_Org_Unit_Assignments.htm#Set_Org_Unit_Assignment_Security_for_a_Request)
  - [Configure and Confirm Request Org Unit
    Assignments](Request_Org_Unit_Assignments.htm)
  - [Incorporate the Security View into Request
    Processing](Incorporate_the_Security_View_into_Request_Processing.htm)
