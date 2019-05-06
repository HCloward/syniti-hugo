# Enable Duplicate Detection

Before Duplicate Detection can be enabled, an index must be created.
Users can perform Duplicate Detection using the same index that is used
for searching or an alternate index. The index must have at least one
column on which Duplicate Detection has been enabled.

Refer to [Build indices for a Data Source for Search and Duplicate
Detection](Build%20Indices%20for%20a%20Data%20Source%20for%20Search%20and%20Duplicate%20Detection.htm),
[Define an Index for Duplicate
Detection](Define%20an%20Index%20for%20Duplicate%20Detection.htm) and
[Add a Column to an Index](Add%20a%20Column%20to%20an%20Index.htm) for
more information.

After Duplicate Detection is enabled, a validation rule named Duplicate
Detection displays in the View list box on the *[Page Validation
Rules](../Page_Desc/Page_Validation_Rules.htm)* page’s *Vertical* View.

To enable duplicate detection for a column:

1.  Select **Admin \> Data Sources** from the *Navigation* pane.
2.  Click the **Index** icon for the data source.
3.  Click the **Columns** icon for the indexed table.
4.  Click **Edit** for the column.
5.  Click **Duplicate Detection** check box.
6.  Click **Save**.

Any number of columns can be used for duplicate detection. For best
results, use only one or two columns. Limiting the number of words that
are compiled into the search string increases performance. The more
words searched, the greater the noise in the search results. Refer to
[Determine Duplicate Detection
Threshold](Determine%20the%20Duplicate%20Detection%20Threshold.htm) for
more information.
