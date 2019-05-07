+++
title = 'CTS Build H'
solution = 'Platform'
+++

# CTS Build H

[CTS Build V](#CTS_Build_V)

<div class="use">

Use this page to [Create Package and Build Archive in Source
Instance.](../Use_Cases/CreatePckgeBuildArcSrceInstance.htm)

</div>

To access this page, select **Admin \> CTS \> Build** in
the *Navigation* pane.

|                    |                                                                                                                                                                                |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field              | Description                                                                                                                                                                    |
| DESCRIPTION        | Displays name of the CTS package.                                                                                                                                              |
| Items              | Click to open the *[CTS Items](CTS_Items_H.htm)* page to configure specific items to include in the package.                                                                   |
| Build Packing List | Click to create a list of items and dependencies to include in the package.                                                                                                    |
| Packing List       | Click to open the [CTS Packing List Summary](CTS%20Packing%20List%20Summary.htm) page to view and exclude items from the packing list.                                         |
| Build Archive      | Click to create an installable archive from a package.                                                                                                                         |
| DATE CREATED       | Displays date and time when the package was created, i.e., when the package record was added to the this page.                                                                 |
| LOG                | Click to open the *[CTS Log](CTS_Log.htm)* page to view error or debug information about the package when either the build packing list or the build archive processes failed. |

## <span id="CTS_Build_V"></span>CTS Build V

[CTS Build H](CTS_Build_H.htm)

<div class="use">

Use this page to [Create Package and Build Archive in Source
Instance.](../Use_Cases/CreatePckgeBuildArcSrceInstance.htm)

</div>

Field

Description

Properties

Description

Displays name of the CTS package.

Comments

Displays additional documentation about the package, such as a
description of what the package contains.

Attributes

Click to open the *[CTS Attributes](CTS_Attributes.htm)* page to add,
edit and delete attributes to be included in an archive. An attribute
allows for additional notes to be added to an archive.

Options

Include Objects

If checked, objects added on the *[CTS Configure (SQL Object
Registrations)](CTS%20Configure%20SQL%20Object%20Registrations.htm)*
page are included in the package.  The default value is checked.

Show Hidden Items

If checked, CTS items defined as “hidden” on the *Vertical* View of the
*[CTS Configure (Shippable
Items)](CTS%20Configure%20Shippable%20Items.htm)* page are visible in
the packing list. The default value is unchecked.

Trace Level

Displays severity of the message logged. Values are: Debug, Error,
Warning, and Message, where Error provides the least amount of
information and Debug provides the greatest amount of information.

History

Date Created

Displays date and time when the package was created, i.e., when the
package record was added to this page.

Date Built

Displays date and time when the archive was built from a package, as in,
when the Build Archive button was clicked on this page.
