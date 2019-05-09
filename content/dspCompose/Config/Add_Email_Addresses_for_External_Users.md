+++
title = 'Add Email Addresses for External Users'
solution = 'Data Quality'
+++

# Add Email Addresses for External Users

External users, such as those that submit emails for external request
scenarios or those that are assigned to the External Data role, may not
have access to dspCompose™ or the server hosting the platform. These
users do not have user accounts in the platform.

**NOTE**: These external users must still have email addresses
registered in dspCompose™ to be assigned as external contacts for
external request scenarios or to be assigned as contacts for External
Data roles.

Within dspCompose™, external user addresses can be added on these pages:

  - *External Users*

  - *Template (External Request Scenario Email Address)*
    
    **NOTE**: This page is only available when an external request
    scenario has been created for the template. Refer to [Use External
    Request Scenarios](../Use_Cases/Use_External_Request_Scenarios)
    for more information.

<!-- end list -->

  - *Template (External Request Scenario External Role)*
    
    **NOTE**: This page is only available when an External Data role is
    configured for the template. Refer to [Use External Data Roles in
    Request
    Processing](../Use_Cases/Use_External_Data_Roles_in_Request_Processing)
    for more information.

To add an email address for an external user on the *External Users*
page:

1.  Select **Configuration \> External Users** in the *Navigation* pane.
    
    **NOTE**: If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    *[View the field descriptions for the External Users
    page](../Page_Desc/External_Users)*

2.  Enter the email address for the external user in the **EMAIL
    ADDRESS** field.
    
    **NOTE**: The address must be unique. It cannot belong to a user
    account in the platform or to a previously added external user. If
    multiple users share the same email account, dspCompose™ will use
    the name of the first user that was associated with the email
    account.

3.  Enter the name of the external user in the **NAME** field.

4.  Click **Save**.

The email address displays as an option in the EMAIL ADDRESS list box on
the *Template (External Request Scenario Email Address)* page and the
RECIPIENT EMAIL ADDRESS list box on the *Template (External Request
Scenario Email External Role)* page. The format for options in the combo
boxes is \[Email address\] (Name – User ID). To differentiate between
external users and those registered in the platform, an external user’s
email does not display a user ID, while those users registered in the
platform do display a user ID.

Refer to [Add Email Addresses for a
Scenario](../Use_Cases/Add_Email_Addresses_for_a_Scenario) for more
information about adding an email address for an external user on the
*Template (External Request Scenario Email Address)* page. After the
email is added, it displays in the EMAIL ADDRESS list box on the
*External Users* page and the RECIPIENT EMAIL ADDRESS list box on the
*Template (External Request Scenario Email External Role)* page. The
format for options in the combo boxes is \[Email address\] (Name – User
ID). To differentiate between external users and those registered in the
platform, an external user’s email does not display a user ID, while
those users registered in the platform do display a user ID.

Refer to [Set External Role Contacts for an External Request
Scenario](../Use_Cases/Set_External_Role_Contacts) to add an email
address for an external user on the *Template (External Request Scenario
External Role)* page. After the email is added, it displays in the EMAIL
ADDRESS list box on the *Template (External Request Scenario Email
Address)* page and the *External Users* page*.* The format for options
in the combo boxes is \[Email address\] (Name – User ID). To
differentiate between external users and those registered in the
platform, an external user’s email does not display a user ID, while
those users registered in the platform do display a user ID.
