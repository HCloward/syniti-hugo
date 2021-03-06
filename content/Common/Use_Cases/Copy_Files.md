+++
title = 'Copy Files'
solution = 'Platform'
+++

# Copy Files

Files can be copied from one directory into another directory.

To copy files:

1.  Select **Toolkit \> File/Folder** in *Navigation* pane.
    
    <span style="font-weight: bold;">NOTE:</span> If no records exist,
    the page displays in add mode. Otherwise, click
    <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Toolkit: File/Folder Operations
    page](../Page_Desc/Toolkit_File_Folder_Operations_H)

2.  Enter a source directory where the file currently exists in **IO
    COPY SOURCE** field.

3.  Enter a target directory where a copy of the file will be placed in
    **IO COPY TARGET** field.

4.  Click <span style="font-weight: bold;">Save</span>;
    <span style="font-style: italic;">Vertical</span> View displays.
    
    [View the field descriptions for the Toolkit: File/Folder Operations
    page](../Page_Desc/Toolkit_File_Folder_Operations_H)

5.  Enter a filter to narrow down the files copied in **IO Copy Mask**
    field, e.g., **\*.txt** to only copy text files.

6.  Click **IO Copy Make Directory** check box to enable it, creating
    needed folders in the IO Copy Target directory (optional). If
    disabled, an error displays if a folder is missing.

7.  Click **IO Copy Overwrite** check box to enable it, overwriting
    same-named files during the copy process (optional).

8.  Click **Save<span style="font-weight: normal;">.</span>**

9.  Click **Copy Files**; a confirmation message displays.

10. Click **Ok**; a copy of all files in the IO Copy Source directory
    that conform to the IO Copy Mask filter are moved into the IO Copy
    Target directory.
