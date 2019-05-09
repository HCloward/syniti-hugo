+++
title = 'Manage SAP Text List'
solution = 'Platform'
+++

# Manage SAP Text List

SAP Text tables must be registered in Collect in order for text tables
to function properly with the DSP®. SAP Text extracts are used to
download text lines, for example, for material and sales
orders.  Registering SAP Text tables allows users to create custom
downloads of this table type.

To create custom downloads:

1.  Select **Administrative \> SAP Text Lists** in the *Navigation*
    pane.

2.  Click **Add**.
    
    [View the field descriptions for the SAP Text List
    page](../Page_Desc/SAP_Text_List_H)

3.  Enter SAP Text table name in **TABLE** field.

4.  Enter object for table in **TEXT OBJECT** field if an object is
    used.

5.  Enter object key for table in **OBJECT KEY** field if a key for the
    object is used.

6.  Enter text ID for table in **TEXT ID** field if an ID must be
    specified.

7.  Enter default language in **LANGUAGE** field if the language must be
    specified.

8.  Click **Save**.

9.  Click **Vertical View** to further configure the SAP Text List.

10. Click **Edit**.
    
    [View the field descriptions for the SAP Text List page's Vertical
    View](../Page_Desc/SAP_Text_List_H)

11. Enter SQL used to build the custom table in **Build SQL Command**
    field.

12. Enter SQL used to alter the table SQL command used to build primary
    keys for table in **Build Primary Key** field.

13. Click **Save**.

14. Add table to the Target Source. Refer to the [Register Tables to
    Source](Register_Tables_to_Source) section for more information.
