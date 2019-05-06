# Process Templates: After Post Rules H

[Process Templates: After Post Rules V](#Process)

<div class="use">

Use this page to [Register After Post Rules to a Process
Template](../../../Platform/Integrate/Use_Cases/Register_After_Post_Rules_to_a_Process_Template_Overview.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Integrate \>
    </span>**Categories** from *Navigation pane*.
2.  Click the **Processes** icon for a category.
3.  Click the **Templates** icon for a process.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the After Post Rule runs for this process template if multiple rules are assigned. Rules process in ascending order.</p></td>
</tr>
<tr class="odd">
<td><p>RULE</p></td>
<td><p>Displays the rule name.</p>
<p>An After Post Rule is used in a multi-template process and can be a stored procedure, Collect Download, or Status View. The rules run after the process template is finished executing and before the next one begins.</p></td>
</tr>
<tr class="even">
<td><p>COMMENT</p></td>
<td><p>Displays user-entered text, which could include a description of the after post rule’s function</p></td>
</tr>
</tbody>
</table>

## <span id="Process"></span>Process Templates After Post Rules V

[Process Templates: After Post Rules
H](../../../Platform/Integrate/Page_Desc/Process_Template_Loop_Field_Mappings_H.htm)

<div class="use">

Use this page to [Register After Post Rules to a Process
Template](../../../Platform/Integrate/Use_Cases/Register_After_Post_Rules_to_a_Process_Template_Overview.htm).

</div>

Field

Description

Basic

Priority

Displays the order the After Post Rule runs for this process template if
multiple rules are assigned. Rules process in ascending order.

Comment

Displays user-entered text, which could include a description of the
after post rule’s function

Business Rule

After Post Rule Data Source ID

Displays the data source that stores the stored procedure.

After Post Rule

Displays the Business Rule name.

Rules pull data down to refresh local data after it has been changed or
to manipulate the local data to prepare for the next template. This
stored procedure runs after the process template is finished executing
and before the next one begins.

When a Business Rule After Post Rule is encountered, Integrate runs the
rule and waits for it to complete before running the next rule.

Refer to [Register a Stored Procedure as an After Post
Rule](../../../Platform/Integrate/Use_Cases/Register_a_Stored_Procedure_as_an_After_Post_Rule.htm)
for more information.

Collect

Collect Source

Displays the source to use for the Collect Download.

**NOTE:** The source is required when registering a Collect Download.

Collect Target

Displays the target to use for the Collect Download.

**NOTE:** The target is required when registering a Collect download.

Collect Table Name

Displays the name of the table to download.

**NOTE:** The table name is required when registering a Collect
Download.

Collect Target Where Clause

Displays the rule to run on target data after the table downloads.

The data returned from this Where clause is used as an input parameter
to the next template in the process.

The target Where clause selects records to delete from the target before
the download.

Refer to [Register a Collect Download After Post Rule
Manually](../../../Platform/Integrate/Use_Cases/Register_a_Collect_Download_After_Post_Rule_Manually.htm)
  for more information.

Collect Source Where Clause

Displays the rule to run on source data after the table downloads. The
source Where clause selects records to download from the source to the
target.

The data returned from this Where clause is used as an input parameter
to the next template in the process.

Refer to [Register a Collect Download After Post Rule
Manually](../../../Platform/Integrate/Use_Cases/Register_a_Collect_Download_After_Post_Rule_Manually.htm)
for more information.

Collect Where Clause

Click to open the [Process Template: After Post Rule: Collect
Where](../../../Platform/Integrate/Page_Desc/Process_Template_After_Post_Rule_Collect_Where.htm)
page to add the inputs to a Where clause that is built automatically at
run time.

Refer to [Register a Collect Download After Post Rule that is Built
Automatically](../../../Platform/Integrate/Use_Cases/Register_a_Collect_Download_After_Post_Rule_that_is_Built_Automatically.htm)
for more information.

Collect Run Rules After Download

If enabled, the rules run on the Collect table after it has downloaded.
If disabled, the rules do not run.

Status

Status View Data Source ID

Displays the data source that stores the Status View.

Status View

Displays the name of the Status View used to communicate a status of the
posting to the user. The view status is "pass" when there are no records
in the view for the PostingID. The view status is "fail" if the view
contains at least one record of data for the PostingID. If a status of
failure is found then that status is written as the status for the
posting of that template.

Refer to [Register a Status View as an After Post
Rule](../../../Platform/Integrate/Use_Cases/Register_a_Status_View_as_an_After_Post_Rule.htm)
for more information.
