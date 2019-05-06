# WebApp Groups

All WebApps, also known as components, have three basic WebApp groups:

  - **PowerUser** – Full access to all pages in the component. The
    creator of a component is automatically added to this group. As a
    recommendation, add as few users to this WebApp group as possible.
    When new pages are created for a component, members of this group
    are automatically added to the PowerUser WebApp group with full page
    rights. Therefore, members of this group always have full access to
    all pages in the component, unless otherwise configured.

  - **User** – Access is determined by the application Designer.

  - **PowerDesigner** – Full access to all pages, not meant to be used
    on site in most cases.
    
    **NOTE:** The term full access means that users have read, write,
    edit, and delete access, as permitted by the page.

**NOTE:** WebApp groups for each component are listed on the *[WebApp
Groups](../Page_Desc/WebApp_Groups_H.htm)* page.

Some components have additional WebApp groups.

## Agent Interface

No additional groups defined.

## Assemble

No additional groups defined.

**NOTE:** Assemble WebApp groups can be viewed using the CranPort
WebApp.

## **AutoGen**

No additional groups defined.

## Automate

Interface Developer - Ability to create and updated interfaces

**NOTE:** Automate WebApp groups can be viewed using the InterfaceServer
WebApp.

## Collect

  - **Service** – Ability to run service pages for Collect via Admin \>
    Resources \> Service Pages
  - **WorkFlowFailureAll** – A user must be assigned to a role that uses
    this WebGroup to receive workflow notifications about table download
    failures in Collect.
  - **WorKFlowFailureByTargetAccess** – A user must be assigned to a
    role that uses this WebGroup to receive workflow notifications about
    table download failures in Collect.

## Common

  - **Analyze** – Full access to only the Analyze pages (Common \>
    Analyze \> Duplicates, Profile and Trace) and Configuration pages
    (Common \> Configuration)

  - **CloudConfigurator** – Not used

  - **Manage** – Not used

  - **ReadOnly** – Read-only access to all pages

  - **RequestPoster**– Passwords for external system data sources are
    stored in Common. Users who are assigned to a role with a role type
    of Post in dspConduct™ must be assigned to this group so that they
    can maintain their passwords.
    
    **NOTE:** If system passwords are used, users do not need to
    maintain their own passwords and do not need access to this WebApp
    group.

<!-- end list -->

  - **Tools** – Full access to only Tools pages (Common \> Tools \>
    Build View and Schedules).

  - **UserManager** – Access provided to the User Management pages
    (Common \> User Management). These pages can be used by a call
    center or help desk of an organization to manage user account and
    password assignment, but do not replace the System Administration
    user and security pages.
    
    **NOTE:** Members of this WebApp group must also be members of the
    User Manager WebApp group in dspConduct™ if they assign users to
    positions in dspConduct™.

## Console

  - **MappingApproval** - Access to the Mapping Approval page only. This
    page is available from the green tab on the Quick Panel, and is
    populated when a field mapping that has been added in Map is waiting
    to be reviewed.

  - **ReadOnly** - Read-only access to all pages

  - **Wavesynchronizer** - Access to buttons and pages related to
    comparing and synchronizing target designs across Waves

## Construct

**NOTE:** The DSP® security key model is implemented in Construct by
Wave Process Area Object ID. Refer to [Getting Started with DSP®
Security for Delivered
Components](GettingStartedwDSPSecurityDlvrdComps.htm) for more
information.

The WebApp groups below can be customized to create more granular access
for smaller groups.

  - **Controlling** – Custom Security Group can be assigned at the page
    level
  - **Finance** – Custom Security Group can be assigned at the page
    level
  - **Materials** – Custom Security Group can be assigned at the page
    level
  - **Sales & Distribution** – Custom Security Group can be assigned at
    the page level
  - **Views** – Not used

## dspCompose™

  - **ReadOnly** – Read-only access to all pages

  - **Requester** – Full access to all Request Data pages (dspCompose \>
    Requests)
    
    **NOTE:** dspCompose™ users must be members of Integrate’s Post
    Monitor WebApp group to post requests using the Post Later feature.

## dspConduct™

  - **ArchiveUser** – Ability to view all archived request data
    (dspConduct \> Archives)

  - **FinalFinishAdmin** – Users in this group receive a workflow
    notification when a final finish package is created but fails to run
    successfully. Users can view all requests and have a read only
    support role.

  - **RoleProcessor** – Access to the Request Role page and all
    dependent pages to process dspConduct™ requests

  - **UserManager** - Access to the Position User page and User Settings
    page.
    
    **NOTE:** Members of this WebApp group must also be members of the
    User Manager group in Common if they assign users to positions.

<!-- end list -->

  - **ReadOnly** – Read-only access to all pages

## dspMonitor™

  - **Designer** – Does not have access to any pages
  - **GroupOwner** – Access to make changes to any group, regardless if
    user is the group owner
  - **Service** – Ability to run service pages for dspMonitor™ via Admin
    \> Resources \> Service Pages
  - **Subscribers** – Receives workflow emails about errors with a link
    to the error report

## dspTrack™

  - **Application Administrator** – Full access to the User Preferences
    page (Configuration \> Workflow \> User Preference) and the Work
    List, and the Parameters page (Configuration \> Parameters). Members
    of this group manage application-level configuration.
  - **Business User**– Read-only access to the Plan pages based on the
    user’s assigned plan. The plan is assigned when the plan is added to
    the template security role’s key. Users in this WebApp group also
    have full access to the User Preferences page (Configuration \>
    Workflow \> User Preference) and the Work List.
  - **Plan User** – Full access to Plan pages associated with the keys
    assigned to the template security role
  - **Project User**– Full access to project pages associated with the
    keys assigned to the template security role.
  - **WorkList only**– Full access to the Work List

## DSP Add-ons

No additional groups defined.

## Information Steward Accelerator

**Administrators** - Access to configure ISA but not to view report
data.

## Information Steward Accelerator Config

No additional groups defined.

## Integrate

**Post Monitor** – Read-only access to Post Monitor, Post Monitor:
Template, Post Files, and Post File Logs pages

**NOTE:** dspCompose™ users must be members of this group to post
requests using the Post Later feature.

## Map

  - **FieldMapper** – Ability to perform (define, edit) field mapping
    actions on the Field Mappings page; user has read-only access to the
    remaining pages
  - **ReadOnly** – Read-only access to all pages
  - **ValueMapper** – Ability to map Source Table values to Target Check
    Table values

## System Administration

  - **Administrator** – Full access to all pages. Only Administrators or
    Power Users of System Administration have security to create
    WebApps.

  - **Audit** – Full access to all audit pages (Data Sources \> Audit)

  - **CTS** – Full access to all CTS pages (i.e., pages under the CTS
    menu)

  - **CustomizationManager** – Access to User/Role/Site level
    customization pages for creating and managing Custom Links, Custom
    Dashboard Layouts, Quick Links, and others.

  - **Customizer** – By default, users have access to this group which
    gives them the ability to replace Dashboards with alternate layouts.
    
    **NOTE:** To create dashboards, users must be a member of the
    CustomizationManager WebApp group.

<!-- end list -->

  - **DataSources** – Full access to all Data Source pages (as in, pages
    under the Data Source menu)

  - **Debugger** – Read only access to exception stack traces.

  - **Designer** – Enables Design capabilities (as in, Design link on
    the Gear toolbar icon). Full access to all WebApp pages (i.e., pages
    under the WebApps menu).
    
    **NOTE:** Designers only have access to modify WebApps to which they
    have security.
    
    **NOTE**: A user who belongs to this WebApp group can use the Show
    SQL feature to view the SQL for the page. Refer to [Show
    SQL](Show_SQL.htm) for more information.

<!-- end list -->

  - **Language** – Full access to all language pages (as in, pages under
    the Translations menu)
  - **Search** – Full access to all search and index pages (pages under
    Configuration \> Search, Data Sources \> Index, Resource \> Bulk
    Duplicate Detection, and Resource \> Monitor)
  - **Security** – Full access to all security pages (as in, pages under
    the Security menu)
  - **Service** – Not meant for users, but to assign to Service pages so
    that the background service can access them

## Target Design

**ReadOnly** – Read-only access to all pages.

## Transform

  - **ReadOnly** – Read-only access to all pages
  - **ReportsOnly** – Read-only access to pages accessed via Reports and
    My Reports
  - **Service** – Ability to run service pages for Transform via Admin
    \> Resources \> Service pages
