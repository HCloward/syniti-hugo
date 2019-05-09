+++
title = 'BDC Screen Conditionals'
solution = 'Platform'
+++

# BDC Screen Conditionals

<div class="use">

Use this page to [Configure a Conditional for a BDC
Screen.](../Use_Cases/ConfigureConditionalBDCScrn)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Integrate \>
    Categories</span> from Navigation pane.
2.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a category.
3.  Locate the template with a type of<span style="font-weight: bold;">
    BDC Script</span>.
4.  Click<span style="font-weight: bold;"> Vertical View</span>.
5.  Click <span style="font-weight: bold;">Configuration</span> tab.
6.  Click <span style="font-weight: bold;">BDC Screen</span> icon.
7.  Click <span style="font-weight: bold;">Vertical View</span> for a
    screen.
8.  Click the <span style="font-weight: bold;">Conditionals</span> icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>CONDITIONAL FIELD NAME</p></td>
<td><p>Displays the name of the field returned from the BDC script that should have the data condition. Only one conditional can be configured per BDC screen. If the data condition is true, the resulting posting script includes the data from the process template field mappings associated with the screen.  If the data condition is false, the screen will be left out of the posting script. Each conditional is data-record specific so that if 10 records are posted, Integrate evaluates the conditional for each data record and applies it to the data in that record only.  If there is no conditional applied to a screen, the posting script includes the screen.</p></td>
</tr>
<tr class="odd">
<td><p>CONDITIONAL TYPE</p></td>
<td><p>Displays the operator for the condition. Values are:</p>
<p>Less Than  &lt; , Less Than or Equals  &lt;= , Not Equal  &lt;&gt; , Equals  = , Greater Than  &gt; , Greater Than or Equals  &gt;= , Between, Contains, Ends With, Starts With.</p></td>
</tr>
<tr class="even">
<td><p>CONDITIONAL VALUE</p></td>
<td><p>Displays the value used by the condition.</p></td>
</tr>
</tbody>
</table>
