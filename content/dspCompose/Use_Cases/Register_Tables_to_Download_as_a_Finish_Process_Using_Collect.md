# Register Tables for Download as a Finish Process using Collect

At the template-role level for a Post role, a Template Administrator can
register tables for download as a Finish process. The Finish process
starts when a user clicks the **Finish** button for a Post role on the
[*Request (Roles)*](../Page_Desc/Request_Roles_H.htm) page.

Additional configuration settings
<span style="font-family: Arial, sans-serif;">set on the *[Template Role
(Finish)](../Page_Desc/Template_Role_Finish.htm)* page and the
*[Template Role (Finish -
Columns)](../Page_Desc/Template_Role_Finish_Columns_H.htm)* page</span>
 allow a Template Administrator to set Collect rules to run on table
data after the download is finished, and to specify filter columns for
both source and target data.

On the *Vertical* View of the *[Template
(Role)](../Page_Desc/Template_Role_H.htm)* page for the Post role, on
the **Approve and Finish Settings** tab, two settings help to facilitate
this functionality: **FinishTables** and **Finish Download in
Background**.

If the **Finish Download In Background** check box is enabled, the data
downloads in the background after the user clicks the **Finish** button
for a Post role on the *Request (Roles)* page.

<span style="font-weight: bold;">NOTE</span>: If the package type to
download data is set to SAP Data Services, it is recommended that the
**Delete Target Table On Build** check box be disabled in Collect on the
<span style="font-style: italic;">[<span style="font-style: italic;">Target
Sources</span>](../../../Platform/Collect/Page_Desc/Target_Sources_H_Collect.htm)</span><span>
page’s </span><span style="font-style: italic;">Vertical</span><span>
View on the Advanced tab. In this case, if the check box is enabled,
dspCompose™ WILL delete every record in the target table during the
Final Finish process (during which data posted in the target ERP system
by the request is downloaded to tables). </span>

This topic contains the following section:

  - [Set Tables to Download](#Set_Tables_to_Download)
  - [Set a Filter Column](#Set_a_Filter_Column)
  - [Enter a Where Clause](#Enter_a_Where_Clause)
  - [Use Custom Syntax](#Use_Custom_Syntax)

## <span id="Set_Tables_to_Download"></span>Set Tables to Download

To set a table for download:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Vertical View** for the Post role.

5.  Click the **Approve and Finish Settings** tab.

6.  Click **Finish Tables**.

7.  Click **Add**.
    
    *[View the field descriptions for the Template Role (Finish)
    page.](../Page_Desc/Template_Role_Finish.htm)*
    
    **NOTE**<span style="font-weight: bold;">:</span>If no records
    exist, the page displays in add mode. Otherwise, click **Add**.

8.  Select a Collect source from the **SOURCE** list box.

9.  Select a Collect target from the **TARGET** list box.

10. Select the name of the table to download when the Post role is
    finished from the **TABLE NAME** list box.

11. Select an option in the **RUN RULES AFTER DOWNLOAD** list box, if
    applicable.
    
    **NOTE**: This option determines the Collect rules to run on a table
    after download, when a user with the Post role clicks Finish for the
    request on the <span style="font-style: italic;">Request
    (Roles)</span> page. Options are:
    
      - **All – Run all of the rules**:  If multiple rules are
        registered to the table in Collect, dspCompose™ will run them on
        the table after download in the priority order set on the
        <span style="font-style: italic;">Collect Table (Rule)</span>
        page.
    
      - **None – Do not run any rules:** Though rules are registered to
        the table in Collect, dspCompose™ will not run those rules on
        the downloaded table.
    
      - **NoParametersOnly –** Run only Collect rules that do not
        contain input parameters, such as an Insert rule.
    
      - **ParametersOnly –** Run Collect rules that contain input
        parameters, such as an Update rule.
        
        **NOTE**: The rule(s) must have already been registered and
        activated in Collect.

12. Click <span style="font-weight: bold;">Save</span>.

The **Source Filter Columns** and **Target Filter Columns** icons are
then active.

## <span id="Set_a_Filter_Column"></span>Set a Filter Column

Instead of downloading an entire table in the finish process, a user can
download data in specific columns, set as filter columns.

The Source Filter Columns are a list of columns used to form the where
clause for selecting values from the source.

The Target Filter Columns are a list of columns used to form the where
clause for selecting values to delete from the target before data is
refreshed from the source.

**NOTE**: If no columns are set up, then dspCompose™ downloads the
entire table.

The *[*Template Role (Finish –
Columns)*](../Page_Desc/Template_Role_Finish_Columns_H.htm)* page
displays for both the Source Filter Columns and Target Filter Columns.

A user can also restrict data for download using a where clause. Refer
to [Enter a Where Clause](#Enter_a_Where_Clause) and [Use Custom
Syntax](#Use_Custom_Syntax) for more information.

To set a filter column:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Vertical View** for the Post role.

5.  Click the **Approve and Finish Settings** tab.

6.  Click <span style="font-weight: bold;">Finish</span>**Tables**.

7.  Click **Source Filter Columns** or **Target Filter Columns** for the
    Finish role record.
    
    <span style="font-weight: bold;">NOTE:</span> If no records exist,
    the page displays in add mode. Otherwise, click
    <span style="font-weight: bold;">Add</span>.
    
    *[View the field descriptions for the Template Role (Finish -
    Columns) page's Vertical
    View](../Page_Desc/Template_Role_Finish_Columns_H.htm)*

8.  Select a column name from the **COLUMN NAME** list box, or enter a
    column name to insert a value.
    
    **NOTE**: The COLUMN NAME contains the values to use for the where
    clause.

9.  Select a data source for the column from the **Data Source ID** list
    box.

10. Select a table name of the table that contains the column from the
    **Table Name** list box.

11. Select a mapped value for the column from the **Mapped Value** list
    box.
    
    **NOTE**: If a mapped value is entered, when the Finish process
    runs, dspCompose™ selects all values from the mapped value binding
    on RequestID and RoleID if they exist in the database object and
    will form an IN statement for selection from the Source <span>filter
    column or the</span><span>Target filter column.</span>

12. Enter a value in the **Fixed Value** field to use as the condition
    of the matching value for download.
    
    **NOTE**: Either a Mapped Value or a Fixed Value can be set, not
    both.

13. Click **Save**.

## <span id="Enter_a_Where_Clause"></span>Enter a Where Clause

If a user enters a Where clause, the Where clause will be used verbatim
when either selecting from the source or deleting from the target. If
the Where clause is set, no other fields on the *[*Template Role (Finish
– Columns)*](../Page_Desc/Template_Role_Finish_Columns_H.htm)*page need
be set and all other fields, if set, will be ignored.

**NOTE**: The Where clause takes precedence over any other Source and
Target Filter settings.

**NOTE**: The data posted in the target system and downloaded in the
table as part of the finish process both use this Where clause.

To enter a Where clause:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Vertical View** for the Post role.

5.  Click the **Approve and Finish Settings** tab.

6.  Click <span style="font-weight: bold;">Finish</span>**Tables**.

7.  Click **Add**.
    
    *[View the field descriptions for the Template Role (Finish)
    page.](../Page_Desc/Template_Role_Finish.htm)*
    
    **NOTE**<span style="font-weight: bold;">:</span><span>If no records
    exist, the page displays in add mode. Otherwise, click
    **Add**.</span>  

8.  Select a Collect source from the **SOURCE** list box.

9.  Select a Collect target from the **TARGET** list box.

10. Select the name of the table to download from the **TABLE NAME**
    list box.

11. Select **None – Do not run any rules** from the **RUN RULES AFTER
    DOWNLOAD** list box.

12. Click <span style="font-weight: bold;">Save</span><span>.</span>

13. Click **Source Filter Columns** or **Target Filter Columns**
    depending on whether the where clause should be applied to the
    target or source table.

14. Click the **Where Clause Filter** tab.

15. Enter the Where clause in the **Where Clause** field.
    
    **NOTE**: If the package type in Collect tables is set to SAP Data
    Services, add the Client value to the Where clause field. For
    example, add  
    \#ColumnName\# IN (\#Data\#) AND MANDT = 'XXX'  
    where 'XXX' is the value of the specific client.

16. Click **Save**.

## <span id="Use_Custom_Syntax"></span>Use Custom Syntax

The *[*Template Role (Finish –
Columns)*](../Page_Desc/Template_Role_Finish_Columns_H.htm)* page for
the source and target also allows a user to enter custom syntax in the
case that the schema cannot be determined for either the source or the
target. When setting the custom settings, the user must mark the
settings as Custom by enabling the **Custom** check box.

To add custom syntax:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.
2.  Click **Templates** for a team.
3.  Click **Roles** for a template.
4.  Click **Vertical View** for the Post role.
5.  Click the **Approve and Finish Settings** tab.
6.  Click <span style="font-weight: bold;">Finish</span>**Tables**.
7.  Click **Source Filter Columns** or **Target Filter
    Columns**depending on whether the where clause should be applied to
    the target or source table.
8.  Click the **Custom** check box to enable it.
9.  Click **Custom Settings** to expand it.
10. Enter the beginning qualifier, if any, to place around the values in
    the **Beginning Qualifier** field.
11. Enter the ending qualifier, if any, to place around the values in
    the **Ending Qualifier** field.
12. Enter the separator to use for data values in the **Separator**
    field.
13. Enter the format of the Where Statement in the **Where Statement**
    field.

<span style="font-weight: bold;">NOTE:</span> dspCompose™ allows two
dynamic substitution values to be used in the where statement:
\#ColumnName\# is the name of the column. \#Data\# is a comma-separated
list of the data.

**NOTE:** If the package type in Collect tables is set to SAP Data
Services, add the Client value to the Where clause field. For example,
add  
\#ColumnName\# IN (\#Data\#) AND MANDT = 'XXX'  
where 'XXX' is the value of the specific client.
