+++
title = 'Object History H'
solution = 'Migration'
+++

# Object History H

[Object History V](#Object_History_V)

<div class="use">

Use this page to [Track Object
History](../Use_Cases/Configure_Object#Track).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane, or select
    <span style="font-weight: bold;">Console</span> in the Context bar.
2.  Select <span style="font-weight: bold;">Elements \> Object</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
3.  Click the <span style="font-weight: bold;">History</span> icon for
    an
Object.

|               |                                                                                                                                    |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Field         | Description                                                                                                                        |
| ID            | Displays the Object identity. Changes are tracked in ascending order, so the higher the number the more recent the change.         |
| OBJECT NAME   | Displays the name of the Object.                                                                                                   |
| Wave          | Displays the name of the Wave that the Object is assigned to.                                                                      |
| Process Area  | Displays the name of the Process Area that the Object is assigned to.                                                              |
| PRIORITY      | Displays the Object’s priority, which is the order the Object displays on the *[Objects](Objects_H)* page’s *Horizontal* View. |
| OBJECT OWNER  | Displays the name of the user registered in the platform who is responsible for the Object.                                        |
| OBJECT STATUS | Displays the overall status of the migration Object, such as In Development, Deferred, or Completed.                               |
| TARGET SYSTEM | Displays the name of the Target system.                                                                                            |
| TARGET TABLES | Displays the Target tables used in the Object.                                                                                     |
| T CODE        | Displays the SAP Transaction Code or the Target System Type transaction code.                                                      |
| VERSION       | Displays the version of the Object. ERP systems allows different versions for recordings.                                          |

 

## <span id="Object_History_V"></span>Object History V

[Object History H](Object_History_H)

<div class="use">

Use this page to [Track Object
History](../Use_Cases/Configure_Object#Track).

</div>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>ID</p></td>
<td><p>Displays the Object identity. Changes are tracked in ascending order, so the higher the number the more recent the change.</p></td>
</tr>
<tr class="odd">
<td><p>Object Name</p></td>
<td><p>Displays the name of the Object.</p></td>
</tr>
<tr class="even">
<td><p>Description</p></td>
<td><p>Displays a brief description of the Object.</p></td>
</tr>
<tr class="odd">
<td><p>Wave</p></td>
<td><p>Displays the name of the Wave that the Object is assigned to.</p></td>
</tr>
<tr class="even">
<td><p>Process Area</p></td>
<td><p>Displays the name of the Process Area that the Object is assigned to.</p></td>
</tr>
<tr class="odd">
<td><p>Priority</p></td>
<td><p>Displays the Object’s priority, which is the order the Object displays on the <em><a href="Objects_H">Objects</a></em> page’s <em>Horizontal</em> View.</p></td>
</tr>
<tr class="even">
<td><p>Data Type</p></td>
<td><p>Displays the type of data represented by the Object. Options include Master Data, Ref/Conditional, and Transactional.</p></td>
</tr>
<tr class="odd">
<td><p>Content Driver</p></td>
<td><p>Displays the name of the group that is driving the contents. Options include Company, Enterprise, and Legal.</p></td>
</tr>
<tr class="even">
<td><p>Spec</p></td>
<td><p>Click <strong>Upload</strong> to upload the specifications document to the web server. If a specifications document has been uploaded, the download icon is available. Click <strong>Download</strong> to download the document from the web server.</p></td>
</tr>
<tr class="odd">
<td><p>Comment</p></td>
<td><p>Displays a user-entered comment about the Object.</p></td>
</tr>
<tr class="even">
<td><p>Load Type</p></td>
<td><p>Displays the method used to load the Object during a Mock Wave. Options include Automatic, Manual or ALE.</p></td>
</tr>
<tr class="odd">
<td><p>RICEFW</p></td>
<td><p>Displays a RICEFW number. RICEFW is a generic industry term for &quot;Reports, Interfaces, Conversions, Extensions, Forms and Workflow.” In the overall Project Plan, Deliverables are often assigned a RICEFW number to identify and track the development progress of that item.  </p>
<p>Conversion Objects are a deliverable, so therefore they may be assigned a RICEFW number by the PMO.</p></td>
</tr>
<tr class="even">
<td><p><span style="font-weight: bold;">Complexity</span></p></td>
<td><p>Displays the complexity for building the Object. This value can be used to evaluate work assignments. Options include Average, Simple or Complex. These options are set on the <em><a href="List_Value_Configuration">List Value Configuration</a></em> page and can be edited. If a Target is created in Map that does not have an assigned Complexity, this value will be passed to Transform to complete the required Complexity field on Transform's <em><a href="../../Transform/Page_Desc/Targets_H">Targets</a></em> page’s <em>Vertical</em> View on the Documentation tab. A user can then update the complexity in Transform.</p></td>
</tr>
<tr class="odd">
<td><p>Approx Volume</p></td>
<td><p>Displays an estimate of the number of records to load for the Object.</p></td>
</tr>
<tr class="even">
<td><p>Legacy Systems</p></td>
<td><p>Displays the user-entered legacy systems.</p></td>
</tr>
<tr class="odd">
<td><p>History Requirements</p></td>
<td><p>Displays the user-entered history requirements.</p></td>
</tr>
<tr class="even">
<td><p>Notes</p></td>
<td><p>Displays user-entered notes about the Object.</p></td>
</tr>
</tbody>
</table>
