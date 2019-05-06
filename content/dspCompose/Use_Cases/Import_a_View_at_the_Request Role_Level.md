# Import a View at the Request-Role Level

<span style="font-weight: bold;">NOTE</span>: To import a view, the View
Import Allowed check box must be enabled on the
<span style="font-style: italic;">Template (Role)</span> page’s
<span style="font-style: italic;">Vertical</span> View’s Import Settings
tab for the Data role. Access this check box via Teams \> Templates \>
Roles \> Vertical View of the Data role. A data source must also be set
for the Data role. Refer to [Add a Data Source that Stores Views for
Import](Add_a_Data_Source_that_Stores_Views_for_Import.htm) for more
information.  

dspCompose™ accommodates complex posting workflows that have multiple
Data Entry roles. Each role can import data into different tables by
importing a view at the request-role level.

The user can import data from a view using a Where clause constructed in
the Where Clause Builder. This Where clause also applies to any request
data that is exported for a role.

When importing a view:

  - Ensure the columns named in the view **match exactly** the technical
    column names on the data entry page. By default, dspCompose™ names
    the columns on the data entry page for the target system’s table
    name/column name combination. For example, if the BISMT field on the
    MARA table is found during an SAP recording, the column name on the
    data entry page is: \[MARA-BISMT\].
  - Do not include a column named ID in the view that is being imported.
    dspCompose™ uses a hidden identity field to ensure record uniqueness
    and having an ID column on the field may lead to unexpected results
    in certain circumstances.
  - Click the **View Data** icon on the *Vertical* View of a request
    role before import to ensure that the data in the view is
    appropriate for import into the request. View Data takes the
    statement in the Where Clause column into account when displaying
    the data to provide an accurate representation of the data that will
    be imported.

**NOTE**: View Import data is always added to a data entry page. View
Import cannot be used to update data.

**NOTE**: A user can set a default data source and view for the
template. Refer to [Assign Default Data Source and
Views](Assign_Default_Data_Source_and_Views.htm) for more information.

To import a view that contains the request data:

1.  Select **Requests** in the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Roles** for the request.

3.  Click **Vertical View** for the role that allows data entry.

4.  Click **Edit**.
    
    *[View the field descriptions for the Request Roles page’s Vertical
    View.](../Page_Desc/Request_Roles_H.htm)*

5.  Select an option from the **Data Source ID** list box.
    
    **NOTE:** The Data Source ID is the data source that contains the
    views that can be imported into the request. The data source must be
    added at the template-role level for the Data role. Refer to [Add a
    Data Source that Stores Views for
    Import](Add_a_Data_Source_that_Stores_Views_for_Import.htm) for more
    information.

6.  Select an option from the **View** list box.
    
    **NOTE:** The View is used to populate the data after the request is
    processed.

7.  Click **Save**.

8.  Click **ViewWhere Clause Builder**.
    
    *[View the field descriptions for the Request (Role View Filter)
    page.](../Page_Desc/Request_Role_View_Filter.htm)*
    
    **NOTE:** A Where clause is used for import only, and not when
    deleting records. If the user selects the **Delete Data Before
    Import** check box on the *Vertical* View of the *Request (Roles)*
    page, data will be deleted from the target for the request-role
    combination.

9.  Select an option from the **COLUMN NAME** list box.
    
    **NOTE:** The COLUMN NAME displays the column used to form the Where
    clause when importing a view at the request-role level.

10. Select an option from the **CONDITIONAL** list box.
    
    **NOTE:**<span>The CONDITIONAL displays the operation used if a
    comparison between two fields is required.</span>

11. Enter a value in **VALUE** field.
    
    **NOTE:** The VALUE is the mass change value used when filtering
    data during the import.

12. Click **Save**.

13. Click **Back** on the browser to return to the *Request (Roles)*
    page’s *Vertical* View.
    
    **NOTE:** The Where clause displays in the **Where Clause** field.
    
    **NOTE:** This Where clause filters on the data within the view to
    only import a subset of data when the request is processed.

14. Click **View Data** to view the request data in the view before it
    is imported.
    
    **NOTE:** The View Data option is only available until a request has
    been posted.

15. Click the **View Delete Data Before Import** check box to enable it,
    if necessary.
    
    **NOTE:** If the View Delete Data Before Import check box is
    enabled, when importing data from the view, dspCompose™ deletes the
    existing target table records and adds records from the view.

16. Click **Import View Data** to bring the view data into the request.
