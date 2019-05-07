+++
title = 'Build Views'
solution = 'Platform'
+++

# Build Views

The Build View process allows users to create views in one database that
reference every table in another database.

To build a view:

1.  Select **Tools \> Build View** in *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Build View
    page](../Page_Desc/Build_View_H.htm)

3.  Select database from **SOURCE DATABASE** list box to control the
    database where tables are referenced.

4.  Select database from **TARGET DATABASE** list box to control the
    database where views are created.

5.  Enter a client in **SAP CLIENT** field if binding the new views off
    client information.

6.  Enter a language in **SAP LANGUAGE** field if binding the new views
    off language information.

7.  Click **OVERWRITE EXISTING VIEWS** check box to overwrite existing
    views in target database with views from the source database.

8.  Click **Save**.

9.  Add Client Columns and/or Language Columns if binding the new views
    off client or language information. Refer to [Add Client
    Columns](#Add_Client_Columns) and [Add Language
    Columns](#Add_Language_Columns) for more information.

10. Select the target/source combination.

11. Click **Build Views** icon to build a view in the Target Database
    for each table in the Source Database with specific client and
    language filters (if filters are applied); a confirmation message
    displays.

12. Click **Ok**.

## <span id="Add_Client_Columns"></span>Add Client Columns

Add client columns if binding (i.e., filtering) the new views (i.e.,
views created from the Build View process) off client information.
Client columns added will be bound based on the SAP Client specified on
the *[*Build View*](../Page_Desc/Build_View_H.htm)* page.

To configure client columns:

1.  Select <span style="font-weight: bold;">Tools \> Build View</span>
    in <span style="font-style: italic;">Navigation</span> pane.
    
    **NOTE:** Data does not display on the *Build View* page until a
    view is built.

2.  Click **Client Columns** for target/source combination.

3.  Click **Add**.
    
    [View the field descriptions for the Client Column Name Variant
    page](../Page_Desc/Client_Column_Name_Variant.htm)

4.  Enter a variation of SAP Client in **COLUMN** field.

5.  Click **Save.**

## <span id="Add_Language_Columns"></span>Add Language Columns

Add language columns if binding (i.e., filtering) the new views off
language information. Language columns added will be bound based on the
SAP Language specified on the *[*Build
View*](../Page_Desc/Build_View_H.htm)* page.

To configure language columns:

1.  Select <span style="font-weight: bold;">Tools \> Build View</span>
    in <span style="font-style: italic;">Navigation</span> pane.
    
    **NOTE:** Data does not display on the *Build View* page until a
    view is built.

2.  Click **Language Columns** for target/source combination.

3.  Click **Add.**
    
    [View the field descriptions for the Language Column Name Variant
    page](../Page_Desc/Language_Column_Name_Variant.htm)

4.  Enter a variation of SAP Language in **COLUMN** field.

5.  Click **Save.**
