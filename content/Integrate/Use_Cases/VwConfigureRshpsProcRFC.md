+++
title = 'View and Configure Relationships for a Process Based on an RFC'
solution = 'Platform'
+++

# View and Configure Relationships for a Process Based on an RFC

<span id="Post Data using an RFC Steps" class="popUpLink">\>Review the
steps in the process. </span>

Each loop in a process template based on an RFC template must be linked
to the Upload or Download loop through a relationship. The Auto Generate
Database Objects feature creates these relationships, but they can also
be edited.

Relationships between loops can be established manually, or Integrate
can automatically determine relationships using the Auto Generate
Database Objects feature.  Refer to
*<span style="color: #0000ff;font-style: normal;">[Generate Database
Objects
Automatically](Generate_Database_Objects_Automatically.htm)</span>* for
more information.

**NOTE:** If the **VIEW NAME** for a process template’s first loop is
updated on the *Process Template Loop* page, Integrate updates
relationships involving that loop with the new view name. Integrate
updates relationships whether or not the process was created using the
Auto Generate Database Objects feature.

To view relationships and configure them manually (if necessary):

1.  Click **Relationships** on the Page toolbar on the *Process Template
    Loop* page.
    
    **NOTE:** If the Auto Generate Database Object feature was used, in
    the column on the left, Integrate mapped each child loop to the
    Upload parent loop. Below the plus icon for each loop name, the blue
    and orange bar indicates that the Child ID has been mapped to the
    Parent ID (in this case the Upload loop).

2.  Click **Edit** for an Upload relationship.
    
    *[View the field descriptions for the Process Template Loop View
    Relationships page.](ProcTempLoopVwRlipsBDCGUIBAPIRFC.htm)*
    
    **NOTE:** The **Parent Direction** and **Child Direction** display
    Upload. The View Name for the Parent Upload is the view name
    generated for this loop by the Auto Generate Database Objects
    feature.  The View Name can be manually updated and saved on the
    *Process Template Loop* page. In this case, Integrate will update
    the View Name in the Parent Upload loop for the relationships.

3.  Select a column name from **Parent Column Name** list box to set a
    parent relationship if necessary.
    
    **NOTE:** When Integrate generates the relationship automatically,
    it uses the value **ID** for the **Parent Column Name.** If the user
    manually sets a column as the **Parent Column Name**, this column
    must contain a unique value that can be mapped to a column in the
    child loop. 

4.  Select a column name from **Child Column Name** list box to set the
    child relationship if necessary.
    
    **NOTE:** When Integrate generates the relationship automatically,
    it uses the value **ParentID** for the **Child Column Name.** If the
    user sets a column as the **Child Column Name**, this column must
    contain a unique value that can be mapped to the **Parent Column
    Name** in the parent loop.  

5.  Navigate back to the *Relationship Mapping* page.
    
    **NOTE:** In the column on the right, Integrate also mapped each
    child loop with download fields to the Download parent loop  Below
    the plus icon for each loop name, the blue and orange bar indicates
    that the Child ID has been mapped to the Parent ID (in this case the
    Download loop). Integrate also sets a relationship between the
    Parent Upload loop and Parent Download loop. The Download loops
    (those loop that contain download fields) map to the Parent Upload
    loop through the Parent Download loop.  This way, each record
    uploaded via the Primary Upload loop will have one or many
    corresponding records in the download tables.

6.  Click **Edit** for a Download relationship.
    
    [View the field descriptions for the Process Template Loop View
    Relationships page.](ProcTempLoopVwRlipsBDCGUIBAPIRFC.htm)
    
    **NOTE:** The **Parent Direction** displays **Upload**. The **Child
    Direction** displays **Download**.

7.  Select a column name from **Parent Column Name** list box to set a
    parent relationship if necessary.
    
    **NOTE:** When Integrate generates the relationship automatically,
    it uses the value **ID** for the **Parent Column Name.** If the user
    manually sets a column as the **Parent Column Name**, this column
    must contain a unique value that can be mapped to a column in the
    child loop. 

8.  Select a column name from **Child Column Name** list box to set the
    child relationship if necessary.
    
    **NOTE:** When Integrate generates the relationship automatically,
    it uses the value **ParentID** for the **Child Column Name.** If the
    user sets a column as the **Child Column Name**, this column must
    contain a unique value that can be mapped to the **Parent Column
    Name** in the parent loop.
