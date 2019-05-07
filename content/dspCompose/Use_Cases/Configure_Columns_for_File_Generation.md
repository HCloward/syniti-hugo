+++
title = 'Configure Columns for File Generation and Data Entry'
solution = 'Data Quality'
+++

# Configure Columns for File Generation and Data Entry

At the request role level, if Excel import is allowed for the template
used by the request, a user assigned to the role can generate an Excel
file to use for data entry.

**NOTE**: To enable Excel import for a template role, on the *Template
(Role Excel Column Control)* page’s *Vertical* View, on the **Import
Settings** tab, click the **Excel Import Allowed** check box to enable
it. This check box is enabled by default.

After data entry is complete, a user can then upload the Excel file at
the request role level and import the data to the mapped page. On the
*Vertical* View of the *Request (Roles)* page, a user clicks the
**Import** button to perform this action.

Column properties can also be added to Data Entry pages to control data
entry on the <span style="font-style: italic;">Data Entry</span> page or
the <span style="font-style: italic;">Mass Change</span> page.

**NOTE**: The column properties added to the Data Entry pages for a
request are available for all additional requests based on the template.

Column properties specify required fields and ensure that specific
values are selected through a list box or combo box when a user manually
enters data. If the data for the request is imported from a view and the
value of the field does not meet the criteria of the column property,
the record displays as invalid.

Some effective column properties to control data entry are:

  - **List Box** - Displays a field as a list box with options from a
    selected table or view**.**
  - **Combo Box** - Displays a field as a text box with options from a
    selected table or view that display once text is entered in the
    field. To improve performance, use a combo box instead of a list box
    when the list view contains too many records to display suitably as
    a list box.
  - **Check Box -** Displays a field as a check box that can be enabled
    or disabled and apply the correct format and value in the database.
  - **Required Fields** - There are two types of required fields:
      - Hard Required - The record cannot be saved until the field is
        populated.
    
      - Soft Required - The record can be saved without the field being
        populated, but is not considered valid until the field is
        populated.

**NOTE:** Any field in the table that does not allow NULLS, such as a
Primary Key, is automatically a Hard Required field.

To configure columns:

  - [Configure Column Display](Configure_Column_Display.htm)
  - [Set a Column’s Control Status](Set_a_Columns_Control_Status.htm)
  - [Add List Boxes to an Excel
    File](Add_List_Boxes_to_an_Excel_File.htm)
  - [Format Required Fields in an Excel
    File](Format_Required_Fields_in_an_Excel_File.htm)
  - [Create Validations for List
    Boxes](Register_Validations_to_List_Boxes.htm)
  - [Import a Column Added to the Role’s Assigned
    Page](Import_a_Column_Added_to_the_Roles_Assigned_Page.htm)
