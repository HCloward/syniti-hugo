+++
title = 'Logging Modules'
solution = 'Platform'
+++

# Logging Modules

<div class="use">

Use this page to [Add Logging
Modules](../Use_Cases/Add_Logging_Modules).

</div>

To access this page:

1.  Select **Configuration \> Parameters** in the *Navigation* pane.
2.  Click the **Modules** icon.

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>MODULE</p></td>
<td><p>Displays the name of the logging module, which is a category of logs that displays information based on what types of errors are logged.</p></td>
</tr>
<tr class="odd">
<td><p>SEVERITY</p></td>
<td><p>Displays the severity level assigned to the task. Options are:</p>
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
<tr class="even">
<td><p>LOG TASKS</p></td>
<td><p>If checked, task for the module are recorded on the <em><a href="Log">Log</a></em> page.</p>
<p>If unchecked, tasks for the module are not recorded on the <em><a href="Log">Log</a></em> page.</p>
<p>It is checked by default.</p></td>
</tr>
</tbody>
</table>
