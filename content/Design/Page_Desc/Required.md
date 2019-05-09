+++
title = 'Required'
solution = 'Migration'
+++

# Required

<div class="use">

Use this page to [Add Custom Requirement
Settings](../Config/Add_Custom_Requirement_Settings).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Select <span style="font-weight: bold;">Configuration \>
    Required</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p><span style="font-size: 12.0pt;">Description</span></p></td>
</tr>
<tr class="even">
<td><p>REQUIRED</p></td>
<td><p>Displays the Requirement setting, used for reporting. The platform is delivered with the following settings that cannot be edited or deleted.</p>
<ul>
<li><strong>Business Required</strong> – Required to meet a business rule or otherwise meet a business need</li>
<li><strong>Technical Required</strong> – Required by the system</li>
<li><strong>Conditional</strong> – Required depending on certain conditions</li>
<li><strong>Optional</strong> – Not required</li>
</ul>
<p>Custom Requirement settings can be added and edited.</p>
<p>This value displays on the <span style="font-style: italic;"><a href="Target_Fields_H_Target_Design">Target Fields</a></span> page in the REQUIRED list box.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a platform-supplied description of the requirement setting or a user-entered description for custom levels.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the priority of the Requirement setting used for reporting purposes. The lower the number, the higher the priority.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If checked, the Requirement setting is active and can be selected in the REQUIRED list box on the <span style="font-style: italic;"><a href="Target_Fields_H_Target_Design">Target Fields</a></span> page and used on reports.</p>
<p>This check box is enabled and cannot be disabled for Requirement settings installed with the platform.</p>
<p>If unchecked, the custom Requirement setting does not display in the REQUIRED list box on the <span style="font-style: italic;">Target Fields</span> page.</p></td>
</tr>
<tr class="even">
<td><p>DSP SUPPLIED</p></td>
<td></td>
</tr>
<tr class="odd">
<td><p>VALIDATION REQUIRED</p></td>
<td><p>If checked and the field is processed in the Target, the field to which the Requirement setting is assigned must have a validation (stored procedure) written and run against the data stored in the field.</p>
<p>This field is for documentation purposes only and indicates that the stored procedure should be written to validate the data, but doesn’t reflect whether one has been written.</p>
<p>For the Requirement settings Business Required and Technical Required, this check box is checked and cannot be edited.</p></td>
</tr>
</tbody>
</table>
