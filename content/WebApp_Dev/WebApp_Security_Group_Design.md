+++
title = 'WebApp Group Design'
solution = 'Platform'
+++

# WebApp Group Design

When designing an application, the Designer should know the different
types of users who will access the application. Some applications are
only meant to have a single user who has full access to the features,
pages, and functionality that will be put into the application. However,
more elaborate and partitioned applications may expect different types
of users to have access to certain pages.

Refer to [Set Security for a Custom
WebApp](Set_Security_for_a_WebApp) for general information.

WebApp Groups are a good way for Application Designers to convey
expected roles to the On Site Administrator, without requiring “Use
Case” documentation.

Pitfalls of Using WebApp Groups:

  - Groups may go unnoticed and under-used. Security Administrators may
    not know how to add control logic to supplement the WebApp Group’s
    functionality.
  - Groups are often an after-thought to an application’s
    implementation. Adding them disrupts the original flow of the
    application’s design.

**NOTE:** User profiling upfront can help prevent these pitfalls, by
understanding the usage scenarios and planning for them.

  - Out of the box, WebApp groups have limited restriction capabilities
    (Page Access, Insert access, Update access, Delete access). However,
    WebApp Groups can be supplemented by more granular features:
      - boaUserGroup can be used as an Environment variable to restrict
        control view information
      - System Views boaWebAppGroupUserSel and boaWebAppSel can be used
        in conjunction with other page-related views

**NOTE:** Unlike with User Control Views, there is no record-per-group
equivalent control view. When attempting to implement boaUserGroup
filter in, for example, a Toolbar View, there is the possibility of a
user existing in two groups.

Benefits of Using WebApp Groups:

Web App Group restriction logic is usually more simplified than trying
to compute it at a [*User Control View or Data Control
View*](Control_Views) level. The overhead on this is much less,
increasing performance while maintaining relatively simple logic. The
overhead also scales with WebApp Group count, instead of User count,
where applications rarely have more than 10 Groups.

Access manipulation of WebApp Groups is performed in System
Administration, instead of within the WebApp itself. This reduces the
number of configuration pages required within the WebApp and does not
require user configuration to happen in both the WebApp and System
Administration.
