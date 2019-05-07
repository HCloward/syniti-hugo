+++
title = 'Update External Role Contacts'
solution = 'Data Quality'
+++

# Update External Role Contacts

When a user enters a request that uses a template with an External Data
role, the contact information for that role must be entered on the
*Request (External Role Contacts)* page.

The *Request (External Role Contacts)* page lists information about each
contact, including the email address, and can be updated to reflect the
external contacts for the request.

To update External Role contacts for a request:

1.  Select **Requests** on the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Locate a request that is based on a template with an External Data
    role type.

3.  Click **Vertical View**.

4.  Click the **General** tab.

5.  Click **External Role Contacts**.
    
    **NOTE:** The **External Role Contacts** icon displays the number of
    external role contacts that have a valid email address. Records that
    contain only a Role ID are not included in the count.
    
    **NOTE:** The template upon which the request is based must have an
    External Data role for this button to be active.

6.  Click **Edit**.
    
    *[View the field descriptions for the Request (External Role
    Contacts) page.](../Page_Desc/Request_External_Role_Contacts.htm)*

7.  Enter the name in the **CONTACT NAME** field.
    
    **NOTE:** This name displays in the email sent to the contact.

8.  Enter an email address in the **CONTACT EMAIL ADDRESS** field.

9.  Select the contact’s language from the **LANGUAGE ID** list box.
    
    <span style="font-weight: bold;">NOTE:</span> The LANGUAGE ID sets
    the language used for the <span> </span>workflow message sent for
    the ExternalData event. Language-specific messages are added on the
    *Workflow Message* page and the *Workflow Language Message* page.
    Refer to [Configure Workflow
    Messages](../Config/Configure_Workflow_Messages.htm) for more
    information.

10. Click **Save**.

11. Navigate to the *Request* page’s *Vertical* View.
    
    **NOTE:** If a request uses both External Contacts and Org Units,
    Org Units must be confirmed before External Contacts are confirmed.
    The **Confirm External Contacts** icon is disabled until a user
    clicks the **Confirm Org Units** icon.

12. Click **Confirm External Contacts** in the Page toolbar; a
    confirmation message displays.
    
    **NOTE:** The **Confirm External Contacts** button is not enabled
    until the user entering the request has completed the required
    fields on the *Request (External Role Contacts)* page.
    
    **NOTE:** If a request has an External Data role, the user must
    click **Confirm External Contacts** to activate the **Roles** icon
    on the *Requests* page. The **Roles** icon is disabled, and request
    processing cannot start, until external contacts have been
    confirmed.

13. Click **Ok**.

**NOTE:** Once the Confirm External Contacts process has completed, the
**Confirm External Contacts** button is no longer active.

**NOTE:** The **Roles** button will not be active until both the
External Contacts and the Org Units have been confirmed. Refer to [Use
Org Units](Use_Org_Units.htm) for more information.

Once this request is activated, dspCompose™ sends the spreadsheet to the
user designated as the external contact for the External Data role. This
user completes the spreadsheet and submits it.

<span style="font-weight: bold;">NOTE:</span> Users assigned to the
External Data role enter or update data only. An External Data role
cannot be used to review or post data.
