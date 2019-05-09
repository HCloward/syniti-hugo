+++
title = 'Assign Page Properties to a Dynamic Page'
solution = 'Platform'
+++

# Assign Page Properties to a Dynamic Page

Page Properties are used to control how the page displays and to define
actions that can be performed on the page, including functions on the
Page toolbar.

Refer to [Page Design Guidelines](Page%20Design%20Guidelines) for
general information.

These page properties can be set for Dynamic pages on the
*[Pages](../Sys_Admin/Page_Desc/Pages_H)* page *Vertical* View on
the General tab or the Advanced Properties tab.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Property</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Order By</p></td>
<td><p>Sets the default sort columns in either ascending or descending order based on Field Name on the <em>Horizontal</em> View only. Sorting must be done in the DSP®, not in the SQL view.</p>
<p><strong>NOTE</strong>:   When a field name is entered in Order By field, the default order is ascending. To sort in descending order, enter the field name followed by a space and desc, for example, lastname desc. Separate entries by a comma.</p></td>
</tr>
<tr class="odd">
<td><p>Persistent Insert</p></td>
<td><p>Forces the page to remain in add mode after a record is entered and saved. It is a useful feature on a page where a user would add multiple records at one time.</p></td>
</tr>
<tr class="even">
<td><p>Support Download</p></td>
<td><p>Allows records on the page to download to an Excel spreadsheet, Word document or other formats. By default, Download is enabled for all pages. When Support Download is disabled, the Download feature is not available.</p>
<p>Refer to <a href="Enable_File_Upload_Download">Enable File Upload/Download</a> for more information.</p>
<p>Use this feature depending on the type of data the page displays, for example, a metric-related page may be useful to download, while a page containing sensitive information may not.</p>
<p><strong>NOTE</strong>: Exclude fields, such as images and buttons, in the downloaded file if needed. Refer to <a href="Set_Column_Control_Status">Set Column Control Status</a> for more information.</p>
<p><strong>NOTE</strong>: In a case where fields should be included on the Download page that are not visible on the <em>Horizontal</em> or <em>Vertical</em> View, hide fields using the page columns All Views view type, but then enable them on the Download for this level of control. Refer to <a href="Enable_File_Upload_Download">Enable File Upload/Download</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Enable Excel Integration</p></td>
<td><p>If enabled, Excel integration is available on the page.</p>
<p>Excel Integration is the ability, at the framework level, to enable end-users to import data from Excel into DSP® pages.  </p>
<p>Refer to <a href="../Sys_Admin/Use_Cases/Enable_Excel_Integration">Enable Excel Integration</a> and <a href="../Excel_Int/Use_Excel_Integration">Use Excel Integration</a> for more information</p></td>
</tr>
</tbody>
</table>
