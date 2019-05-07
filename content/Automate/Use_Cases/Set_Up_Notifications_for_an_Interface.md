+++
title = 'Set Up Notifications for an Interface'
solution = 'Platform'
+++

# Set Up Notifications for an Interface

Roles are used for notification purposes, such as emailing information
pertinent to the completion of an interface. Users can be assigned to
multiple roles.

A Business role and a Development role can be assigned to each
interface. These roles can receive notification emails depending on
notification options.

To set up notifications for an interface in Automate:

1.  Set up Users and Roles, which drive email notifications. Refer to
    [Add Roles](Add_Roles.htm) and [Assign Users to
    Roles](Assign_Users_to_Roles.htm) for more information
2.  [Fill Out Contact Info](#Fill)
3.  [Sync Instances](#Sync)
4.  [Configure Email Sender](#Configur)
5.  [Configure and Test Mail Server](#Configur2)

## <span id="Fill"></span>Fill Out Contact Info

The interface will not send an email if the Contact Info fields are
blank.

Before performing this task, [Add Roles](Add_Roles.htm) and [Assign
Users to Roles](Assign_Users_to_Roles.htm).

To fill out contact info in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click **Vertical View** for an interface.

3.  Click the **Contact Info** tab.

4.  Click **Edit**.
    
    [View the field description for the Contact Info tab on the
    Interfaces page’s Vertical
    View](../Page_Desc/Interfaces.htm#_Contact_Info)

5.  Enter a message in the **Message Success** field.
    
    **NOTE:** The Message Success field is used as the body of the email
    message when the interface completes with a successful status.

6.  Enter a message in the **Message Failure** field.
    
    **NOTE:** The Message Failure field is used as the body of an email
    message when the interface fails.
    
    **NOTE:** The Message Success and Message Failure fields support
    dynamic substitution, where any value preceded and followed by \# is
    replaced (i.e., dynamically substituted) at run time.

7.  Select a role from the **Business Role** list box.
    
    **NOTE:** The Business Role indicates the recipient of an automated
    interface email.

8.  Select an option from the **Business Notification Option** list box
    to configure when to send an automated interface email to the
    specified Business Role. Options are:
    
      - **Always** **–** Sends an email notification when an interface
        completes, regardless of the interface status.
    
      - **Failure Only** **–** Sends an email notification only if the
        interface instance encounters an unexpected error. For example,
        if a stored procedure references a SQL object that does not
        exist. Failure emails are NOT sent when a validation registered
        on an interface event captures a problem and ends the execution
        of the interface instance.
    
      - **Success Only** **–** Sends an email notification only if the
        interface successfully completes.

9.  Select a role from the **Development Role** list box.
    
    **NOTE:** The Development Role indicates the recipient of an
    automated interface email.

10. Select an option from **Development Notification Option** list box
    to configure when to send an automated interface email to the
    specified Development Role. Options are:
    
      - **Always** **–** Sends an email notification when an interface
        completes, regardless of the interface status.
    
      - **Failure Only** **–** Sends an email notification only if the
        interface instance encounters an unexpected error. For example,
        if a stored procedure references a SQL object that does not
        exist. Failure emails are NOT sent when a validation registered
        on an interface event captures a problem and ends the execution
        of the interface instance.
    
      - **Success Only** **–** Sends an email notification only if the
        interface successfully completes.

Continue with [Sync Instances](#Sync).

## <span id="Sync"></span>Sync Instances

Before performing this task:

  - [Add Roles](Add_Roles.htm)
  - [Assign Users to Roles](Assign_Users_to_Roles.htm)
  - [Fill Out Contact Info](#Fill)

The Instance field MUST be identical across the following three pages:

  - The *[Parameters](../Page_Desc/Parameters.htm)* page in Automate.
  - The *[Role (Instance)](../Page_Desc/Role_Instance.htm)* page in
    Automate.
  - The
    *[Parameters](../../Sys_Admin/Page_Desc/Parameters_All_TabsSysAdmin.htm)*
    page in System Administration.

Continue with [Configure Email Server.](#Configur)

## <span id="Configur"></span>Configure Email Sender

Emails are sent from a user assigned to the Admin Role. The default
Admin Role is “Admin.”

Before performing this task:

  - [Add Roles](Add_Roles.htm)
  - [Assign Users to Roles](Assign_Users_to_Roles.htm)
  - [Fill Out Contact Info](#Fill)
  - [Sync Instances](#Sync)

Configuring email sender settings is a three-step process:

1.  Configure the Admin role. Whatever role is deemed as the Admin role,
    verify that role is set in the Admin Role field on the
    *[Parameters](../Page_Desc/Parameters.htm)* page.
2.  Look up the user assigned to Admin Role on the *[Role
    (Instance)](../Page_Desc/Role_Instance.htm)* page. Make note of the
    user(s) assigned to this role.
3.  Verify the user has a valid email address by reviewing the E Mail
    Address field on the
    *[Users](../../Sys_Admin/Page_Desc/Users_H.htm)* page in System
    Administration. An email address must contain a “@” symbol and a
    period (.) to be considered valid.

Continue with [Configure and Test Mail Server](#Configur2).

## <span id="Configur2"></span>Configure and Test Mail Server

Before performing this task:

  - [Add Roles](Add_Roles.htm)
  - [Assign Users to Roles](Assign_Users_to_Roles.htm)
  - [Fill Out Contact Info](#Fill)
  - [Sync Instances](#Sync)
  - [Configure Email Server](#Configur)

Make sure a working mail server is configured:

1.  Select **Admin \> Configuration \> Parameters** in the *Navigation*
    pane.
2.  Verify the **Email Server** field is correctly populated. If not,
    update the field.
3.  Click the **Test Email** button to test the mail server connection.
    An email is sent to the email address configured for the user
    assigned to the Admin Role. If an email was not received, the mail
    server is not working.
