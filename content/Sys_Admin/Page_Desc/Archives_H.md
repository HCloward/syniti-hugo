+++
title = 'Archives H'
solution = 'Platform'
+++

# Archives H

[Archive V](#Archive_V)

<div class="use">

Use this page to:

  - [Export CTS Archive to Target
    Instance](../Use_Cases/Export_CTS_Archive_to_Target_Instance)
  - [Import Archive to the Target
    Instance](../Use_Cases/Import_Archive_on_the_Target_Instance)

</div>

To access this page, click **Admin \>CTS \> Archives** on *Navigation*
pane.

|                 |                                                                                                                                                                                                                                                                         |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                                                                                                                                                             |
| Detect Archives | Click to detect all archives exported to this instance to be installed.                                                                                                                                                                                                 |
| NAME            | Displays name of the archive.                                                                                                                                                                                                                                           |
| DATE CREATED    | Displays date and time when the archive was created, (i.e., when the Build Archive button was clicked on the *CTS Build* page).                                                                                                                                         |
| Attributes      | Click to open the *[Archive Attributes](Archive_Attributes)* page to view attributes defined for the archive. Attributes for a CTS package are optional and allow for additional notes to be added to an archive that would be helpful to include with the package. |
| Manifest        | Click to open the *[Archive Manifes](Archive_Manifest)t* page to view the list of contents in an archive.                                                                                                                                                           |
| History         | Click to open the *[Archive History](Archive_History)* page to view an audit log of when the package was built, installed, etc. and by whom.                                                                                                                        |
| INSTALL         | Click to install the package into the instance.                                                                                                                                                                                                                         |
| EXPORT          | Click to move the package to designated instance. Once the archive is exported, the button name is updated to Re-Export.                                                                                                                                                |
| Log             | Click to open the *[Archive Log](Archive_Log)* page to view information about failed actions for the archive, such as when an install process fails.                                                                                                                |

## <span id="Archive_V"></span>Archive V

[Archives H](Archives_H)

<div class="use">

Use this page to:

  - [Export CTS Archive to Target
    Instance](../Use_Cases/Export_CTS_Archive_to_Target_Instance)
  - [Import Archive to the Target
    Instance](../Use_Cases/Import_Archive_on_the_Target_Instance)

</div>

Field

Description

General

Name

Displays name of the archive. When an archive is built from a package,
the package description is used as the name of the archive.

Description

Displays additional documentation about the package, such as a
description of what the package contains. When the archive is built from
a package, the comment from the package is used as the description of
the archive.

File Information

File Name

Displays name of install file generated when the Build Archive button is
clicked on the<span style="font-style: italic;">CTS Build</span>page.

Version

Displays the CTS version number. This value ensures that source and
target environments for an archive use the same version. 

History

Date Created

Displays date and time when the archive was created, i.e., when the
archive was built from the original package when the Build Archive
button on the<span style="font-style: italic;">CTS Build</span>page was
clicked.

Date Installed

Displays date and time when the archive was installed on the target
instance, i.e., when the Install/Import button on
the<span style="font-style: italic;">Archives</span>page was clicked.

Date Imported

Displays date and time when the archive record on the target instance is
inserted into the CranSoft database, i.e., when the Import button on
the<span style="font-style: italic;">Archives</span>page is clicked.

Date Exported

Displays date and time when the package was exported from the source
instance, i.e., when the Export button on
the<span style="font-style: italic;">Archives</span>page was clicked.
