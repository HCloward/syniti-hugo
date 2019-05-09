+++
title = 'Role Dependencies'
solution = 'Master Data Management'
+++

# Role Dependencies

Role dependencies are designed in dspConduct™ to manage the logical
progression of tasks that must be finished to complete a request. For
example, dependencies establish that when processing a request to start
a Post role type, the Application and Review role types must BOTH first
be completed. The buttons on the [Request Role
Task](../Page_Desc/Request_Role_Task) page  for the Post role is
disabled until all Application roles and the Review role that the Post
role depends on are completed.

A Designer can assign one or many dependencies among roles. Those
dependencies can be used across all assigned business processes and
scenarios but only apply if both roles are within the same scenario.  

Role records become active when the dependent roles are completed. A
role is completed when the Role Processor clicks the Finish button on
the [Request Role](../Page_Desc/Request_Role_H) page and the
validations all pass.

As roles are finished, workflow emails are sent to the users assigned to
dependent roles, notifying them that they have work to complete.

**NOTE**: Dependencies must be configured for role types for requests to
process.

This topic contains the following sections:

  - [Dependencies and Role Types](#Dependencies_and_Role_Types)
  - [Add Dependencies to Roles](#Add_Dependencies_to_Roles)
  - [Assign a Condition to a Role Dependency
    Relationship](#Assign_a_Condition_to_a_Role_Dependency_Relationship)

**NOTE**: Data-driven dependencies can be configured so that work on a
role can begin when certain conditions are met.

<span style="font-weight: bold;">NOTE</span>: Scenarios also have
dependencies. Refer to [Add a Dependent Scenario to a
Scenario](Add_a_Dependent_Scenario) for more
information.

## <span id="Dependencies_and_Role_Types"></span>Dependencies and Role Types

The request process uses standard roles with role types that require
specific dependencies.

These dependencies must be configured. Refer to [Add Dependencies to
Roles](#Add_Dependencies_to_Roles) for more information.

The Application type role is used to enter data into pages in the
Content WebApp for preparation to send to the system(s) of record.
Application roles:

  - Must have a lower priority than the Review or Post roles (i.e., the
    Review role must have a higher priority than the Application role).
  - Can have a dependency on other Application type roles.
  - Cannot be dependent on a Review or Post role.  

The Review type role is used to review changes to a preceding dependent
Application type role. Review roles:

  - View all changes made within the execution of a request and approve
    or reject them.  
  - Review everything within the tasks of their dependent Application
    roles within a scenario.
  - Must have a higher priority than the Application type role but a
    lower priority than a Post role.
  - Can only be dependent on Application roles.

The Post type role is used when all Application and Review roles are
complete to send the collected and validated data to the system(s) of
record. A Post role must have a higher priority than a Review role.

<span style="font-weight: bold;">NOTE</span>: The Post role can be
configured to execute automatically if dependencies are completed.
Results can be emailed to the Requestor and any other persona configured
at the request level. This Auto Post Role option is set on the [Scenario
(Roles)](../Page_Desc/Scenarios_Roles_H) page’s
<span style="font-style: italic;">Vertical</span> View.

<span style="font-weight: bold;">NOTE</span>: The Auto Post Role option
can only be set for the Post role.  Refer to [Auto Post a
Request](Post_a_Request#Auto_Post_a_Request) for more information.

## <span id="Add_Dependencies_to_Roles"></span>Add Dependencies to Roles

A Designer can add a dependency to a role, meaning one role cannot be
started until its dependent role is completed.

Dependencies allow a Designer to reuse roles to design dynamic business
processes and scenarios rapidly and effectively.

Before performing this task, [Add Roles](Add_a_Role) with the role
type of Application, Review, and Post.  

To add dependencies to roles in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click the<span style="font-weight: bold;"> Roles</span> icon for a
    category.

3.  Click the <span style="font-weight: bold;">Dependencies</span> icon
    for a role.

4.  If no dependencies exist, the page displays in add mode. Otherwise,
    click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Role (Dependencies)
    page.](../Page_Desc/Role_Dependencies)

5.  Select the role upon which the selected role depends in the
    <span style="font-weight: bold;">DEPENDENT ROLE ID</span> list box.

6.  Set dependencies based on role type. Refer to [Dependencies and Role
    Types](Role_Dependencies#Dependencies_and_Role_Types) for more
    information.

7.  Click
<span style="font-weight: bold;">Save</span>.

## <span id="Assign_a_Condition_to_a_Role_Dependency_Relationship"></span>Assign a Condition to a Role Dependency Relationship

A data-driven dependency condition identifies a condition within a field
when processing a role that determines whether a subsequent dependent
role is processed. A Designer completes this task.

Conditions must be added before they are assigned to a role dependency
relationship. Refer to [Add Data-Driven Dependency Conditions to a
Category](Add_Data_Driven_Dependency_Conditions) for more
information.

**NOTE:** A new condition can be added on *[Role Dependency Condition
Assignment](../Page_Desc/Role_Depend_Cond_Assin_Page)* page.
Conditions must be deleted on the
*[Conditions](../Page_Desc/Conditions)* page*.*

To assign a condition to a scenario dependency relationship in
dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Design** in the *Navigation* pane.

2.  Click the **Roles** icon for a category.

3.  Click the **Dependencies** icon for a scenario.

4.  Click the **Conditions** icon for a scenario dependency.
    
    *[View the field descriptions for the Role Dependency Condition
    Assignment page.](../Page_Desc/Role_Depend_Cond_Assin_Page)*

5.  Select one or more conditions, and then click the **Assign** icon.
