+++
title = 'Execute a Boomi Process From a Custom Page'
solution = 'Platform'
+++

# Execute a Boomi Process From a Custom Page

Using a public plugin, a WebApp Developer can execute Processes created
in Boomi. This allows integration with a wide variety of external
systems, as defined by Connectors.

Boomi Processes can be used, for example, to validate, import, and
export data or to execute automation tasks, but are not limited to these
actions.

Before performing these steps:

  - The Boomi Process can exist in Boomi. If data is returned after the
    Process executes, the Boomi Process must be included in the BOA
    Boomi Process template. If data is not returned, use any non-BOA
    Boomi Process template.
  - The IG Universal Connect data source, which includes the Boomi Atom
    ID, must be registered in the Data Source Registry in Common.
  - The WebApp Developer must understand how to create a view in SQL,
    how to design pages in the platform, and, depending on the Process,
    how to write Validation and Business rules.

To execute a Boomi Process from a custom page:

1.  Create a page view (*Horizontal* or *Vertical*) with an event. The
    view must have these columns with these exact names:
    
      - **BoomiDataSourceId** — The GUID that is the unique identifier
        that represents an IG Universal Connect (Boomi) Data Source.
        This value is populated from the DataSourceId field from
        ttDataSourceRegistry table and exists after the IG Universal
        Connect data source is registered in Common.
    
      - **BoomiProcessId** — The GUID that is the unique identifier that
        represents the Boomi Process to execute. This GUID can be found
        in the Boomi AtomSphere. Select the Process in the IG Universal
        Connect Template, and click Revision History. The GUID displays
        in the Component ID field.

The following columns are optional in the view.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>BoomiAtomId </p></td>
<td><p>The GUID that is the unique identifier that represents the Atom ID to be used when executing the Process. This field overrides the atom registered at the IG Universal Connect Data Source level. If this field is NULL or not included in the view, the Process executes against the default atom.</p></td>
</tr>
<tr class="odd">
<td><p>Synchronous </p></td>
<td><p>The bit field that sets whether the process runs synchronously or asynchronously.</p>
<p>When using the default setting of 1, or synchronous, the plugin waits until the Process is completed and a status is returned before proceeding. When using the synchronous method, which is recommended, the IG Universal Connect process template is required. This method is set by default.</p>
<p>When set to false (asynchronous), the plugin executes the process and does not retrieve the status.</p></td>
</tr>
<tr class="even">
<td><p>ExcludedColumns</p></td>
<td><p>This field with a data type of nvarchar is used to specify data row columns to exclude as parameters. Sensitive data or large data fields should be excluded if they are not required for the Process. Specify the column names to exclude from passing into the Process in a comma delimited list (for example, ColumnName1, ColumnName2, ColumnName3). Fields in the data row contract (the fields in this table) are automatically excluded.</p></td>
</tr>
<tr class="odd">
<td><p>MessageOption </p></td>
<td><p>This field with a data type of string, nvarchar specifies when to display status messages to the user. Options are:</p>
<ul>
<li><strong>Always</strong> — Always return a message after execution. </li>
<li><strong>Never</strong> — Never return a message after execution. </li>
<li><strong>OnlyOnError</strong> — Only return a message if the Boomi execution failed or an exception is thrown. This is the default value.</li>
</ul>
<p><strong>NOTE</strong>: Status messages display if the plugin is registered to an event that runs in the foreground. They do not display for background events.</p></td>
</tr>
</tbody>
</table>

 

2.  Register the  
    DSP.DataSourceOperations.BoomiProcessExecutionPlugin public plugin
    as an event to the custom page.

The next steps to take depend on what action the Process performs:

  - If the Process sends data to an external system, this task is
    complete.
  - If the Process validates data, create Validation rules based on the
    data returned after successful execution.
  - If the Process imports data, create Business rules to update page
    data based on the data returned after successful execution.

**NOTE**: Whether status messages display and Business rules continue to
run when a Process fails to execute successfully depends on whether the
plugin is registered to a foreground or background event. If the plugin
is registered to a foreground event, the status message displays to the
user. However, no exceptions will be thrown and business rules will
continue to run even if a Process fails to execute. If the plugin is
registered to a background event, status messages do not display but an
exception will be thrown when the Process fails to execute or the
process results in an exception. In this case, business rules stop
running. Configure whether an event runs in the foreground or background
using the Event Process Type ID list box on the *[Page
Events](../Sys_Admin/Page_Desc/Page_Events_H.htm)* page.

To troubleshoot or monitor process execution, view the logs stored in
the DSPCommon ttDebugLog table.
