# Delete Files

All files in a directory according to a specific mask can be deleted.

**WARNING:** This action cannot be undone.

**NOTE:**  The root of a drive (i.e., C:\\) cannot be specified for the
Delete Files plugin.

To delete files:

1.  Select **Toolkit \> File/Folder** in *Navigation* pane.
    
    <span style="font-weight: bold;">NOTE:</span> If no records exist,
    the page displays in add mode. Otherwise, click
    <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Toolkit: File/Folder Operations
    page](../Page_Desc/Toolkit_File_Folder_Operations_H.htm)

2.  Enter a source directory in **IO DELETE SOURCE** field where files
    to be deleted reside.

3.  Click <span style="font-weight: bold;">Save</span>; the
    <span style="font-style: italic;">Vertical</span> View displays.
    
    [View the field descriptions for the Toolkit: File/Folder Operations
    page](../Page_Desc/Toolkit_File_Folder_Operations_H.htm)

4.  Enter a filter of what file to delete in **IO Delete Mask** field,
    e.g., **\*.pdf** to delete PDF files.

5.  Enter the number of days in **IO Delete Minimum Created Age** field
    (optional). If the file Created On date is older than this value,
    the file is deleted.

6.  Enter the number of days in **IO Delete Minimum Changed Age** field
    (optional). If the file Modified On date is older than this value,
    the file is deleted.
    
    **NOTE:** If both **IO Delete Minimum Created Age** and **IO Delete
    Minimum Changed Age** are specified, the utility will not delete the
    file unless <span class="underline">both</span> the CreatedOn and
    ModifiedOn dates of the file meet the respective criteria.

7.  Click **IO Delete Recursive** check box to enable it, deleting all
    files in subfolders (optional).

8.  Click **IO Delete Empty Folders** check box enabling it, deleting
    empty folders after files are deleted (optional).

9.  Click **Save.**

10. Click **Delete Files**; a confirmation message displays.

11. Click **Ok**; all files in the IO Delete Source folder that meet the
    following criteria are deleted:

<!-- end list -->

  - Conform to the IO Delete Mask
  - The Created On date is older than the IO Delete Minimum Created Age
    days
  - The Modified On date is older than the IO Delete Minimum Changed Age
    days
