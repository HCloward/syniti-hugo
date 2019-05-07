+++
title = 'Configure Process Template Loops for an XML Template'
solution = 'Platform'
+++

# Configure Process Template Loops for an XML Template

<span id="Create and Transfer XML files Steps" class="popUpLink">Review
the steps to create and transfer XML files. </span>

Once an XML template has been added to a process, each loop in the
template must be configured either manually or by using the Auto
Generate Database Object feature. Each loop level must have a
relationship, View, and Primary Key Column Name configured.

Each loop level must be the Parent or Child of another loop and must
contain at least one relationship.

Enter the database objects manually, or use the optional Auto Generate
Database Objects feature to automatically generate tables and views in
the database, values for the **VIEW NAME** and **PRIMARY KEY COLUMN
NAME** on the *Process Template Loop* page, and relationships between
parent and children loops. Refer to [Generate Database Objects
Automatically](Generate_Database_Objects_Automatically.htm) for more
information.

To configure the process template loops for an XML Template
automatically:

1.  Click **Categories** on *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click the **Loops** icon for the process that uses the User Defined
    XML template.
    
    *[View the field descriptions for the Process Template Loop
    page.](../Page_Desc/Process_Template_Loop.htm)*
    
    **NOTE**: The **Loops** icon displays the number of structures added
    to the User Defined XML template during template creation.
    
    **NOTE** The *Process Template Loops* page displays a record for
    each structure. The **Field Mappings** icon displays the number of
    fields (elements and attributes) added to the structure during
    template creation.

4.  Confirm the **INCLUDE** check box is enabled for all rows.
    
    **NOTE**: If the **INCLUDE** check box is not enabled, the structure
    will not be included in the resulting XML file.

5.  Click **Auto Generate Database Objects** on the Page toolbar; a
    confirmation message displays.
    
    **NOTE**: Auto Generate Database Objects will create tables in the
    DataSource mapped to the Process to serve as data staging for Upload
    and return value targets. It will also create Upload views based on
    the data staging tables. The created objects will be auto registered
    to the Process Template Loops. Auto Generating Database Objects will
    drop and re-create previously auto created objects.
    
    **NOTE**: The Auto Generate Database Objects feature is optional.
    Views and tables can be added manually in SQL.

6.  Click **Ok**.
    
    **NOTE**: When using the Auto Generate Database Objects feature,
    Integrate populates the **VIEW NAME** with \[Process Name\]
    \[Template Name\] {Loop Name\] and the **PRIMARY KEY COLUMN NAME**
    with **ID**.

7.  Click **Field Mappings** for a structure.
    
    **NOTE**: Integrate mapped all of the fields. The **TEMPLATE FIELD
    UNIQUE NAME** and **MAPPING VALUE** contain identical data.

8.  Navigate to the *Process Template Loop* page.

9.  Click **Relationships**.
    
    **NOTE**: Integrate maps the parent child relationships
    automatically for each structure. All structures must be included in
    a parent child relationship for Integrate to generate the XML file
    correctly. 
    
    **NOTE**: A user can also add, update or delete parent child
    relationships manually. Refer to [Configure Process Template Loops
    for an XML Template](ConfigureProcessTemplateLoopsXML.htm) for more
    information.

10. Navigate to the *Process* page.

11. Click the **Templates** icon for the process.

12. Click **Vertical View** for the process template.

13. Click **Edit**.
    
    *[View the field descriptions for the Process Templates page’s
    Vertical
    View.](../Page_Desc/Process_Templates_H.htm#Process_Templates_V)*

14. Enter the file name format in **File Name Format** to override the
    default (if necessary).
    
    **NOTE**:  The default is set in Common in **Configuration \>
    Modules \> Integrate \> Parameters – Integrate**.  
    Set the format of the file name using the following set of possible
    dynamic replacement values:
    
    \#Comment\# - From the DataRowContract, this is a comment passed
    into the Post
    
    \#Date\# - The Date of the Posting
    
    \#PostingID\# - The ID of the Posting
    
    \#ProcessName\# - The Name of the Process
    
    \#TemplateName\# - The Name of the Template
    
    The dynamic replacement also supports any column name from the
    calling view.

15. Enter the path and folder name of the folder on the web server where
    the files should be stored in **Folder** to override the default (if
    necessary).
    
    **NOTE**: The default is set in Common in **Configuration \> Modules
    \> Integrate \> Parameters –Integrate**.

16. Select an option from the **Data Source ID** list box.
    
    <span style="font-family: Arial, sans-serif;">**NOTE**: If
    transferring the file, this field must contain the data source ID of
    the remote FTP server where the files are transferred. </span>

17. Click **Save**.
