+++
title = 'Set Design Status'
solution = 'Migration'
+++

# Set Design Status

<div class="use">

Use this page to [Set a Target's Design
Status](Set_the_Design_Status).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span>icon on the
    *[Design](../Page_Desc/Design)* page.
4.  Click the link in the <span style="font-weight: bold;">DESIGN
    STATUS</span> column for the Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p><span style="font-family: Arial, sans-serif;">In Design</span></p></td>
<td><p>Click to set the selected Target's Design Status to In Design.</p>
<p>A Target is in this Design Status, when it has been added and while the Target is being configured. During the In Design phase, all functionality related to adding and designing a Target is available including synchronizing with Map and using SQL AutoGen</p>
<p>When a Target in this status is selected, the Sync to Map icon is enabled.</p></td>
</tr>
<tr class="odd">
<td><p>Design Finished</p></td>
<td><p>Click to set the selected Target's Design Status to Design Finished.</p>
<p>When a Target is in this status, the Target design is complete but has not gone through the migration process. The design is locked down, and no changes are allowed (as in, the Target cannot be edited or deleted). A Target can only move to this status if it is in sync with Map. When this Target is synced with Map, {Target Rules} are added.</p>
<p>Auto Generation in Data Services and in SQL is allowed.</p>
<p>Updates to Business Contacts and Developers are allowed.</p></td>
</tr>
<tr class="even">
<td><p>Complete</p></td>
<td><p>Click to set the selected Target's Design Status to Complete.</p>
<p>When a Target is in this status, the design is locked down, and no changes are allowed. A Target can only move to this status if it is in sync with Map. Auto-generation in Data Services and in SQL is not allowed.</p>
<p>When a Target in this status is selected, the Sync to Map icon is disabled.</p>
<p>Updates to Business Contacts and Developers are allowed.</p></td>
</tr>
<tr class="odd">
<td><p>Inactive</p></td>
<td><p>Click to set the selected Target's Design Status to Inactive.</p>
<p>When a Target is moved to an Inactive status:</p>
<ul>
<li>The Target cannot be edited.</li>
<li>The Target is not pushed to Map for mapping and is not available in Transform when the Sync to Map process runs.</li>
<li>The Target is no longer visible in Map and Construct.</li>
<li>Mappings for the Target that are waiting for approval on the <a href="../../Map/Page_Desc/Mapping_Approval_H">Mapping Approval</a> page are removed from the page.</li>
</ul>
<p>When a Target in this status is selected, the Sync to Map icon is disabled.</p>
<p>Updates to Business Contacts and Developers are allowed.</p></td>
</tr>
</tbody>
</table>
