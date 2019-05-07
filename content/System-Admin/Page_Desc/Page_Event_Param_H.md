+++
title = 'Page Event Parameters H'
solution = 'Platform'
+++

# Page Event Parameters H

Page Event Parameters V

<div class="use">

Use this page to [Set Parameters for a Public WebApp
Event](../../WebApp_Dev/Set_Param_Public.htm).

</div>

To access this page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click **Pages** for a WEB APP NAME.

3.  Click **Events** for a page.

4.  Click **Vertical View** for an event.

5.  Click the **Advanced Properties** tab.

6.  Click the **Parameters** icon.
    
    **NOTE:** The Parameters icon is active if the Public check box is
    checked on the Page Events page’s Vertical View.

<table>
<thead>
<tr class="header">
<th style="text-align: left;"><p>Field</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;"><p>PRIORITY</p></td>
<td><p>Displays the sort order on this page to indicate the parameter’s relative importance or logical grouping. The priority order is used when aligning values from another event to call this event. The framework auto-inserts the table’s key fields in their order from the table, and/or the page’s column properties marked as keys. Commonly, higher priority parameters are specific to other business rules, such as plugins or procedures that expect other row data.</p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p>PARAMETER NAME</p></td>
<td><p>Displays the name of the parameter passed by a WebApp to run this Public event. The key(s) fields on the table upon which the page is based are included by default if the Public check box on the Page Events page has been checked.</p></td>
</tr>
<tr class="odd">
<td style="text-align: left;"><p>PARAMETER TYPE</p></td>
<td><p>Displays whether the parameter is a key field on the table when executing this public event and must be passed or is optional. Options are:</p>
<ul>
<li><strong>Required</strong> – A value for this parameter must be passed to the event</li>
<li><strong>Key</strong> – The value passed for this event must be a key(s) value. This value is also required, but is treated as a key field, not a data field, during event execution.</li>
<li><strong>Optional</strong> – A value for this parameter could be passed to the event, but it is not required.</li>
</ul>
<p><strong>NOTE:</strong> The value selected is displayed to a developer, when setting up an event to call this public event from another page.</p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p>DESCRIPTION</p></td>
<td><p>Displays a description of the parameter.</p></td>
</tr>
</tbody>
</table>

## <span id="Page"></span>Page Event Parameters V

Page Event Parameters H

Field

Description

Priority

Displays the sort order on this page to indicate the parameter’s
relative importance or logical grouping. The priority order is used when
aligning values from another event to call this event. The framework
auto-inserts the table’s key fields in their order from the table,
and/or the page’s column properties marked as keys. Commonly, higher
priority parameters are specific to other business rules, such as
plugins or procedures that expect other row data.

Parameter Name

Displays the name of the parameter passed by a WebApp to run this Public
event. The key field(s) on the table upon which the page is based are
included by default if the Public check box is checked on the Page
Events page's Vertical View.

Parameter Type

Displays whether the parameter is a key field on the table when
executing this public event and must be passed or is optional. Options
are:

  - **Required** – A value for this parameter must be passed to the
    event
  - **Key** – The value passed for this event must be a key(s) value.
    This value is also required, but is treated as a key field, not a
    data field, during event execution.
  - **Optional** – A value for this parameter could be passed to the
    event, but it is not required.

**NOTE:** The value selected is displayed to a developer, when setting
up an event to call this public event from another page.

Description

Displays a description of the parameter.

Advanced Properties

NOTE: <span style="font-weight: normal;">Configuring the fields in this
section will present the user with a list box with the options entered
below on the *Page Event Parameters* page's *Vertical* View. These
options are used when they are configuring the page to call this public
WebApp event.</span>

List View

Displays the name of the view in SQL that contains the values and
displays fields for a list box if the values for a list box must be
passed to the event.

List Value Field

Displays the name of the field that stores the value. In most cases,
List Value Field is the primary key stored in the table. Refer to [Add
List Boxes and Combo
Boxes](../../WebApp_Dev/Add_List_Boxes_and_Combo_Boxes.htm) for more
information.

List Display Field

Displays the option visible in the List Box or Combo Box. Refer to [Add
List Boxes and Combo
Boxes](../../WebApp_Dev/Add_List_Boxes_and_Combo_Boxes.htm) for more
information.
