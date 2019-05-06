# Perform Bulk Execution via a Public WebApp Event

Bulk Execution can be invoked via a Public WebApp Event on a custom
designed page, which allows a developer to provide a mechanism of
implicit validation. A user will not have to access each page
individually and use the Bulk Execution panel. The Public WebApp event
can also allow non-direct access users to invoke Bulk Execution via the
Services user (Background Service).

**NOTE**: If the Public WebApp Event is foreground, the current user is
utilized. This is important to note as users may not have access to the
page specified.

Bulk Execution is executed on the targeted page with the associated
event with environment criteria as defined by the optional parameters.

Results are stored in a result table within the framework’s database to
be accessed by the calling application. The results themselves are not
accessible via boa\* views as this is a not a definitive access method
and may be changed in the future.

**NOTE**: The page-level OnValidate event must have been written before
Bulk Execution can be configured for it.

This topic contains the following sections:

  - [Set Up the Event](#Set_Up_the_Event)
  - [Add a Parameter View](#Add_a_Parameter_View)
  - [Access Results](#Access_Results)

## <span id="Set_Up_the_Event"></span>Set Up the Event

To set up the Public WebApp Event:

1.  Navigate to the page where the Public WebApp Event is to be used.
2.  Click **Design Page \> Design**.
3.  Select a page and click the **Events** icon.
4.  Select the event to which the Public WebApp Event will be added.
5.  Click the **Business Rules i**con.
6.  Add a new business rule where the **PROCEDURE TYPE** is
    **WebAppEvent**.
7.  Choose **System Administration: Bulk Execution** as the
    **EventPageID**.
8.  Choose **Invoke** as the **Event Name**.

## <span id="Add_a_Parameter_View"></span>Add a Parameter View

Configure the usage of a Public WebApp Event by creating a parameter
view and defining each field for each parameter as needed.

This plugin executes Bulk Execution based on the criteria provided.

Parameters:

  - **Event \[Key\]** - Name of the event to be Bulk Executed. This
    event must have Support Bulk Execution checked.
  - **PageID \[Key\]** - Page which hosts the event that will be bulk
    executed.
  - **BindingCriteria** \[Optional\] - Binding criteria which should be
    included in the context of the Bulk Execution. This is bound against
    the source record.
  - **ExcludeBusinessRules** \[Optional\] - Whether business rules
    should be considered when executing the Page Event.
  - **SharedCriteria** \[Optional\] - Shared criteria which should be
    included in the context of the Bulk Execution. This is bound against
    the source record.

## <span id="Access_Results"></span>Access Results

Results generated during an event that includes the invocation of the
Bulk Execution: Invoke Public WebApp Event are stored in both the
BulkExecutionResult and BulkExecutionValidationRuleResult tables within
the framework database. The results from the bulk execution that are
stored in the table are kept for a few hours. As a best practice, the
records from those tables should be copied to a data store in the custom
application to work with and reference.

BulkExecutionResult stores the event parameters as well as the metrics
about the execution. This includes time to complete
\[ExecutionTimeSeconds\], \[RecordsFailed\], \[RecordsSkipped\],
\[RecordsUnknown\], \[RecordsPassedWithMessage\],
\[RecordsPassedWithNoMessage\], and \[RecordsThrewErrors\].

BulkExecutionValidationRuleResult stores the validations associated with
the Bulk Execution event. This includes \[ForcedFail\], \[ForcedPass\],
and \[Count\].

These resultant records are identified by a BulkExecutionResults ID. The
calling event is informed of the relevant ID via a callback mechanism
implemented with this feature. Any subsequent event rules run after the
Bulk Execution Invoke Public WebApp Event are given the
BulkExecutionResults ID if the reserved parameters @
boaActionResultsIdentifier is included in the parameter view.

BulkExecutionResults ID is also available from within plugins under the
host object accessible via Host.ActionResultsIdentifier. When available,
the values reflect that of the previous invocation of “Bulk Execution :
Invoke.” The ID can then be used to access the data to copy it where
needed, as these result are not guaranteed to last indefinitely.
