# Perform Bulk Execution

For general information about Bulk Execution, refer to [Use Bulk
Execution](Use_Bulk_Execution).

Bulk Execution runs against the context of the page at the time the
panel was opened. If the user filters the records after the panel is
opened, it will still run on the original data set.

By default, the number of records that can have Bulk Execution performed
at one time is 100K. Refer to [Set Bulk Execution
Parameters](../Sys_Admin/Use_Cases/Set_Bulk_Execution_Parameters)
for more information. When no filter is applied, all records on the page
are validated.

The Bulk Execution panel contains several context related items to
ensure that the user understands the context in which Bulk Execution
will be performed. The Bulk Execution panel displays the following
information, where relevant:

<table>
<tbody>
<tr class="odd">
<td><p>Icon/Information</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Row Count</p></td>
<td><p>The record count reflects the context of the page when it was opened and isn’t a guaranteed count for processing. The number of rows is displayed in the upper right area of the panel.</p></td>
</tr>
<tr class="odd">
<td><p>Filter button</p></td>
<td><p>If the record set is filtered, a filter button displays. Hover over the filter button to display the name of the column on which the records are filtered.</p></td>
</tr>
<tr class="even">
<td><p>Drill Down</p>
<p> </p></td>
<td><p>This icon indicates what value the page is “drilled” or “bound” on when the user hovers over it. If the page where the user opens the Bulk Execution panel does not have “Drill” or “Binding” criteria, the icon does not display.</p></td>
</tr>
</tbody>
</table>

To perform Bulk Execution:

1.  Select **Bulk Execution** from the page gear menu.
    
    **NOTE:** The **Bulk Execution Limit** parameter is checked against
    the number of records in the current filtered record set. If the
    current number of records exceeds the Bulk Execution Limit parameter
    setting, a notification displays and the Bulk Execution process is
    not launched.
    
    **NOTE:** The **Event** field displays the only event used by Bulk
    Execution, the Validate event.

2.  Click the **Exclude Business Rules** check box, if needed.
    
    **NOTE:** If checked, the OnValidate event runs without running any
    business rules registered to the page event. If unchecked, both the
    Validation and Business rules run. In most cases, the user does not
    need to change this setting unless instructed to do so by the Page
    Designer of the custom application.
    
    **NOTE:** The Page Designer can enable the check box by default
    and/or disable the user's ability to update it.  Refer to [Configure
    Business Rule
    Settings](../Sys_Admin/Use_Cases/Configure_Business_Rule_Settings)
    in System Administration for more information.

3.  Click **Next**; or click the **Action on Warnings** tab.
    
    **NOTE:** Page Validations of type warning display on the Action on
    Warnings tab. If no validations of type warning are registered to
    the OnValidate event for the page, tthe Action on Warning tab is
    disabled and a Start button displays.
    
    **NOTE:** On the Action on Warnings tab, the user can choose which
    action to take on a record that fails for the warning validations.

4.  Select an option for an individual warning listed on the tab. The
    user can choose to **Update All**.
    
    **NOTE:** When an option is chosen from the **Update All** field,
    the options for each validation warning are set to that value.
    
    Options include:
    
      - **Pass**—Any records that fail the validation are passed as
        valid during the Bulk Execution process.
      - **Fail**—Any records that fail the validation are failed during
        the Bulk Execution process.
      - **No Action**—Any record that fails the validation is given a
        validation status of Unknown on the Results tab.

5.  Click **Start**.
    
    **NOTE:** If an error occurs as a result of running a business rule
    execution against the event, the result is an error status.
    
    **NOTE:** The same record can exist in multiple results. If a record
    is contained in multiple warning sets, fail takes precedence over
    pass, meaning, if a record is contained in a warning that is set to
    Pass and is contained in another warning set to Fail, the record is
    marked as Failed during processing.
    
    Continue with [View Bulk Execution
    Results](View_Bulk_Execution_Results).
