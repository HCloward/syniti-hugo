+++
title = 'Source (Info) H'
solution = 'Migration'
+++

# Source (Info) H

[Source (Info) V](#Source__Info__V)

This report lists all Target Source reports for all contexts that are
info reports. All report types that are not error report types (Error
and Target Readiness) display on this report page. The record count, the
date the report last ran, and icons to view and download the report are
also included

**NOTE:** When a user accesses the Source (Info) report in the
*Navigation* pane, the fields below display. When a user clicks View on
the *Source (Info)* page to view report data, the report title still
reads Source (Info) even though the columns that display depend on the
columns on the generated report. In this case, the *Source (Info)* page
displays the report’s columns only and not the fields below.

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Select **Reports \> Source (Info)** in the *Navigation* pane.

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
<td><p>SOURCE REPORT</p></td>
<td><p>Displays the name of the Target Source report that has a report type of Info. The report is a view created in SQL. The report type is set on the <em><a href="Target_Source_Reports_H.htm">Target Source Reports</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the report’s description as entered on the <em>Target Source Reports</em> page.</p></td>
</tr>
<tr class="even">
<td><p>REPORT TYPE</p></td>
<td><p>Displays the report type. All report  types except error report types (Error and Target Readiness) display on this report.</p>
<ul>
<li><strong>Business Readiness —</strong> Checks data against a smaller set than Target Readiness reports.  For example, though a check table may have values A-Z, a customer may only want to use a subset of the check tables, such as A-B.</li>
<li><strong>Business Relevancy —</strong> Defines rules/conditions that require the data to have relevancy to the project. The client defines rules to check data and decides if it is relevant and should therefore be included in the migration.</li>
<li><strong>Info —</strong> Identifies reports with data that is used for informational purposes only and that does not require further action.</li>
<li><span style="font-weight: bold;">Pre-Load — </span> Identifies reports used only for the Pre-Load phase of the project.</li>
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

## <span id="Source__Info__V"></span>Source (Info) V

[Source (Info)
H](#Source__Info__H)

|               |                                                                                                                                                                                |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field         | Description                                                                                                                                                                    |
| Target ID     | Displays the target table name where the data is being migrated to.                                                                                                            |
| Source ID     | Displays the name of the database where the source table is stored.                                                                                                            |
| Source Report | Displays the name of the Target Source report that has a report type of Info. The report is a view created in SQL. The report type is set on the *Target Source Reports* page. |
| Comment       | Displays a comment entered about the report on the *[Target Reports](Target_Reports_H.htm)* page’s *Vertical* View on the Documentation tab.                                   |
