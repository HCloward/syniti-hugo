# Toolkit: File/Folder Operations H

[Toolkit: File/Folder Operations V](#Toolkit_File_Folder1)

<div class="use">

Use this page to:

  - [Copy Files](../Use_Cases/Copy_Files.htm)
  - [Move Files](../Use_Cases/Move_Files.htm)
  - [Copy Folders](../Use_Cases/Copy_Folders.htm)
  - [Delete Files](../Use_Cases/Delete_Files.htm)

</div>

To access this page, select <span style="font-weight: bold;">Common \>
Toolkit \> File/Folder</span> in
<span style="font-style: italic;">Navigation</span>
pane.

|                  |                                                                       |
| ---------------- | --------------------------------------------------------------------- |
| Field            | Description                                                           |
| ID               | Displays ID of record.                                                |
| IO COPY SOURCE   | Displays source directory where file/folder currently exists.         |
| IO COPY TARGET   | Displays target directory where file/folder is copied or moved.       |
| IO DELETE SOURCE | Displays source directory where files or folder to be deleted reside. |

## <span id="Toolkit_File_Folder1"></span>Toolkit: File/Folder Operations V

[Toolkit: File/Folder Operations
H](Toolkit_File_Folder_Operations_H.htm)

<div class="use">

Use this page to:

  - [Copy Files](../Use_Cases/Copy_Files.htm)
  - [Move Files](../Use_Cases/Move_Files.htm)
  - [Copy Folders](../Use_Cases/Copy_Folders.htm)
  - [Delete Files](../Use_Cases/Delete_Files.htm)

</div>

Field

Description

ID

Displays ID of record.

Copy/Move

IO Copy Source

Displays source directory where file/folder currently exists.

IO Copy Target

Displays target directory where file/folder is copied or moved.

IO Copy Mask

Displays filter to restrict files or folders being copied.

IO Copy Make Directory

If enabled, needed folders are created in the IO Copy Target directory.
If disabled, an error displays if a folder is missing.

IO Copy Recursive

If enabled, all subfolders are copied.

IO Copy Overwrite

If enabled, same-named files are overwritten during the copy process.

Copy Files

Click to copy all files in the IO Copy Source directory that form to the
IO Copy Mask filter to the IO Copy Target directory.

Copy Folder

Click to copy the folder from the IO Copy Source to the IO Copy Target
directory.

Move File

Click to move (and rename) the IO Copy Source to the IO Copy Target.

Delete

IO Delete Source

Displays source directory where files or folder to be deleted reside.

IO Delete Mask

Displays filter to restrict files or folders being deleted.

IO Delete Minimum Created Age

Displays number of days where, if the file Created On date is older than
this value, the file is deleted.

IO Delete Minimum Changed Age

Displays number of days where, if the file Modified date is older than
this value, the file is deleted.

IO Delete Recursive

If enabled, all subfolders within the folder being deleted are deleted.
If disabled, all subfolders within the folder being deleted remain, but
are empty

IO Delete Empty Folders

If enabled, empty folders are deleted after files are deleted.

Delete Files

Click to delete the IO Delete Source folder that conforms to the IO
Delete Mask, and if the Created On date is older than the IO Delete
Minimum Created Age days and the Modified On date is older than the IO
Delete Minimum Changed Age days, the files are deleted.

Delete Folder

Click to delete the folder and all its contents.
