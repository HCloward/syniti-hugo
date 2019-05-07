+++
title = ''
solution = 'Migration'
+++

# <span id="Target_Info_H"></span>Target (Info) H

[Target (Info) V](#Target__Info__V)

This report lists all Target reports for all contexts that are info
reports. All report types that are not error report types (Error and
Target Readiness) display on this report page. The record count, the
last date the report ran, and icons to view and download the report are
also included.

**NOTE:** When a user accesses the Target (Info) report in the
<span style="font-style: italic;">Navigation</span> pane, the fields
below display. When a user clicks View on the *Target (Info)* page to
view report data, the report title still reads Target (Info) even though
the columns that display depend on the columns on the generated report.
In this case, the *Target (Info)* page displays the report’s columns
only and not the fields below.

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Select **Reports \> Target (Info)** in the *Navigation* pane.

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
<td><p>Displays the name of the target report that has a report type of Info. The report is a view created in SQL. The report type is set on the <em><a href="Target_Reports_H.htm">Target Reports</a></em> page.</p></td>
</tr>
<tr class="even">
<td><p>REPORT TYPE</p></td>
<td><p>Displays the report type. All report  types except error report types (Error and Target Readiness) display on this report:</p>
<ul>
<li><strong>Business Readiness</strong> – Checks data against a smaller set than Target Readiness reports. For example, though a check table may have values A-Z, a customer may only want to use a subset of the check tables, such as A-B.</li>
<li><strong>Business Relevancy</strong> – Defines rules/conditions that require the data to have relevancy to the project. The client defines rules to check data and decides if it is relevant and should therefore be included in the migration.</li>
<li><strong>Info</strong> – Identifies reports with data that is used for informational purposes only and that does not require further action.</li>
<li><span style="font-weight: bold;">Pre-Load</span> – Identifies reports used only for the Pre-Load phase of the project.</li>
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

## <span id="Target__Info__V"></span>Target (Info) V

[Target (Info)
H](#Target_Info_H)

|               |                                                                                                                                                                  |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field         | Description                                                                                                                                                      |
| TARGET ID     | Displays the name of the target on which the report is based.                                                                                                    |
| TARGET REPORT | Displays the name of the target report that has a report type of Info. The report is a view created in SQL. The report type is set on the *Target Reports* page. |
| COMMENT       | Displays text a user entered in the Comments field on the *Target Reports* page’s *Vertical* View on the Documentation tab.                                      |
