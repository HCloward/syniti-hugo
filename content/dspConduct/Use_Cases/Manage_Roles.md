+++
title = 'Manage Roles'
solution = 'Master Data Management'
+++

# Manage Roles

A role is a collection of tasks. Each task is performed on a web page
designed to collect and validate information required to support the
scenarios and business processes to which that role is assigned. The web
page is developed at a client’s site and is stored in the Content
WebApp.

Begin designing a business process by adding a role at the category
level, then defining a scenario, a set of roles that can be reused by
business processes.

Each role is assigned a role type to define how role data within a
request can be manipulated. Role types are:

  - <span style="font-weight: bold;">Application</span> – Gathers,
    enters or makes changes to data using pages in the Content WebApp
    for preparation to send to the system(s) of record.
  - <span style="font-weight: bold;">Display</span> – Views data but is
    unable to make changes. Users assigned to a role with a Display role
    type are not active participants in the process.
  - <span style="font-weight: bold;">Review</span> – Evaluates and
    reviews data, either approving or rejecting all changes made within
    the execution of a request. Data can be viewed but not modified. A
    role with this role type can also review the tasks of their
    dependent application roles within a scenario.
  - <span style="font-weight: bold;">Post</span> – Posts data to a
    target system after the roles with Application and Review role types
    have been completed.

To work with roles:

  - [Add a Role](Add_a_Role.htm)
  - [Add Dependencies to
    Roles](Role_Dependencies.htm#Add_Dependencies_to_Roles)
  - [Assign a Condition to a Role Dependency
    Relationship](Role_Dependencies.htm#Assign_a_Condition_to_a_Role_Dependency_Relationship)
  - [Add a Task to a Role](Add_a_Task_to_a_Role.htm)
  - [Enable or Disable Messages for a
    Role](Enable_or_Disable_Messages_for_a_Role.htm)
  - [Add a Conflict to a Role](Add_a_Conflict_to_a_Role.htm)
  - [View dspConduct™ Pages that are Assigned to
    Roles](View_a_Roles_dspConduct_Pages.htm)
  - [Add Custom Business Rules](Add_Custom_Business_Rules.htm)
  - [Auto Finish a Role](Auto_Finish_a_Role.htm)
  - [View the Scenarios Where a Role is Used and the Tasks Assigned to
    that Role](View_a_Roles_Scenarios_and_Tasks.htm)
  - [Configure the Post Later Feature at the Role
    level](Configure_the_Post_Later_Feature_at_the_Role_Level.htm)
  - [Copy a Role](Copy_a_Role.htm)
