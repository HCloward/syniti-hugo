+++
title = 'Effectively Implementing Security Definitions (Role Security)'
solution = 'Platform'
+++

# Effectively Implementing Security Definitions (Role Security)

Security Definitions (commonly referred to as Role Security
Configuration) is a feature that enables application developers to:

  - Internally restrict data access to particular users (or roles) and
  - Provide an external API to other applications to secure their data
    on the source of the data itself. This allows inter-dependent
    applications to share a single security model across the platform.

Refer to [Set Security for a Custom
WebApp](Set_Security_for_a_WebApp) for general information.

The secured data is then made available to users via direct access or
Roles. Good candidates for data that can be secured via these Security
Definitions are:

  - Low record count tables / values (i.e., only ever be \<100 unique
    values)
  - Very high level data sets (not low on the hierarchy, data won’t
    build exponentially)
  - Landing page data that’s usually the first page(s) the user sees
    when utilizing the app

**NOTE**: You do NOT have to create a security definition only using a
table’s primary keys. The Security Definition keys could be a
commonality that data sets share. It could also be user configuration
data driven, not predefined by the application Designer, as long as the
application Designer is aware of the likely data sets that will make up
the Security Definitions data set.

These data sets are managed by an onsite Administrator on a daily basis.
The fewer total Security Definition records there are, the easier it is
for them to manage.

**NOTE**: If there is already a role that contains the relevant Web
Application access and data access, the user can be directly assigned to
the role from the *Roles* page.

**NOTE**: If the user is not expected to participate in any Roles,
directly application access can be grated via the WebApp Security pages.

For example, an application allows users to create a request, which can
then be approved or rejected by another user, and then finally completed
by a final user.

This application has three roles built into it, “Requester,” “Approver,”
and “Request Completer” where:

  - Requester – Can create, edit, and remove requests
  - Approver – Can accept or reject requests (but not delete)
  - Request Completer – Can close the request by completing it

These roles allow the Designer to manipulate application flow and
restrict access to an individual user, to show them only what’s relevant
for the task they are attempting to accomplish.
