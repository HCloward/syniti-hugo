+++
title = 'Page Event Rule Parameters'
solution = 'Platform'
+++

# Page Event Rule Parameters

<div class="use">

Use this page to [Set a Parameter Value for Business Rule Parameters for
a Public WebApp
Event](../../WebApp_Dev/SetParameterValueBusinessRules.htm).

</div>

To access this page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.
2.  Click the **Pages** icon for a **WEB APP NAME**.
3.  Click the **Events** icon for a page.
4.  Click the **Business Rules** icon for an event.
5.  Click **Vertical View** for a Business Rule with a procedure type of
    WebApp Event.
6.  Click the **Parameters** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays a number indicating the order the Business Rules display.</p></td>
</tr>
<tr class="odd">
<td><p>PARAMETER NAME</p></td>
<td><p>Displays the name of the parameter passed by a WebApp to run this Public event. The key fields on the table upon which the page is based on are included by default.</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the name of the name of the validation which is computed based on the type of the validation and the entity chosen (whether it’s a view, procedure, or plugin), for example, webdcsMARA_FullConstruct_DSP9587DupKeyVal.</p></td>
</tr>
<tr class="odd">
<td><p>PARAMETER TYPE</p></td>
<td><p>Displays whether the parameter is a key field on the table and must be passed or is optional. This value is set on the <em><a href="Page_Event_Param_H.htm">Page Event Parameters</a></em> page.</p>
<p>Values are:</p>
<ul>
<li><strong>Required</strong> – A value for this parameter must be passed to the event.</li>
<li><strong>Key</strong> – The value passed for this event must be a key(s) value.</li>
<li><strong>Optional</strong> – A value for this parameter could be passed to the event but is not required.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>PARAMETER VALUE</p></td>
<td><p>Displays the value to pass to the parameter for the public event.</p>
<p><strong>NOTE:</strong> It the Parameter Type is Required or Key, this value must be entered.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the parameter.</p></td>
</tr>
</tbody>
</table>
