# Configure Logic Tags

Once a tag with a Logic tag type has been added, it can be further
configured by adding rules and validations that will execute for any
task assigned to the tag.

Validations are stored procedures or views that have been written and
saved in a data source that is registered in the DSP®. A validation
executes when an event occurs, and confirms that a process is valid. If
the validation fails, processing stops. For example, a validation is
registered to a Receive Email event. The validation confirms that an
email received at a designated address has an attachment in a specified
format. If the attachment is in a valid format, the validation passes
and processing can continue. However, if the attachment is in an invalid
format, the validation fails, and processing stops.

Rules are stored procedures that have been written and saved in a data
source that is registered in the DSP®. A rule runs during a process to
manipulate data, perform an extra step in the process, or finish a task
the process starts. For example, a rule could dictate that once table A
has been populated with 1000 rows of data, that data is archived in a
table B and removed from table A.

**NOTE**: When a Work List Event rule or validation is added to a task
using a tag, then the rule or validation can only be edited at the tag
level (Configuration \> Tag \> Tag Type \> Registrations \> Rules or
Validations).

To add a rule to the tag:

1.  Select **Configuration \> TagType** in the *Navigation* pane.

2.  Click **Tags** for the Logic Tag Type.

3.  Click **Registrations** for the tag.

4.  Click **Rules**.
    
    **NOTE**: If no rules exist, the page displays in add mode.
    Otherwise, click <span style="font-weight: bold;">Add.</span>
    
    [View the field descriptions for the Work List Event Rules - Tag
    Registration
    page](../Page_Desc/Work_List_Event_Rules_Tag_Registration.htm)

5.  Enter a value in the **PRIORITY** field.
    
    **NOTE**: The rule runs in this order if multiple rules are assigned
    to the
    tag<span class="MsoCommentReference" style="font-size: 8.0pt;font-family: Arial, sans-serif;color: #E1E1E1;"> </span>.

6.  Select the data source that contains the rule from the **DATA SOURCE
    ID** list box.
    
    **NOTE**: These options are data sources registered in Common. Refer
    to [Register a Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.

7.  Select the rule in the **RULE** list box.
    
    **NOTE**: This rule must have been written and stored in the data
    source.

8.  Select the event that triggers the rule to run in the **WORK LIST
    EVENT ID** list box.
    
    **NOTE**: This option sets whether the rule runs when work on the
    task<span> </span> begins or ends (i.e., when a user clicks Next
    Action on the Work List)

9.  Click the <span style="font-weight: bold;">ACTIVE</span> check box
    to disable it if the rule should not be run.

10. Enter a comment about the rule in **COMMENT** field if necessary.  

11. Click **Save**.

The rule will run for tasks assigned to this tag depending on the option
selected in the WORK LIST EVENT ID list box.

Work List Event Rules can also be registered at the
[plan](Register_Work_List_Event_Rules_for_a_Plan.htm) level, [Work List
Item](Register_WorkList_Event_Rules_WorkList_Item.htm) level and [Plan
Task](Register_Work_List_Event_Rules_for_a_Plan_Task.htm) level.

Refer to [Register Work List Event
Rules](Register_Work_List_Event_Rules.htm) for more information about
viewing and editing all rules from one page, and about parameters that
can be used in Work List Event Rules.

To add a validation<span> </span>to the tag:

1.  Select **Configuration \> Tag Type** in the *Navigation* pane.

2.  Click **Tags** for the Logic Tag Type.

3.  Click **Registrations** for the tag.

4.  Click **Validations**.
    
    **NOTE**: If no validations exist, the page displays in add mode.
    Otherwise, click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Work List Event Validations -
    Tag Registration
    page](../Page_Desc/Work_List_Event_Validations_Tag_Registration.htm)

5.  Enter a value in the **PRIORITY** field.
    
    **NOTE**: The validation runs in this order if multiple validations
    are assigned to the
    tag<span class="MsoCommentReference" style="font-size: 8.0pt;font-family: Arial, sans-serif;"> </span>.

6.  Select whether the validation is a Stored Procedure or a View in the
    **VALIDATION TYPE** list box.

7.  Click **Save**; the Vertical View displays.

8.  Select the data source that stores the view or stored procedure in
    the **Data Source ID** list box.
    
    **NOTE**:
    <span style="font-size: 14.6666669845581px;line-height: normal;orphans: auto;text-indent: -60px;widows: 1;-webkit-text-stroke-width: 0px;display: inline !important;float: none;background-color: #ffffff;">These
    options are data sources registered in Common. Refer
    to</span><span class="Apple-converted-space"> </span>[Register a
    Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.

9.  Select the name of the stored procedure or view from the
    **Procedure/View** list box.

10. Select whether the validation runs when a task starts or ends in the
    **Work List Event ID** list box.

11. Enter a brief message that will display to the user when the
    validation fails in the **Validation Message** box.
    
    **NOTE**: The message should provide information about what may have
    caused the error and potential solutions if applicable.

12. Enter a detailed description of the validation in the
    **Description** box.
    
    <span>**NOTE**: This description should contain notes about the
    validation that serve as a summary of the SQL code so that another
    user does not have to review the SQL code to understand the
    validation.</span>

13. Click **Save**.

The validation will run for the task assigned to this tag depending on
the option selected in the WORK LIST EVENT ID list box.

Work List Event Validations can also be set at the [Plan
Task](Register_WorkList_Event_Validations_Plan_Task.htm) level, [Work
List Item](Register_WorkList_Event_Valid_WorkList_Item.htm) level, and
the [plan](Register_WorkList_Event_Validations_Plan.htm) level.

Refer to [Register Work List Event
Validations](Register_Work_List_Event_Validations.htm) for more
information about viewing and editing all validations from one page, and
about parameters that can be used in Work List Event validations.

Refer to [Assign a Tag to Tasks](Assign_a_Tag_to_Tasks.htm) to continue
with configuring Logic tags.
