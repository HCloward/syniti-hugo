+++
title = 'Register Work List Event Validations'
solution = 'Platform'
+++

# Register Work List Event Validations

Work List Event Validations can also be set at the [Plan
Task](Register_WorkList_Event_Validations_Plan_Task.htm) level, [Work
List Item](Register_WorkList_Event_Valid_WorkList_Item.htm) level, the
[tag](Configure_Logic_Tags.htm) level, and  the
[plan](Register_WorkList_Event_Validations_Plan.htm) level, and can be
set to run when work on a Plan Task or Work List Item starts or
completes.

Validations are stored procedures or views that have been written and
saved in a data source that is registered in the DSP®. A validation
executes when an event occurs and confirms that a process is valid. If
the validation fails, processing stops. For example, a validation is
registered to a Receive Email event. The validation confirms that an
email received at a designated address has an attachment in a specified
format. If the attachment is in a valid format, the validation passes
and processing can continue. However, if the attachment is in an invalid
format, the validation fails, and processing stops.

If a validation fails:

  - dspTrack™ displays an error message.
    
    **NOTE:** That message was entered in the Validation Message field
    when the validation was added.

  - The event the validation was registered to does not run.

The validation is triggered when a user clicks the Next Action button on
the Work List to indicate that work on the Plan Task or Work List Item
has started or finished.

**NOTE**: Before registering the validation, it must be written and
stored in a data source that is registered in Common. Refer to [Register
a Data Source in
Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common.htm) for
more information. The validation can only use parameters that can be
passed in from the Work List. Refer to [Parameters for Work List Event
Validation](../Page_Desc/Parameters_for_Work_List_Event_Validations.htm)
for more information.
