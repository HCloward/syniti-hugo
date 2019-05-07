+++
title = 'Work List Detail – Tag'
solution = 'Platform'
+++

# Work List Detail – Tag

<div class="use">

Use this page while [Viewing Work List
Details](../Use_Cases/View_Work_List_Details.htm).

</div>

To access this page:

1.  Click the blue tab on the Quick Panel to access the Work List.

2.  Click **Work List Details** on the Page Toolbar; all work list
    details for all Plan Tasks and Work List Items display.

3.  Click the **Tags** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>TAG ID</p></td>
<td><p>Displays the name of the tag assigned to the selected task.</p></td>
</tr>
<tr class="odd">
<td><p>TAG TYPE ID</p></td>
<td><p>Displays the tag type, either Plan, Logic, or Security.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the tag description.</p></td>
</tr>
<tr class="odd">
<td><p>REQUIRE LATE COMMENT</p>
<p> </p></td>
<td><p>Displays an option to indicate if users are required to enter a late comment when finishing a task after the planned finish date. Users finish a task by clicking Next Action on the Work List when a task status is In Progress. Values include:</p>
<ul>
<li><strong>Inherit</strong> – The Require Late Comment setting is inherited from the most granular level in the hierarchy. If the Require Late Comment setting is set to [None], Inherit is used by default. The requirement hierarchy’s most granular level is task, followed by tag, plan and parameter.<br />
Require Late Comment settings set at the task level override those set at any other level. If a task's Require Late Comment setting is set to [None] or Inherit, the task's Require Late Comment setting is inherited from the tag level (provided the tag level does not also have a Require Late Comment setting of [None] or Inherit). If the tag level has a Require Late Comment setting of Inherit or [None], Require Late Comment settings are then inherited at the plan level (provided the plan level does not also have a Require Late Comment setting of [None] or Inherit), and so on.<br />
For example, the Require Late Comment list box has been set to [None] at the parameter level. At the plan level, it has been set to Inherit. At the tag level, the Require Late Comment list box is set to Yes. At the task level, Task A in the Plan has a Require Late Comment setting of Inherit. Task B in the plan has a Require Late Comment setting of No. In this scenario, Task A would have a Require Late Comment setting of Yes. Task B would have a Require Late Comment setting of No.</li>
<li> <strong>Yes</strong> – This task will require a comment when the user clicks Next Action on the Work List after the planned finish date.</li>
<li><strong>No</strong> – This task will not require a comment when the user clicks Next Action on the Work List after the planned finish date.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>REQUIRE COMMENT</p></td>
<td><p>Displays an option to indicate if users are required to enter a comment when finishing a task after the planned finish date. Users finish a task by clicking Next Action on the Work List when a task status is In Progress. Values include:</p>
<ul>
<li><strong>Inherit</strong> – The Require Comment setting is inherited from the most granular level in the hierarchy. If the Require Comment setting is set to [None], Inherit is used by default. The requirement hierarchy’ s most granular level is task, followed by tag, plan and parameter.<br />
Require Comment settings set at the task level override those set at any other level. If a task's Require Comment setting is set to [None] or Inherit, the task's Require Comment setting is inherited from the tag level (provided the tag level does not also have a Require Comment setting of [None] or Inherit). If the tag level has a Require Comment setting of Inherit or [None], Require Comment settings are then inherited at the plan level (provided the plan level does not also have a Require Comment setting of [None] or Inherit), and so on.<br />
For example, the Require Comment list box has been set to [None] at the parameter level. At the plan level, it has been set to Inherit. At the tag level, the Require Comment list box is set to Yes. At the task level, Task A in the Plan has a Require Comment setting of Inherit. Task B in the plan has a Require Comment setting of No. In this scenario, Task A would have a Require Comment setting of Yes. Task B would have a Require Comment setting of No. </li>
</ul>
<ul>
<li><strong>Yes</strong> – This task will require a comment when the user clicks Next Action on the Work List on or before the planned finish date.</li>
<li><strong>No</strong> – This task will not require a comment when the user clicks Next Action on the Work List on or before the planned finish date.</li>
</ul></td>
</tr>
</tbody>
</table>
