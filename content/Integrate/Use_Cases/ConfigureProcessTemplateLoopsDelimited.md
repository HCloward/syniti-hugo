# Configure Process Template Loops for a Delimited or Fixed Width Template

<span id="Post Data Using UDF or Fixed Width Steps" class="popUpLink">Review
the steps in the process. </span>

For a Delimited or Fixed Width Template, the **VIEW NAME**, **PRIMARY
KEY COLUMN NAME** and **FLAT FILE OBJECT KEY** must be configured for
each loop in the process.

Use the Auto Generate Database Objects feature to automatically create
tables and views and to generate values for the **VIEW NAME**, **PRIMARY
KEY COLUMN NAME** and **FLAT FILE OBJECT KEY** value on the *Process
Template Loop* page. Refer to [Generate Database Objects
Automatically](Generate_Database_Objects_Automatically.htm) for more
information.

**NOTE**: The Flat File Object Key is a unique identifier for an object
that Integrate uses to join the data stored in different tables to make
a complete data set for the object. The data set has two loop levels,
the header and the details. For example, Integrate uses the flat file
object key of 1 in the first loop (the header) to join the header with
detail records stored in tables that also have the flat file object key
of 1. When posting, batch sizes are based on the number of header
records as set by the flat file object key.

Create tables and views manually in SQL or generate them using the
optional Auto Generate Database Object feature.

To generate database objects automatically:

1.  Click **Categories** on *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click the **Loops** icon for the process that uses the User Defined
    template.
    
    *[View the field descriptions for the Process Template Loop
    page.](../Page_Desc/Process_Template_Loop.htm)*
    
    **NOTE**: The **Loops** icon displays the number of structures added
    to the User Defined template during template creation.
    
    **NOTE** The *Process Template Loops* page displays a record for
    each structure. The **Field Mappings** icon displays the number of
    fields added to the structure during template creation.

4.  Click **Auto Generate Database Objects** on the Page toolbar; a
    confirmation message displays.
    
    **NOTE**: Auto Generate Database Objects will create tables in the
    DataSource mapped to the Process to serve as data staging for Upload
    and return value targets. It will also create Upload views based on
    the data staging tables. The created objects will be auto registered
    to the Process Template Loops. Auto Generating Database Objects will
    drop and re-create previously auto created objects.
    
    **NOTE**: The Auto Generate Database Objects feature is optional.
    Tables and views can be manually created in SQL.

5.  Click **Ok**.
    
    **NOTE**: Integrate populates the **VIEW NAME** with \[Process
    Name\] \[Template Name\] {Structure Name\], the **PRIMARY KEY COLUMN
    NAME** with **ID**, and the **FLAT FILE OBJECT KEY** with
    **FlatFileObjectKey**.

6.  Click the **Field Mappings** icon for a structure.
    
    **NOTE**: Integrate mapped all of the fields. The **TEMPLATE FIELD
    UNIQUE NAME** and **MAPPING VALUE** contain identical data.

7.  Navigate to the *Process* page.

8.  Click the **Templates** icon.

9.  Click **Vertical View** for the process template.

10. Click **Edit** for a process template.

11. Enter the file name format in **File Name Format** to override the
    default (if necessary).
    
    **NOTE**:  The default is set in Common in **Configuration \>
    Modules \> Integrate \> Parameters –Integrate**.  
    Set the format of the file name using the following set of possible
    dynamic replacement values:
    
      - \#Comment\# - From the DataRowContract, a comment passed into
        the post
      - \#Date\# - The date of the posting
      - \#PostingID\# - The ID of the posting
      - \#ProcessName\# - The name of the process
      - \#TemplateName\# - The name of the Template
    
    The dynamic replacement also supports any column name from the
    calling view.

12. Enter the path and folder name of the folder on the web server where
    the files should be stored in **Folder** to override the default (if
    necessary).
    
    **NOTE**: The default is set in Common in **Configuration \> Modules
    \> Integrate \> Parameters –Integrate**.

13. Select an option from the **Data Source ID** list box.
    
    **NOTE**: If transferring the file, this field must contain the data
    source ID of the remote FTP server where the files are transferred. 

14. Enter a symbol in **No Data Symbol**.
    
    **NOTE**: Integrate will use this symbol in the file if there is no
    data to post for a field.

15. Click **Save**.
