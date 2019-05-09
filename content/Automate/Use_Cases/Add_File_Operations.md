+++
title = 'Add File Operations'
solution = 'Platform'
+++

# Add File Operations

File Operations are the selection of the source and target paths, which
are created on the *[Logical Paths](../Page_Desc/Logical_Paths)*
page. This topic is also used for the configuration of other settings
required for the FileIterator event, which copies files from a source
folder to a target folder, then deletes the files from the source
folder. Refer to [About Automate Events](About_Automate_Events) for
more information.

To add file operations in Automate:

1.  Select **IO Config \> File Operations** in the *Navigation* pane.

2.  Click **Edit** for the desired file operation.
    
    [View the field description for the File Operations
    page](../Page_Desc/File_Operations)

3.  Enter the name of the operation to perform in the **OPERATION**
    field. It is recommended to create a name that references the in/out
    logical path and possibly the File Spec.

4.  Select the logical path of the source from which files will be
    transferred when the FileIterator event runs from the **LOGICAL PATH
    IN** list box. This path value was created on the *[Logical
    Paths](../Page_Desc/Logical_Paths)* page.

5.  Enter the file specification into the **FILE SPEC** field.
    
    **NOTE:** The FILE SPEC indicates the search pattern used to
    determine the files that are copied from the Source folder to the
    Target folder.

6.  Select the target path where the files are copied from when the
    FileIterator event runs from the **LOGICAL PATH OUT** list box. This
    path is configured on the *[Logical
    Paths](../Page_Desc/Logical_Paths)* page.

7.  Select the backup path from the **LOGICAL PATH BACKUP** list box.
    When the file is copied from the Source folder to the Target folder,
    it is deleted from the Source folder. The LOGICAL PATH BACKUP makes
    a backup copy of the file to a backup folder. This path is
    configured on the *[Logical Paths](../Page_Desc/Logical_Paths)*
    page.

8.  Click the **APPEND DATE** check box to enable it, which appends the
    current date (in the format YYYYMMDD) to the LOGICAL PATH OUT path
    folder.

9.  Click the **APPEND TIME** check box enable it, which appends the
    current time (in the format HHMMSS) to the LOGICAL PATH OUT path.

10. Click **Save**.

**NOTE:** If changes must be made to the source file data before the
file is copied to the target (e.g., adding or deleting a header),
populate the Script Path field on the *Vertical* View.
