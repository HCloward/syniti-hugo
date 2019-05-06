# Synchronize Target Designs Across Waves

A Migration Developer can compare the target design across Waves,
identifying differences between Waves and synchronizing a baseline Wave
with one or more child Waves. They can also sync target designs at the
Process Area, object, target or field level across Waves, making target
design a global, efficient and streamlined process.  

Once the comparison is processed, the differences between elements in
the compared Waves display on the
<span style="font-style: italic;">Vertical</span> View of the results
page at each element level. Comparisons list any elements that exist in
one Wave but not the other and field changes (add, update or delete)
that are in one Wave and not the other.

To make comparisons easier to review, hide all matching comparisons
(i.e., those comparisons that do not need to be synced) using the Hide
Identical icon on the Page toolbar at each element level.

The appearance of comparison colors is controlled on the
<span style="font-style: italic;">[Parameters](../Page_Desc/Parameters.htm)</span>
page in Console and can be updated. For example, by default, values that
are in sync display in orange, but can be updated.

The status icon on the
<span style="font-style: italic;">Horizontal</span> View of each results
page provides a summary of the comparison. Hover a cursor over this icon
for details.

Synchronizations can be performed for all migration elements or for a
single element (i.e., all Process Areas in a Wave or a selected Process
Area). To sync Target Designs, the user either clicks the Sync All
\[Element Name\] in the page toolbar, or selects a record and selects
Sync \[Element Name\] in the Page toolbar.

**NOTE**: A user must be assigned to Console's Wavesynchronizer WebApp
group in System Administration or granted security through a security
role to access the icon and pages related to synchronizing target
designs.

At a high level, to compare and synchronize target designs, the
Migration Developer:

1.  Selects the baseline Wave and child Wave and runs the comparison
    process.
2.  Reviews the differences between the Waves at any level of the
    migration hierarchy.
3.  Syncs the target designs between the baseline and child Wave at the
    element level or at the single record level.

To compare target designs in Console:

1.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">dspMigrate</span>
    in the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Navigation</span>
    pane, or click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Console</span>
    in the Context bar.

2.  Select the baseline Wave and click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Build
    Comparison</span> icon in the Page toolbar on the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">[Waves](../Page_Desc/Waves_H.htm)</span>
    page.

3.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Add</span>
    in the *Build Wave Comparison* page in the child pane.
    
    [View the field descriptions for the Build Wave Comparison
    page](../Page_Desc/Build_Wave_Comparison.htm)

4.  Select the child Wave to compare to the baseline Wave in the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Wave
    ID</span> list box.  

5.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Save</span>.

6.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Process</span>
    icon on the Page toolbar.

Click the icon corresponding to the level in the migration hierarchy to
compare the baseline Wave with the child Wave.

Once the comparison is processed, the differences between elements in
the compared Waves display on the
<span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Vertical</span>
View of the results page at each element level. For example, to view the
comparison results for a target, on the
<span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">[<span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Build
Wave Comparison</span>](../Page_Desc/Build_Wave_Comparison.htm)</span>
page, click the **Targets** icon, then click the**Vertical** **View**
icon for a target.

For example, a user compares a baseline Wave and a child Wave that both
contain material data. On the
<span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">[Wave Compare Process Area
Results](../Page_Desc/Wave_Compare_for_Process_Area_Results_H.htm)</span>
page, the Process Areas are named the same but have different data
sources. The user does not want to synchronize the data sources, so
continues the review at the object level.

The Material object name is also shared by both Waves and does not need
to be synced.

At the target level, both Waves contain the ttMARA target, so the user
clicks the Hide Identical icon in the page toolbar and these targets
that do not need to be synced no longer display. The ttADRC target
exists in one Wave and not the other. The user views this detail by
hovering over the Status icon on the *Horizontal* View of the *[Wave
Compare for Target
Results](../Page_Desc/Wave_Compare_for_Target_Results.htm)* page for the
record. The user selects the ttADRC record and clicks the Sync Target
icon on the Page toolbar to sync the targets in both Waves.
