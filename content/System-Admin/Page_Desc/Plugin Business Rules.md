+++
title = 'Plugin Business Rules'
solution = 'Platform'
+++

# Plugin Business Rules

<div class="use">

Use this page to:

  - [Register the Plugin as an External
    Page](../Use_Cases/Register%20Plugin%20in%20DSP.htm#RegisterPluginasanExternalPage)
  - [View where Plugin is used within the
    DSP](../Use_Cases/View%20Where%20Plugin%20is%20Used.htm)

</div>

To access this page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.
2.  Click the **Plugins** icon for the desired WEB APP NAME.
3.  Click the **Plugins** icon for the desired ASSEMBLY PATH.
4.  Click the **Business Rules** icon for the desired PLUGIN NAME.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>WEB APP NAME</p></td>
<td><p>Displays the name of the WebApp where the business rule resides.</p></td>
</tr>
<tr class="odd">
<td><p>PAGE NAME</p></td>
<td><p>Displays the page name within the WebApp where the business rule runs.</p></td>
</tr>
<tr class="even">
<td><p>EVENT NAME</p></td>
<td><p>Displays the event that runs on the page.</p></td>
</tr>
<tr class="odd">
<td><p>EVENT DESCRIPTION</p></td>
<td><p>Displays a brief description of the event.</p></td>
</tr>
<tr class="even">
<td><p>RUN ON VALIDATE</p></td>
<td><p>If checked, the business rule runs when the event is validated.</p>
<p>If unchecked, the business rule does not run when the event is validated.</p></td>
</tr>
<tr class="odd">
<td><p>RUN ON VALIDATE FAIL</p></td>
<td><p>If checked, the business rule runs even when the event fails.</p>
<p>If unchecked, the business rule does not run when the event fails.</p></td>
</tr>
<tr class="even">
<td><p>FORCE FOREGROUND EXECUTION</p></td>
<td><p>If checked and if the validation rule is set to run in the background, it will execute twice: once in the foreground and later in the background.</p>
<p>The intent of this feature is to ensure that the Business rule runs against the Web Server, even if the event is set to run in the background. For example, Force Foreground Execution may be required for plugin access to the Http Context.</p></td>
</tr>
<tr class="odd">
<td><p>IS ACTIVE</p></td>
<td><p>If checked, the business rule runs for the event.</p>
<p>If unchecked, the business rule does not run for the event.</p></td>
</tr>
</tbody>
</table>
