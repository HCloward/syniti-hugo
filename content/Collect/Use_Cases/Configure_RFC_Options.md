+++
title = 'Configure RFC Options'
solution = 'Platform'
+++

# Configure RFC Options

Before performing this task:

  - [Register Tables to Source](Register_Tables_to_Source)
  - [Encrypt Columns](Encrypt_Columns)

RFC options enable the configuration of a table using an RFC and are
available by field name for conditional data downloads. This feature
serves as a Where Clause to limit data read from the tables. In order to
configure the RFC options, the Package Type for the table must be set to
BOA RFC using Options and the BackOffice  transports must be installed.
Refer to the project team lead to verify the transport files are
installed.

To configure RFC
Options:

1\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">    </span> Click
**Tables** in *<span style="font-size: 11.0pt;">Navigation</span>*
pane.

2\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">    </span> Click
**Vertical View** for a table where the Package Type is **BOA RFC using
Options**.

3\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">    </span> Click
**Action**
tab.

4\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">    </span> Click
**Options**.

5\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">    </span> Click
**Add**.

[View the field descriptions for the Table (Rfc Options)
page](../Page_Desc/Table_Rfc_Options)

6\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">    </span> Update
**PRIORITY** field if the default value is not
applicable.

<span style="font-weight: bold;">NOTE:</span><span>The</span><span style="font-weight: bold;">PRIORITY</span>
field controls the sort order of column
fields.

7\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">    </span> Select
a field name from **FIELD** list
box.

8\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">    </span> Update
**SIGN** list box if the default value is not
applicable.

<span style="font-weight: bold;">NOTE:</span><span>The</span><span style="font-weight: bold;">SIGN</span>
field controls whether the value is included or excluded for the
field.

9\.<span style="font: 7.0pt &#39;Times New Roman&#39;;">    </span> Update
**OPTION** list box if the default value is not applicable.

<span style="font-weight: bold;">NOTE:</span> The
<span style="font-weight: bold;">OPTION</span> field controls the
relationship between values.

10\.<span style="font: 7.0pt &#39;Times New Roman&#39;;"> </span> Enter
a value in **LOW** field.

**NOTE:** The <span style="font-weight: bold;">LOW</span> field is the
search value of the request.

11\.<span style="font: 7.0pt &#39;Times New Roman&#39;;"> </span> Enter
a value in **HIGH** field if a high range is needed.

**NOTE:** If using a between clause, both LOW and HIGH fields must be
populated.

12\.<span style="font: 7.0pt &#39;Times New Roman&#39;;"> </span> Select
a value from **OPERATOR** list box.

13\.<span style="font: 7.0pt &#39;Times New Roman&#39;;"> </span> Select
a type from **ABAP TYPE** list box.

**NOTE:** The <span style="font-weight: bold;">ABAP TYPE</span> controls
the type of data that was entered in the LOW and HIGH fields.

14\.<span style="font: 7.0pt &#39;Times New Roman&#39;;"> </span> Click
**Save**.
