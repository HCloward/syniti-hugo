+++
title = 'Enable File Upload and Download'
solution = 'Platform'
+++

# Enable File Upload and Download

The Files Column Property is used to stage any type of file including
graphics, text, Word or Excel files. Files are stored in a specific
location on the web server and are enabled for download.

This feature is available for the File control only.

To enable file upload and download:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page</span> for a column with a File control.

2.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H)*

3.  Enter the path name to upload files to and to store files for
    download in **File Path** field.
    
    **NOTE:** The user must manually create the folder if it does not
    already exist.
    
    **NOTE:**The files are usually stored in a folder with the same name
    as the DSP® WebApp ID (GUID). Use the forward slash **/** within and
    at the end of the path. The forward slash at the end of the path
    denotes a folder. For example, if **/NWEmployees** is used, it is
    treated as a file name. **/NWEmployees/employee/** is treated as a
    folder.
    
    **NOTE:** The folder **UserArea** is created by DSP® and should
    always be the first folder name in the path. The English folder is
    required and must be added by the user. The WebApp ID sets the path
    to the WebApp. Other folders or sub folders can be used but the
    English folder is used as the default.

4.  Select **Virtual** from the **File Path Type** list box.

5.  Select **Upload or Download** from the **File Direction** list box.

6.  Click **Save**.
