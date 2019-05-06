# GUI Script Conditionals

<div class="use">

Use this page to [Configure Conditional GUI Script Data
Records](../Use_Cases/ConfigureConditionalGUIScriptDatarec.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Integrate
    \></span><span style="line-height: normal;">**Categories** on *Navigation
    pane*.</span>
2.  Click the **Templates** icon for a category.
3.  Click **Vertical View** for a template based on a GUI script.
4.  Click **Configuration** tab.
5.  Click the GUI Script Data icon.
6.  Click **Vertical View**for a data record.
7.  Click **Conditionals** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>CONDITIONAL FIELD NAME</p></td>
<td><p>Displays the name of the field returned from the GUI script that should have the data condition. Only one conditional can be configured per GUI data record. If the condition is true, the resulting posting script includes the data from the process template field mappings associated with the script.  If the data condition is false, the record will be left out of the posting script. Each conditional is data record specific so that if 10 records are posted, the conditional will be evaluated for each data record and applied to the data in that record only.  If there is no conditional applied to a script, the posting script includes the data record.</p></td>
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
