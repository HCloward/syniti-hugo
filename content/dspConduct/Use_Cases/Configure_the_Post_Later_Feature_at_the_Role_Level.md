+++
title = 'Configure the Post Later Feature at the Role Level'
solution = 'Master Data Management'
+++

# Configure the Post Later Feature at the Role Level

A Designer can configure a feature that allows a Role Processor with the
Post role type to schedule a post to process at a specified date and
time.

Refer to [Schedule a Post for a Specified Date and
Time](Post_a_Request.htm#Schedule_a_Post_for_a_Specified_Date_and_Time)
for more information.

Before performing this task, [Design a Governance
Hierarchy](dspConduct_Design_Process_Overview.htm) and [add a
role](Add_a_Role.htm) with the Post role type.

When the Designer updates the Schedule Post Allowed setting on the
<span style="font-style: italic;">[Role](../Page_Desc/Role_H_dspConduct.htm)</span>
page’s <span style="font-style: italic;">Vertical</span> View, a
confirmation message displays that determines how the update affects:

  - Scenario \> role combinations that currently use the role and
  - Roles that will be added in the future.

If the user clicks OK, the update cascades through all scenario \> role
combinations that use this role.

If the user clicks Cancel, the setting is retained as the default
setting when roles with a Post role type are added in the future, but
the update does not affect any existing scenario \> role combinations.

For example, a Designer accesses the
<span style="font-style: italic;">Role</span> page’s
<span style="font-style: italic;">Vertical</span> View for the
dspConduct Post role. The Designer clicks the Scheduled Post Allowed
check box to enable it. The confirmation message displays. The Designer
clicks OK.  The check box is enabled. All existing scenario \> role
combination with the dspConduct Post role allow the Role Processor to
schedule a request to post later.

In another example, a Designer disables the Scheduled Post Allowed check
box. The confirmation message displays. The user clicks Cancel. The
check box is disabled. All active requests that use the scenario \> role
combination with the dspConduct Post role still allow the Role Processor
to schedule a request to post later. However, the next time a role with
a Role Type of Post is added, the Schedule Post Allowed check box is
disabled by default and this role will not have the option of specifying
a date and time for a post.

**NOTE**: The Scheduled Post Allowed setting can be set for a specific
scenario \> role combination, and it is at this level that access to the
Post Later feature is controlled. Refer to [Configure the Post Later
Feature at the Scenario - Role
Level](Configure_the_Post_Later_Feature_at_the_Scenario_Role_Level.htm)
for more information.

To configure Post Later at the role level:

1.  Select <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    category.

3.  Click <span style="font-weight: bold;">Vertical View</span> for a
    role with role type of Post.

4.  Click the <span style="font-weight: bold;">Scheduled Post
    Allowed</span> check box to enable it or disable it as needed.

5.  Either:
    
    Click <span style="font-weight: bold;">OK</span>. The change
    cascades through all scenario \> role combinations that use the
    role.
    
    OR
    
    Click <span style="font-weight: bold;">Cancel</span>. The change is
    used as the default setting for roles with the Role post type that
    are added in the future. The change does not affect scenario \> role
    combinations.
