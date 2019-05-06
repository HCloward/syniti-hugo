# Add a Tag

Add a tag on the *Tag* page.

**NOTE**: A tag cannot be added on the *Tag – All Types* page.

To add a tag:

1.  Select **Configuration \> Tag Type** from the *Navigation* pane.

2.  Click the icon for a Tag Type.
    
    **NOTE**: If the user clicks the icon for All Tag Types, no tags can
    be added.

3.  Click **Add**. 
    
    [View the field descriptions for the Tag page](../Page_Desc/Tag.htm)

4.  Enter a name for the tag in **NAME** field.

5.  Click **Save**.
    
    **NOTE**: The TYPE field displays the tag type selected when the
    user clicked the icon in step 2.

6.  Click **Vertical View** to further configure the tag, if necessary.

7.  Click **Edit**.
    
    [View the field descriptions for the Tag page](../Page_Desc/Tag.htm)

8.  Enter a brief description of the tag in **Description** field.

9.  Select an option from the **Require Late Comment** list box, if
    applicable.
    
    **NOTE**: The **Require Late Comment** list box displays options to
    indicate if and how users are required to enter a comment when
    finishing a task assigned to this tag after the planned finish date.
    Values are:
    
      - **Inherit** – The Require Late Comment setting is inherited from
        the most granular level in the hierarchy. If the Require Late
        Comment setting is set to <span class="error9">\[None\]</span>,
        Inherit is used by default. The requirement hierarchy’s most
        granular level is task, followed by tag, plan and parameter.  
        Require Late Comment settings set at the task level override
        those set at any other level. If a task's Require Late Comment
        setting is set to <span class="error9">\[None\]</span> or
        Inherit, the task's Require Late Comment setting is inherited
        from the tag level (provided the tag level does not also have a
        Require Late Comment setting of
        <span class="error9">\[None\]</span> or Inherit). If the tag
        level has a Require Late Comment setting of Inherit or
        <span class="error9">\[None\]</span>, Require Late Comment
        settings are then inherited at the plan level (provided the plan
        level does not also have a Require Late Comment setting of
        <span class="error9">\[None\]</span> or Inherit), and so on.  
        For example, the Require Late Comment list box has been set to
        <span class="error9">\[None\]</span> at the parameter level. At
        the plan level, it has been set to Inherit. At the tag level,
        the Require Late Comment list box is set to Yes. At the task
        level, Task A in the Plan has a Require Late Comment setting of
        Inherit. Task B in the plan has a Require Comment setting of No.
        In this scenario, Task A would have a Require Late Comment
        setting of Yes. Task B would have a Require Late Comment setting
        of No. 
      - **Yes** – Tasks assigned to this tag will require a comment when
        the user clicks Next Action on the Work List after the planned
        finish date.
      -  **No** – Tasks assigned to this tag will not require a comment
        when the user clicks Next Action on the Work List after the
        planned finish date.

10. Select an option from **Require Comment** list box, if applicable.

**NOTE:** This list box displays an option to indicate if and how users
are required to enter a comment when finishing a task assigned to this
tag before or on the planned finish date. Values are:

  - **Inherit** – The Require Comment setting is inherited from the most
    granular level in the hierarchy. If the Require Comment setting is
    set to <span class="error9">\[None\]</span>, Inherit is used by
    default. The requirement hierarchy’s most granular level is task,
    followed by tag, plan and parameter.  
    Require Comment settings set at the task level override those set at
    any other level. If a task's Require Comment setting is set to
    <span class="error9">\[None\]</span> or Inherit, the task's Require
    Comment setting is inherited from the tag level (provided the tag
    level does not also have a Require Comment setting of
    <span class="error9">\[None\]</span> or Inherit). If the tag level
    has a Require Comment setting of Inherit or
    <span class="error9">\[None\]</span>, Require Comment settings are
    then inherited at the plan level (provided the plan level does not
    also have a Require Comment setting of
    <span class="error9">\[None\]</span> or Inherit), and so on.  
    For example, the Require Comment list box has been set to
    <span class="error9">\[None\]</span> at the parameter level. At the
    plan level, it has been set to Inherit. At the tag level, the
    Require Comment list box is set to Yes. At the task level, Task A in
    the Plan has a Require Comment setting of Inherit. Task B in the
    plan has a Require Comment setting of No. In this scenario, Task A
    would have a Require Comment setting of Yes. Task B would have a
    Require Comment setting of No. 
  - **Yes** – Tasks assigned to this tag will require a comment when the
    user clicks Next Action on the Work List on or before the planned
    finish date.
  - **No** – Tasks assigned to this tag will not require a comment when
    the user clicks Next Action on the Work List on or before the
    planned finish date.

The tag is then further configured depending on the Tag Type. Refer to
[Configure Logic Tags](Configure_Logic_Tags.htm), [Configure Plan
Tags](Configure_Project_Tags.htm), and [Configure Security
Tags](Configure_Security_Tags.htm) for more information/
