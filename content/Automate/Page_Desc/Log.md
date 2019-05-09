+++
title = 'Log H'
solution = 'Platform'
+++

# Log H

[Log V](#_Log_V)

<div class="use">

Use this page to [View Logs for an
Interface](../Use_Cases/View_Logs_for_an_Interface).

</div>

To access this page:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click the **History** icon for the desired interface.

3.  Click the **Important** icon to view the *Log* page filtered by
    tasks with a level set at Reporting by Importance Level or above.
    This icon is only enabled of there are tasks written to the log for
    the interface according to the level set in the Reporting by
    Importance Level field on the *[Parameters](Parameters)* page.
    
    Or

4.  Click the **All** icon to view the *Log* page and all tasks for the
    interface. 

 

|              |                                                                                                                                                        |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Field**    | **Description**                                                                                                                                        |
| **SEVERITY** | Displays an icon indicating the severity. Refer to [Configure Logging Severities](../Use_Cases/Configure_Logging_Severities) for more information. |
| MODULE       | Displays the name of the module, which is a category of logs that displays information based on what types of errors are logged.                       |
| MESSAGE      | Displays a message that corresponds to the Severity . For example, with a Severity of SQL, the SQL code used to execute the task displays.             |
| DURATION     | Displays the time it took for the task to finish running.                                                                                              |

 

# <span id="_Log_V"></span> Log V

[Log H](#LogH)

 

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Severity</strong></p></td>
<td><p>Displays an icon indicating the severity. Options are:</p>
<ul>
<li><strong>80 – Fatal –</strong> Production, fatal application error, application cannot continue, e.g., the database is down.</li>
<li><strong>70 – Error –</strong> Production, application error/exception, but the application can continue. Part of the application is not working properly.</li>
<li><strong>60 – Warning –</strong> Production, simple application error or unexpected behavior, but the application can continue, e.g., a bad login attempt or unexpected data import during jobs.</li>
<li><strong>50 – Notice –</strong> Production, notice information</li>
<li><strong>40 – Info –</strong> Production optionally, course grained (rarely written information), used to print that a configuration is initialized or that a long running import job is starting and ending.</li>
<li><strong>30 – SQL –</strong> SQL statements and results</li>
<li><strong>20 – Trace –</strong> Program executions</li>
<li><strong>10 – Debug –</strong> Variables</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Date Time</p></td>
<td><p>Displays the date and time when the task finished running.</p></td>
</tr>
<tr class="even">
<td><p>Duration</p></td>
<td><p>Displays the time it took for the task to finish running.</p></td>
</tr>
<tr class="odd">
<td><p>SQL Statement</p></td>
<td><p>Displays the SQL code used to execute the task.</p>
<p><strong>NOTE:</strong> This field only displays for tasks with SQL severities.</p></td>
</tr>
<tr class="even">
<td><p>SQL Results</p></td>
<td><p>Displays the results of the SQL Statement that ran.</p>
<p><strong>NOTE:</strong> This field only displays for tasks with SQL severities.</p></td>
</tr>
<tr class="odd">
<td><p>Rows</p></td>
<td><p>Displays the number of rows of data being passed. For tasks with a severity of SQL, this field displays the number of updated rows.</p>
<p><strong>NOTE:</strong> This field only displays for tasks with SQL and Debug severities.</p></td>
</tr>
<tr class="even">
<td><p>Parameters</p></td>
<td><p>Displays information passed to the module.</p>
<p><strong>NOTE:</strong> This field only displays for tasks with Debug severities.</p></td>
</tr>
<tr class="odd">
<td><p>Message</p></td>
<td><p>Displays a message that corresponds to the Severity .</p>
<p><strong>NOTE:</strong> This field only displays for tasks with Debug, Trace, Info, Notice, Warning , Error and Fatal severities.</p></td>
</tr>
<tr class="even">
<td><p>Stack Trace</p></td>
<td><p>Displays technical details of the error message mused by developers to determine where the issue occured.</p>
<p><strong>NOTE:</strong> This field only displays for tasks with Error and Fatal severities.</p></td>
</tr>
</tbody>
</table>
