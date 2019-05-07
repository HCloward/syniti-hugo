+++
title = 'Workflow Overview'
solution = 'Platform'
+++

# Workflow Overview

Workflow is an email notification method called from within a WebApp
where an email is sent upon the execution of an event. If a workflow
requires a user to log in to the platform in order to perform a
function, a link can be included in the email to navigate directly to
the relevant page in the WebApp.

Workflow is used in situations where groups, users and fields outside
the context of a particular page are needed, or when the decisions to
manually send an email are particularly complex.

Setting up a workflow involves:

  - Create a workflow view in SQL Server.
  - [Register the view in the platform](Register_Workflow_Views.htm)
  - [Configure Workflow Fields](Configure_Workflow_Fields.htm)
  - [Configure Workflow Links](Configure_Workflow_Links.htm)

## Types of Workflow

## Standard

To use standard workflow authentication, design the workflow view to
specify an email address in the **To** field. Leave the
**WorkflowUserID** field blank on the *Workflow* page in System
Administration. The platform sends an email to the email address
specified in the **To** field. The link in the email navigates through
the standard platform authentication process which could be anonymous,
basic or integrated authentication, depending on how the site is
configured.

## Semi-anonymous

Using semi-anonymous is convenient for the user. When the link in the
email is clicked, the user is automatically signed into their account
without entering credentials. To use semi-anonymous workflow
authentication, design the workflow view to use a platform User ID in
the **To** field instead of an email address. The platform looks up the
user’s email address in the user’s account in order to send the workflow
email. When the recipient clicks the workflow link in the email, they
are automatically logged in as the specified user. The
**WorkflowUserID** field is ignored.

If the site parameter **Support Workflow Authentication** is disabled,
the recipient must log into the DSP when they click the workflow link.
Refer to [Parameters](../Page_Desc/Parameters_All_TabsSysAdmin.htm) for
more information on this field.

## Anonymous

When using anonymous, the email address recipient does not have or need
to have their own account to log in. To use anonymous workflow
authentication, specify a **WorkflowUserID** on the *Workflow* page in
System Administration. The WorkflowUserID select list is populated with
only anonymous users. Make sure the anonymous user selected has
permissions to the page to which it is linked. The email is sent to the
email address specified in the **To** field of the workflow view. Upon
clicking the link in the email, the user is automatically logged in as
the anonymous user selected.
