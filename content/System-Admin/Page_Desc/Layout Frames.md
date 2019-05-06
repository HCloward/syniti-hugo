# Layout Frames

<div class="use">

Use this page to[:](../../WebApp_Dev/Create_Header_Detail_Pages.htm)

  - [Create a Header Detail
    Page](../../WebApp_Dev/Create_Header_Detail_Pages.htm)
  - [Create a Dashboard](../../WebApp_Dev/Create_a_Dashboard.htm)

</div>

**NOTE**: Different columns display on this page depending on how it is
accessed.

To access this page:

1.  Click **WebApps** in the *Navigation* pane.
2.  Click the **Pages** icon for a WebApp.
3.  Click **Vertical View** for a page with the page type of Header
    Detail.
4.  Click the **Frames** icon.

OR

1.  Click **Configuration \> Layouts** in the *Navigation* pane.
2.  Click the **Layout Frames** icon.

OR

While [creating a dashboard](../../WebApp_Dev/Create_a_Dashboard.htm),
click the **+** icon in the Layout ID field on the *Vertical* View of
the *[Pages](Pages_H.htm)* page

<table>
<tbody>
<tr class="odd">
<td style="text-align: left;"><p>Field</p></td>
<td style="text-align: left;"><p>Description</p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p>PRIORITY</p></td>
<td style="text-align: left;"><p>Displays the priority of the header page, 10, or the detail page, 20. when the page is accessed for a Header Detail page.</p>
<p>For non Header/Detail pages, the priority sets the sort order on the page.</p></td>
</tr>
<tr class="odd">
<td style="text-align: left;"><p>DEPENDENT FRAME ID</p></td>
<td style="text-align: left;"><p>Displays the frame ID of the dependent page. This column is blank for the Header row for a Header/Detail page.</p>
<p><strong>NOTE</strong>: This column only displays when the page is accessed from the Frames icon, available on the <em>Vertical</em> View of the <em>Pages</em> page for a page type of Header Detail.</p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p>DESCRIPTION</p></td>
<td style="text-align: left;"><p>Displays a description of the header page, detail page or frame.</p></td>
</tr>
<tr class="odd">
<td style="text-align: left;"><p>DEFAULT PAGE ID</p></td>
<td style="text-align: left;"><p>Displays the page in the WebApp defined as the header, detail page or dashboard.</p>
<p><strong>NOTE</strong>: This value is populated once the dashboard based on this layout has been saved.</p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p>INITIAL PAGE COLUMN</p></td>
<td style="text-align: left;"><p>Displays the name of the Detail page that displays when a Header Detail page opens. A Header Detail page always displays two pages: the Header, or parent, page and the Detail, or child, page. The Header page is always connected to the Detail page via a button with a link to the Detail page.</p>
<p>If there are multiple buttons on the Header page that link to different Detail pages, this setting determines the Detail page that displays when the Header Detail page opens.</p>
<p><strong>NOTE</strong>: This field must be completed if a Header page can open different Detail pages to ensure both the Header and Detail pages can automatically open when the page is being rendered.</p>
<p><strong>NOTE</strong>: This column only displays when the page is accessed from the Frames icon, available on the <em>Vertical</em> View of the <em>Pages</em> page for a page type of Header Detail.</p></td>
</tr>
</tbody>
</table>
