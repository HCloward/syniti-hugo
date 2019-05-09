+++
title = 'Set Target Dependencies'
solution = 'Migration'
+++

# Set Target Dependencies

Dependencies are used to document the order of execution across Process
Areas and objects within the Wave. Dependencies are set for Target
tables that have a relationship with one or more Target tables.

Tables can have parent and child dependency relationships that are
defined in Target Design.

For example, if Target A is the parent of Target B, data from a field in
Target A must be populated for a corresponding field in Target B. In
this case, Target B has a child dependency with Target A. The fields
that are used in the dependency are defined on the
<span style="font-style: italic;">Target Dependency Relationship</span>
page.

Dependencies are set at the child level. In other words, the selected
Target’s dependency is set in relation to its parent. If the selected
Target is the parent of Target C, this relationship is set for Target C.

View the dependencies for a Target on the
<span style="font-style: italic;">Target Dependency (Children)</span>
and the <span style="font-style: italic;">Target Dependency
(Parents)</span> pages (Design \> Targets \> Vertical View).

<span style="font-weight: bold;">NOTE</span>: All Targets across all
Waves and Process Areas are available for use in a dependency.

<span style="font-weight: bold;">NOTE</span>: If a Target field is used
in a relationship, the field and the Target cannot be deleted.

After a Target dependency relationship has been established, field
dependencies must be added for key fields. These dependencies are then
synced with Map.

To set a parent dependency for a Target table:

1.  Select <span style="font-weight: bold;">Design</span> in the Context
    bar.

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Design](../Page_Desc/Design)* page.

3.  Click the <span style="font-weight: bold;">Dependencies</span> icon
    for a Target.

4.  If no records exist, the page displays in add mode. Otherwise, click
    <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Target Dependencies
    page](../Page_Desc/Target_Dependencies)

5.  Select the table name from the
    <span style="font-weight: bold;">PARENT TARGET ID</span> list box.
    
    **NOTE:** All Targets across all Waves and Process Areas are
    available.
    
    **NOTE:** Multiple relationships can be set for the same parent
    table (as in, multiple fields in the parent table can have a
    dependency with fields in child table(s)).

6.  Click <span style="font-weight: bold;">Save</span>.

7.  Click the <span style="font-weight: bold;">Relationships</span>
    icon.

8.  If no records exist, the page displays in add mode. Otherwise, click
    <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Target Dependency Relationship
    page](../Page_Desc/Target_Dependency_Relationship)

9.  Select a field name in the <span style="font-weight: bold;">PARENT
    FIELD</span> list box.
    
    **NOTE:** All fields in the parent table, active and inactive,
    display in this list.

10. Select a field name in the <span style="font-weight: bold;">CHILD
    FIELD</span> list box.
    
    **NOTE:** All fields in the child table, active and inactive,
    display in this list.

11. Enter a description or notes about the relationship in the
    <span style="font-weight: bold;">DESCRIPTION</span> field.

12. Click <span style="font-weight: bold;">Save</span>.

13. Navigate to the [Target
    Dependencies](../Page_Desc/Target_Dependencies) page.

14. Click the **Find Dependencies** icon on the Page toolbar.

15. Select the dependency.

16. Click **Add**.

When the Target is next synced with Map, the dependency is added.
