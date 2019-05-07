+++
title = 'Add Relationship Joins to Sources'
solution = 'Migration'
+++

# Add Relationship Joins to Sources

Relationship joins support the automation of rules built for Update Row
Sources within mapping, where rules are automatically created and
registered in Transform. Joins are only required if there is an Update
Row Source AND if rule automation is used. If rules are being manually
created in Transform, relationship joins are not needed.

Add relationship joins between the Add Row and the Update Row Source(s)
where  the Source information and Source criterion are coming from a
table other than the Add Row table being mapped. The join indicates how
the table in the Add Row Source is joined to the table in the Update Row
Source so the update rules can be created and registered in Transform.

Refer to [Update Row Sources Overview](Add_Update_Row_Sources.htm) for
more information.

Relationship joins between Add Row and Update Row Sources are created
automatically if the Add Row Source table has a primary key and the key
also exists on the Update Row Source table. In this case, the left table
in the join is the ST table of the Add Row Source and the right table is
the Rule Source Table.

If the Add Row Source does not have a primary key and/or the primary key
columns on the Add Row Source do not exist on the Update Row Source
database Object, the relationship setting the Rule Source Table to the
ST Table for the Update Row Source is created, but the user must create
the join manually.

For example, if the Add Row Source table is Product (as in, the LEFT
TABLE is stMARC\_AW\_Product), and the Update Row Source table is
ProductInventory (i.e., the RIGHT TABLE is stAW\_ProductInventory), a
join would be set up on the keys between the two tables, the ProductID
field.

<span style="font-weight: bold;">NOTE:</span> The system creates joins
from the Add Row to Update Row Source automatically for matching natural
key fields in the Source system. When joining an Add Row to a Construct
table, the joins are from the zLegacy keys on the Add Row Source table
to the zLegacy keys on the Construct table.

<span style="font-weight: bold;">NOTE:</span> If the relationship is
being used in a field mapping, the relationship cannot be deleted until
it is removed from the field mapping.

To add relationships to a Source in Map:

1.  Click **ProcessArea** in the *Navigation* pane.

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)* page.

3.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

4.  Click the **Update Row Sources** icon for a Source.

5.  Click the <span style="font-weight: bold;">Secondary Source</span>
    icon for an Add Row Source.

6.  Click the **Relationships** icon for the Add Row Source.

7.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    [View the field descriptions for the Relationship Joins
    page](../Page_Desc/Relationship_Joins_H.htm)

8.  Enter name of relationship in **NAME** field, for example, Product
    Inventory.

9.  Enter name of Source table in **RIGHT TABLE** field, for example,
    ProductInventory.

10. Click **Save**.

11. Click **Vertical View** for the relationship join to add a WHERE
    clause.
    
    **NOTE:** Enter a WHERE clause, if necessary, to apply the join
    correctly during auto-generation.

12. Click **Edit**.
    
    [View the field descriptions for the Relationship Joins
    page](../Page_Desc/Relationship_Joins_H.htm)

13. Enter a filter in **Where Clause** field.

14. Click **Save**.

15. Close the <span style="font-style: italic;">Vertical</span> View.

16. Click the **Fields** icon.

17. If no records exist, the page displays in Add mode. Otherwise, click
    **Add**.
    
    [View the field descriptions for the Relationship Fields
    page](../Page_Desc/Relationship_Fields.htm)

18. Enter the priority used to build the join in the **PRIORITY** field.

19. Select name of the table on the left of the join from the **LEFT
    TABLE** list box, for example, stMARC\_AW\_Product.
    
    **NOTE:** The LEFT TABLE must exist in the Object's database (when
    processed) since this is the database where the joins are generated
    and executed. By default, this is the ST table of the Add Row
    Source.

20. Select the name of the field in the LEFT TABLE from the **LEFT
    FIELD** list box, for example, ProductID.

21. Select the name of the table on the right of the join from the
    **RIGHT TABLE** list box, for example, stAW\_ProductInventory.
    
    **NOTE:** The RIGHT TABLE must exist in the Object's database (when
    processed) since this is the database where the joins are generated
    and executed. Update Row views are created when the Update Row is
    added to the Add Row Source if the table doesn’t exist. It is
    defaulted to the Rule Source Table.

22. Select the name of the field in the RIGHT TABLE from the **RIGHT
    FIELD** list box, for example, ProductID.

23. Click <span style="font-weight: bold;">Save</span>.
