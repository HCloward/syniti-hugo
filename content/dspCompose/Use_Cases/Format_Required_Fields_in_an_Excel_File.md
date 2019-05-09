+++
title = 'Format Required Fields in an Excel File'
solution = 'Data Quality'
+++

# Format Required Fields in an Excel File

A user can generate an Excel file at the request role level for data
entry purposes. To indicate that a column in the file is required,
dspCompose™ can format the column according to options set on the
*Template (Role Excel Column Control)* page.

**NOTE:** On the *Template (Role*) page, the **Excel Column Control**
icon is disabled after a user records a template. Once the template is
generated, this icon is enabled. To generate a template, on the
*Templates* page’s *Vertical* View, click **Generate**.

<span style="font-weight: bold;">NOTE:</span> The default background
color and text color for required fields are set at the Parameter level
on the <span style="font-style: italic;">Parameters</span> page on the
Posting and File tab (Configuration \> Parameters).

To set formatting for required columns:

1.  Click **Team** on *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Excel Column Control** for a role.

5.  Click **Required Columns Format** on the Page toolbar.

6.  Click **Edit**.
    
    *[View the field descriptions for the Template Role Excel (Required
    Columns)
    page.](../Page_Desc/Template_Role_Excel_Required_Columns)*

7.  Select a color from the **Background Color** list box.

8.  Select a color from the **Text Color** list box.

9.  Click **Save**.

10. Click **Preview** on the Page toolbar to view the formatting.

This setting is saved at the template role level, and determines how
required columns in Excel display when dspCompose™ generates a file at
the corresponding request role level.

For example, a Required Columns Format has been set for a template
called Create Customer for the Data role. The background color of a
required column displays red. A user with the Date role creates a
request based on the Create Customer template, and clicks the **Generate
Template File** icon on the *Vertical* View of the *Request (Roles)*
page. dspCompose™ generates an Excel file, and formats all required
columns in red, indicating that these columns cannot be left blank.
