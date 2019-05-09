+++
title = 'View and Configure Relationships for a Process Based on a GUI Script Template'
solution = 'Platform'
+++

# View and Configure Relationships for a Process Based on a GUI Script Template

<span id="Post Data using a GUI Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

A process based on a looped template must have links assigned to the
view for different loops. These links are called relationships and are
used to map values in parent views to values in child views.

Relationships between loops can be established manually, or Integrate
can automatically determine relationships using the Auto Generate
Database Objects feature.  Refer to
<span style="color: #0000ff;">[Generate Database Objects
Automatically](Generate_Database_Objects_Automatically)</span> for
more information.

For each unique value in the Parent Column Name, Integrate will look for
matching values in the Child Column Name and process each of the child
rows through the post process.

**NOTE**: Each loop must have a View Name and Primary Key Column Name
before a relationship can be added to the loop.

**NOTE**: If the **VIEW NAME** for a process template’s first loop is
updated on the *Process Template Loop* page, Integrate updates
relationships involving that loop with the new view name. Integrate
updates relationships whether or not the process was created using the
Auto Generate Database Objects feature.

**NOTE**: A process cannot be activated if the process is based on a GUI
Script template with loops and no relationships have been established
between the loops.

To add a relationship manually:

1.  Click **Categories** from *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click the **Loops** icon for a process based on a BDC Script
    template with multiple loops.

4.  Click **Relationships** on Page toolbar.
    
    *[View the field descriptions for the Relationship Mapping
    page.](../Page_Desc/RelationshipMappingBDCGUIBAPIRFC)*
    
    **NOTE**: Each loop level must be linked to another loop as either a
    parent or a child in a relationship.  The first loop in the process
    template and the parent of all other loops in the process template
    displays at the top of list on the *Relationship Mapping* page, and
    is called **Upload**.

5.  Click the + icon below a loop level.
    
    **NOTE**: This action allows the user to create a parent child
    relationship between the loop level above the + icon and the loop
    level that is above it in the hierarchy (the parent loop called
    **Upload**). For example, The *Relationship Mapping* page displays
    the Upload loop. Underneath Upload, Loop 1.1 and Loop 1.2 display.
    Clicking the plus icon beneath Loop 1.1 displays the *Process
    Template Loop View Relationships* page, where the user selects the
    column name for the parent Upload loop and the column name of the
    child Loop 1.1. This column name will link these loops together.

6.  Select a column name from **Parent Column Name** list box to set the
    parent relationship.
    
    **NOTE**: When Integrate generates the relationship automatically,
    it uses the value **ID** for the **Parent Column Name.** If the user
    manually sets a column as the **Parent Column Name**, this column
    must contain a unique value that can be mapped to a column in the
    child loop.  

7.  Select a column name from **Child Column Name** list box to set the
    child relationship.
    
    **NOTE**: When Integrate generates the relationship automatically,
    it uses the value **ParentID** for the **Child Column Name.** If the
    user sets a column as the **Child Column Name**, this column must
    contain a unique value that can be mapped to the **Parent Column
    Name** in the parent loop.  

8.  Click **Save**.

To edit a relationship on the *Relationship Mapping* page to accommodate
changes in tables an d views:

1.  Click **Edit** beneath the plus icon for a loop.
2.  Select an option from **Parent Column Name** list box.
3.  Select an option from **Child Column Name** list box.
4.  Click **Save**.
