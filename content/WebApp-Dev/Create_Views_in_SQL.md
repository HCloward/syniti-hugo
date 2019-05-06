# Create Views in SQL

All Dynamic pages in DSP® are based on a view.

When creating page views:

  - Do not include Order By statements. The **Order By** page property
    in DSP® must be used. Refer to Order By for more information.
  - Name the column names in the table so that the contents of the
    column are self-explanatory.
  - Do not alias column names in views solely for display purposes
    unless it is necessary to avoid duplicate column names in a view or
    to avoid adding labels and tabs. Translations in DSP® can be defined
    to change a column name. Refer to
    [Catalogs](../Sys_Admin/Use_Cases/Use_Catalogs.htm) for more
    information.
  - Only include the necessary tables.
  - For labels and tabs (column properties in DSP®), enter NULL in the
    column and enter the name of the label or tab in the Alias field.
    Refer to [Createa Label](Add_a_Label.htm) and [Add a
    tab](Add_a_Tab.htm) for more information.
  - Only fields that are present in the page’s view and associated table
    from the page definition are supported for input and edit. However,
    other tables and/or fields can be joined in the view to provide and
    display read-only supporting information.
  - Functions can be used to display content in a column, but can affect
    performance. A field that displays data from a function is read-only
    and cannot be updated.
  - Use a view to reference tables in another database. The most common
    use of this practice is when referencing Collect (dgSAP) tables or
    DSP® tables.
  - A view can also be used in a page property as a table selection as
    long as the required key(s) are listed in the view and properly
    defined in a column property. 
  - Do not add BOA reserved columns to views (except for the BoaStatus
    column). Refer to [Append BOA Reserved Columns to
    Tables](Append_BOA_Reserved_Columns_to_Tables.htm) for more
    information.

View Type refers to both the configuration of the page’s data views
(Horizontal, Vertical, etc.) as well as the Page Column View Type
specification. During page design, the Application Designer has to
consider fast page load, versus the quantity of relevant data that
displays on the page.

This section contains the following topics:

  - [SQL View/Function/Procedure
    Design](SQL_View_Function_Procedure_Design.htm)
  - [Horizontal vs Vertical Views](Horizontal_vs_Vertical_Views.htm)
