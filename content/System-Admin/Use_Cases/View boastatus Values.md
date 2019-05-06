# View boaStatus Values

The DSP® uses the boaStatus column to display information about a
record, such as:

  - Whether a record passed or failed validations

  - If a record is new

  - If a record is valid

  - The record's Control Status
    
    **NOTE:** A user can set which boaStatuses return 0 (disabled) and
    which return 1 (enabled), setting whether a column or control is
    hidden, active, or dimmed. Refer to [Set Column Control
    Status](../../WebApp_Dev/Set_Column_Control_Status.htm) for more
    information.

  - Whether processing for a record completed, is currently running, or
    failed

For example, business rules that take a long time to run can be forced
to run in the background. Background events are placed into a job queue
for later execution. The boaStatus is Queued when the rule is first
submitted. When the event is running, the boaStatus becomes Processing.
It then becomes Processing Failed or Procedures Complete.

An Administrator can also add and configure custom statuses as needed,
using Custom Status. Settings for delivered boaStatus values should not
be updated.

To access the *[Status](../Page_Desc/Status.htm)* page to view boaStatus
values, click **Admin \> Configuration \> Setup \> Status** in the
*Navigation* pane.

Each boaStaus is configured to:

  - Allow for deletion or update
  - Be considered valid
  - Auto refresh upon record update

**NOTE:** An OnValidate event must be added for every page that contains
a boaStatus field, even if there are no validation rules or business
rules registered to the page. If the OnValidate event is not created,
boaStatus is not automatically updated by DSP®.

**NOTE:** The boaStatus field can be automatically added to tables.
Refer to [Append BOA Reserved Columns to
Tables](../../WebApp_Dev/Append_BOA_Reserved_Columns_to_Tables.htm) for
more information.
