+++
title = 'Set the Control Table Prefix'
solution = 'Master Data Management'
+++

# Set the Control Table Prefix

When a table is generated for control views, the control table prefix is
added to the table name. The prefix can be set at the category and page
level.

<span style="font-weight: bold;">NOTE</span>: dspConduct™ is delivered
with a default control table prefix. Updating the prefix is optional.

The control table prefix set at the category level on the
[Category](../Page_Desc/Category_H.htm) page’s
<span style="font-style: italic;">Vertical View</span> is the prefix to
the table name when a table is generated for a scenario \> role \> task
combination for the category. When a table is generated for the control
views or required validations, the table name starts with this
configured text.

For example, a user can enter the prefix "ttSRTC\_" and all control
tables for the category are generated with that prefix.

The control table prefix set at the page level on the [Task
Page](../Page_Desc/Task_Page_H.htm) page is the prefix in the table name
when a table is generated for a scenario \> role \> task combination
that uses this page.

When a table is generated, it follows the naming convention \[Control
table prefix\]\_\[Page View’s Root Name\]\_\[variant column name or
required\].

For example, a content page named “Address” has a Horizontal View
webRequestAddressHor. The control tables prefix configured for this
Category is "ttSRTC\_". The task has an active variant configured for
the “Country” field. On the
<span style="font-style: italic;">Vertical</span> View of the Task Page
page for “Address”, the Control Table Prefix is
“ttSRTC\_RequestAddress\_”. When created, the control view table name
is ttSRTC\_RequestAddress\_Country.

Refer to [Create Tables and Views for Content WebApp
Pages](Create_Tables_and_Views_for_Content_WebApp_Pages_Overview.htm)
and [Create and Configure Column
Variants](Activate_Configure_Column_Variants.htm) for more information.
