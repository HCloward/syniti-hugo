# View Bulk Execution Results

For general information about Bulk Execution, refer to [Use Bulk
Execution](Use_Bulk_Execution).

The Results tab includes the record metrics in the top right of the tab.

The Record Metrics display:

  - **Failed**—The total number of records that failed all validations
    and business rules, if applicable, during Bulk Execution.
  - **Passed**—The total number of records that passed all validations
    and business rules, if applicable, during Bulk Execution.
  - **Unknown**—The total number of records that failed validations for
    which the user set the action to “No Action”.

The Error, Warning and Message results display separately with their
respective validation messages and the number of records in that record
set.

Failed records include:

  - Any records that fail a business rule
  - Any records that fail a validation rule that has a type of Error
  - Any records that fail a validation rule that has a type of Warning
    with the Fail Action on Warning set

**NOTE:** If a record is affected by more than one validation rule and
it fails any of them, the status is set to failed.

Passed records include:

  - Any records that fail a validation that has a type of Message
  - Any records that fail a validation that has a type of Warning with
    the Pass Action on Warning set

Unknown records include any records that fail a validation that has a
type of Warning with the No Actions Action on Warning set.

If a record is read-only, the record is not included in the Bulk
Execution process. When Bulk Execution completes, read-only records
display on the Results tab under the label Record was skipped during
execution.

Click the **Expand All** and **Collapse All** buttons to show and hide
all results.

Each validation has a Filter and a Status icon.

The Filter icon allows the user to filter the record set on records that
have failed that validation. When the user clicks the Filter icon, the
corresponding record set displays on the DSP page. To concatenate filter
results, Ctrl+click multiple Filter icons.

When the user clicks the Key icon, the Key column for that record, which
is sometimes hidden on the DSP page, displays at the bottom of the Bulk
Execution panel.

Corrections to warnings and errors can be made while the Bulk Execution
panel is open. After updates have been made to any failed records, the
Bulk Execution process must be rerun to get the new results. The records
can be validated again in the Bulk Execution panel without closing and
reopening it.
