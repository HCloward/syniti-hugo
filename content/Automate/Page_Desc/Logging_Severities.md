+++
title = ''
solution = 'Platform'
+++

# <span id="LoggingSeveritiesH"></span> Logging Severities H

[Logging Severities V](#LoggingSeveritiesV)

<div class="use">

Use this page to [Configure Logging
Severities](../Use_Cases/Configure_Logging_Severities.htm).

</div>

To access this page, select **Configuration \> Logging \> Severities**
in the *Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays a number to indicate the logging severity.</p></td>
</tr>
<tr class="odd">
<td><p>IMAGE</p></td>
<td><p>Displays an image to indicate the type of logging severity. This image corresponds to the Image Name field on the <em><a href="#LoggingSeveritiesV">Vertical</a></em> View.</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the name of the logging severity.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of what the logging severity indicates and examples of when it might apply. Options are:</p>
<ul>
<li><strong>10 – Debug –</strong> Variables</li>
<li><strong>20 – Trace –</strong> Program executions</li>
<li><strong>30 – SQL –</strong> SQL statements and results</li>
<li><strong>40 – Info –</strong> Production optionally, course grained (rarely written information), used to print that a configuration is initialized or that a long running import job is starting and ending.</li>
<li><strong>50 – Notice –</strong> Production, notice information</li>
<li><strong>60 – Warning –</strong> Production, simple application error or unexpected behavior, but the application can continue, e.g., a bad login attempt or unexpected data import during jobs.</li>
<li><strong>70 – Error –</strong> Production, application error/exception, but the application can continue. Part of the application is not working properly.</li>
<li><strong>80 – Fatal –</strong> Production, fatal application error, application cannot continue, e.g., the database is down.</li>
</ul></td>
</tr>
</tbody>
</table>

# <span id="LoggingSeveritiesV"></span> Logging Severities V

[Logging Severities H](#LoggingSeveritiesH)

**Field**

**Description**

Priority

Displays a number to indicate the logging severity.

Name

Displays the name of the logging severity.

Description

Displays a description of what the logging severity indicates and
examples of when it might apply.

Image Info

Image

Displays the image that corresponds with the Image Name.

Image Name

Displays the name of the image.

Formatting Info

Html Pre Tag

Displays an HTML preformat text applied to the log message in the
Automate *[Log](Log.htm)* page.

Html Post Tag

Displays an HTML postformat text applied to the log message in the
Automate *[Log](Log.htm)* page.
