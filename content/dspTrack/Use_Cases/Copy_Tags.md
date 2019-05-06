# Copy Tag Tasks

When a user copies a Tag, all of the tasks assigned to the tag are
copied. The following items associated with all of the tasks can also be
copied:

  - Users assigned to the tasks assigned to the tag
  - Task dependencies for all tasks assigned to the tag
  - Tags assigned to all tasks assigned to the tag
  - Work List Event rules for all tasks assigned to the tag
  - Work List Event validations for all tasks assigned to the tag

**NOTE**: Because tags are not plan specific, a user must specify the
source plan and the destination plan when copying a tag.

A tag can be copied from the:

  - *Tag* page (Configuration \> Tag Type \> Tag Type icon)

  - *Tag – All Types* page (Configuration \> Tag Type)

  - *Plan Task Tag* page (Configuration \> Tag Type \> Tag Type icon
    \>Tasks)

  - *Plan Tag* page (Project \> Plans \> Tags)

To copy a tag:

1.  Navigate to the page to copy the tag.

2.  Select a tag in **NAME**.

3.  Click **Copy Tag Tasks**.
    
    **NOTE**: All items are enabled for copying by default.

4.  Click a check box to disable it if an item should not be copied.

5.  Click the **Keep Source Tag** check box to enable it if the original
    tag name should be applied to the copy of the tag in the destination
    plan.

6.  Click **Edit**.
    
    [View the field descriptions for the Copy Tag Tasks
    page](../Page_Desc/Copy_Tag.htm)

7.  Enter a suffix in the **Task Copy Suffix** field if the names of all
    copied tasks should have a suffix.

8.  Select a plan in the **Destination Plan ID** list box.
    
    **NOTE**: This is the plan to which the tag’s tasks will be copied.

9.  Select a plan in the **Source Plan ID** list box.
    
    **NOTE**: This is the plan from which the tag’s tasks will be
    copied.

10. Enter a name for the copy of the tag in the **Name** field.

11. Enter a description of the copy of the tag in the **Description**
    field.

12. Click **Save**.

13. Click **Copy Tag Tasks**; a confirmation message displays.

14. Click **Ok**.

The copied tag displays on the *Tag* page applied to the plan and tasks
in the Destination plan.
