+++
title = 'Create Requests'
solution = 'Data Quality'
+++

# Create Requests

To create a request a user must:

  - Be a member of the Requester WebApp group and
  - Have permission to access at least one active template.

Refer to [Set Up Security](../Config/Set_Up_Security.htm) and [Grant
Template Access at the Template
Level](Add_Users_to_Templates.htm#Grant_Template_Access_at_the_Template_Level)
for more information.

A request can also be created automatically using External Request
Scenarios. Refer to [Use External Request
Scenarios](Use_External_Request_Scenarios.htm) for more information.

To create a request in dspCompose:

1.  Select **Requests** on the *Navigation* pane.

2.  Click **Add**; the *Vertical* View displays.
    
    *[View the field descriptions for the Request page’s Vertical
    View.](../Page_Desc/Request_H.htm)*

3.  Enter a request description in the **Description** field.

4.  Select a template from the **Template** list box.

5.  Click **Save**.

6.  Click the **Connections** icon to select a connection to the target
    system for each process template.
    
    **NOTE:** The connection is used to post the data during the posting
    role. dspCompose™ can post to multiple instances of the target
    system.
    
    **NOTE:** The Process Templates for which a connection can be set
    are based on:
    
      - The Integrate template type. Refer to [Create a Basic
        Template](../../../Platform/Integrate/Use_Cases/Create_a_Basic_Template.htm)
        in Integrate for more information.
      - The "Allowed Connections" configured at the Integrate Process
        Template level. Refer to [Set Available Connections at the
        Process Template
        Level](../../../Platform/Integrate/Use_Cases/Set_Connections_at_the_Process_Template_Level.htm)
        in integrate for more information.

<!-- end list -->

1.  Click **Edit**.

2.  Select the connection from the **CONNECTION ID** list box.
    
    **NOTE:** If a user adds a request based on this template and does
    not select a connection ID, the default connection assigned to the
    Integrate Template is used for the request. Refer to [Establish a
    Connection to a Target
    System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
    for more information.

3.  Click **Save**.

**NOTE:** A requester can create a request, but may not be able to view
the request if the request uses Org Units and the requester does not
have security to an Org Unit on the template and an Org Unit value on
the request. Refer to [Use Org Units](Use_Org_Units.htm) for more
information.

**NOTE:** When the request is saved, the roles associated with the
template are added by default, and the request is considered active.

**NOTE:** If the **Roles** icon is disabled on the *Request (Roles)*
page, and the request has Org Units or External Contacts assigned, the
user must click **Confirm Org Units** or **Confirm External Contacts**
on the Page toolbar prior to processing the request. The **Roles** icon
will then become active. If both Org Units and External Contacts are
used in the request, click **Confirm Org Units** first.

After creating the request, person(s) responsible for the Data Entry
role(s) can populate the data to be posted for the request using one of
these methods.

  - Upload data from a view in SQL Management Studio. Refer to [Import a
    View at the Request-Role
    Level](Import_a_View_at_the_Request%20Role_Level.htm) for more
    information.

  - Upload data from an Excel Spreadsheet.  
    After creating a request, a user can generate a spreadsheet in a
    specific format that can be used for data entry. This spreadsheet
    can then be imported into dspCompose™. Refer to [Import a File at
    the Request-Role
    Level](Import_a_File_at_the_Request%20Role_Level.htm) for more
    information.

  - Manually enter data. Refer to [Manually Change
    Data](Enter_Data_for_a_Request.htm#Manually_Change_Data) for more
    information.

**NOTE:** Templates in dspCompose™ are highly customizable and can be
configured to have multiple Role IDs with the Role Type of "Data." Users
assigned to these roles add or update request data. A template can have
multiple Data Entry roles. The generic term “Data Entry role” is used
throughout this use case, and can refer to one or multiple Role IDs with
the Role Type of Data.

**NOTE:** A rule can be associated with this template level event. Refer
to [Register Rules to Template-level
Events](Register_Rules_to_Template%20level_Events.htm)  for more
information.
