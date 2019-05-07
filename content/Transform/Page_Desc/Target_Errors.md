+++
title = ''
solution = 'Migration'
+++

# <span id="Target_Errors_H"></span>Target (Errors) H

[Target (Errors) V](#Target__Errors__V)

This report lists all Target reports for all contexts that are error
reports. Report types of Error and Target Readiness display on this
report page. The record count, the last date the report ran, and icons
to view and download the report are also included.

**NOTE:** When a user accesses the Target (Errors) report in the
Navigation pane, the fields below display. When a user clicks View on
the *Target (Errors)* page to view report data, the report title still
reads Target (Errors) even though the columns that display depend on the
columns on the generated report. In this case, the *Target (Errors)*
page displays the report’s columns only and not the fields below.

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Select **Reports \> Target (Errors)** in the *Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Process Area</p></td>
<td><p>Displays the name of the Process Area to which the data on the report belongs.</p>
<p>Process Areas are created in Console and, along with a Wave, create a context.</p></td>
</tr>
<tr class="odd">
<td><p>OBJECT NAME</p></td>
<td><p>Displays the name of the object to which the data on the report belongs.</p>
<p>Objects are created in Console and are assigned to a Wave and Process Area, also known as a context.</p></td>
</tr>
<tr class="even">
<td><p>TARGET ID</p></td>
<td><p>Displays the name of the target on which the report is based.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET REPORT</p></td>
<td><p>Displays the name of the target report that has a report type of Error. The report is a view created in SQL. The report type is set on the <em><a href="Target_Reports_H.htm">Target Reports</a></em> page.</p></td>
</tr>
<tr class="even">
<td><p>REPORT TYPE</p></td>
<td><p>Displays the report type. The report types Error and Target Readiness display on this report.</p>
<ul>
<li><strong>Error</strong> – Displays data that must be fixed before loaded.</li>
<li><strong>Target Readiness</strong> – Checks against a valid configuration or check tables and looks for matches between the data and the check table data. For example, if a customer-defined credit limit with ten valid limits in SAP, the report compares/checks data in Transform against the check tables.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records on the report.</p></td>
</tr>
<tr class="even">
<td><p>ACTION ON</p></td>
<td><p>Displays the date when the report last ran.</p></td>
</tr>
<tr class="odd">
<td><p>View</p></td>
<td><p>Click to view the report data.</p></td>
</tr>
<tr class="even">
<td><p>DOWNLOAD</p></td>
<td><p>Click to download the report in Excel 2007-2012 (.xlsx) format.</p></td>
</tr>
</tbody>
</table>

## <span id="Target__Errors__V"></span>Target (Errors) V

[Target (Errors)
H](#Target_Errors_H)

|               |                                                                                                                                                                   |
| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field         | Description                                                                                                                                                       |
| Target ID     | Displays the name of the target on which the report is based.                                                                                                     |
| Target Report | Displays the name of the target report that has a report type of Error. The report is a view created in SQL. The report type is set on the *Target Reports* page. |
| Comment       | Displays text a user entered in the Comments field on the *Target Reports* page’s *Vertical* View on the Documentation tab.                                       |
