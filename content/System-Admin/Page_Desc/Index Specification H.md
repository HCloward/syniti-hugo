# <span id="top"></span>Index (Specification) H

[Index (Specification) V](#Index)

<div class="use">

Use this page to:

  - [Create an Index](../Use_Cases/Create%20an%20Index.htm)
  - [Configure an Index](../Use_Cases/Configure%20an%20Index.htm)
  - [Build Index Objects](../Use_Cases/Build%20Index%20Objects.htm)

</div>

To access this page:

1.  Select **Admin \> Data Sources** in the *Navigation* pane.
2.  Click the **Index** icon for a data source.

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
<td><p>Build</p></td>
<td><p>Click to build the index tables and stored procedures for indexing.</p>
<p>Before a table can be indexed, the objects must be built based on the index configuration. Building the index objects is generally a one-time event. If the index configuration changes, the objects must be rebuilt.</p>
<p><strong>NOTE</strong>: An index cannot be built until a searchable column has been defined for the index on the <em><a href="Index%20Columns.htm">Index Columns</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the selected table's indices that are active are fully indexed by a service page that runs once daily.</p>
<p>If disabled, the index is not used.</p></td>
</tr>
<tr class="even">
<td><p>TABLE</p></td>
<td><p>Displays the name of the table that is indexed.</p></td>
</tr>
<tr class="odd">
<td><p>Columns</p></td>
<td><p>Click to open the <a href="Index%20Columns.htm">Index Columns</a> page to set the columns that contain the data to be indexed.</p></td>
</tr>
</tbody>
</table>

## <span id="Index"></span>Index (Specification) V

[Index (Specification) H](#top)

<div class="use">

Use this page to [Configure an
Index](../Use_Cases/Configure%20an%20Index.htm).

</div>

Field

Description

Tables

Table

Displays the name of the table that is indexed.

Index Table

Displays the name of the index table (the nonclustered index) created
for the database table.

The \#Search table is the reverse index for the table and associates
individual words with records. A word is paired to a record once. If the
word appears in the record more than once, a count is reflected in the
Occurrences column. The IsSynonym column designates whether the word
appears in the record or whether a synonym of the word appears in the
index.

Index Word Table

Displays the name of the index word table (the nonclustered index)
created for the database table.

Every unique word in the source table contains a record in the
\#SearchWord table. In addition to the word, a pre-computed SoundEx
value is stored with the word. The word is assigned an ID, boaIndexID,
which is a SQL Server IDENTITY column.

Settings

Non Searchable Characters

Displays characters excluded from the index. Non-searchable characters
are stripped from column values during the index process and are not
stored in the index. This process decreases the index size, which
reduces size requirements and improves performance.

By default, the list of non-searchable characters contains punctuation
and numbers. Such characters may not be optimal when performing
duplicate detection against some types of data.

For instance, if the search engine index contains street addresses and
P.O. Boxes, more accurate results may be achieved if numbers from the
list of non-searchable characters are removed. Removing numbers
increases the size of the index and decreases performance of the Bulk
Duplicate Detection process.

Search Word Limit

Displays maximum number of words to index out of each column during
search indexing. Default value is 64.

Stop List ID

Displays the name of the stop list used in this index. A stop list is a
list of words (such as prepositions, conjunctions, adjectives and
adverbs) that is ignored during indexing to improve performance and
accuracy.

Refer to [Create Stop Lists](../Use_Cases/Create_Stop_Lists.htm) for
more information.

Search Threshold

Displays the percentage value that is used to filter out possible false
positives, both in Search and Duplicate Detection. Each search match has
a percentage rank against the existing data. If the number of results
seems high for data sets with many words, increasing the match threshold
will remove the lower ranked matches.

The default value for Search Threshold is 25.00%

Duplicate Detection Threshold

Displays weight percent of the calculated value for matched words. Words
that match carry more weight than words that sound alike.

If the duplicate detection process finds a match for a record whose
quality is below the cut off threshold (expressed as a percentage
value), the match is not stored in the \#Duplicate table. The default
value is 50.00%

The Duplicate Detection Threshold can be used to adjust bulk duplicate
detection. When a record is inserted or updated, lower quality matches
at the bottom of the list can be ignored. When performing Bulk Duplicate
Detection, the results may need to be trimmed by increasing the
threshold to improve performance and to reduce the size of the
\#Duplicate table.

Refer to Find Duplicates Overview in Common help for more information.

Synonym Weight

Displays weight value of synonym matches. In a synonym match, two
records may be duplicates if the field is not an exact match, but
instead is a match based on a field dictionary synonym, for example, ST
= STREET. Generally speaking, a synonym match should count less than an
exact match, and this value controls how much less. For example, if the
weight is set to 0.50, a synonym match counts for half of an exact
match.

Refer to [Create Dictionaries](../Use_Cases/Create_Dictionaries.htm) for
more information about synonyms.

Sound Ex Weight

Displays the percentage of the combined calculated value for words found
within the search (number of words found plus the number of words that
sound alike divided by the total number of words). Words that match
carry more weight than words that sound alike. Ranking is determined by
the number of words found (ranking 1) plus the number of words that
sound alike (less than 0.5, for example) divided by the total number of
words. The default value is 50.00%.

Custom Sound Ex Function ID

Displays ID for custom SQL Server Sound Ex function. Selecting a custom
function improves accuracy of duplicate detection, but consequently,
decreases performance.

Options are:

  - **Enhanced SoundEx routine** - Based on the metaphone family of
    algorithms and is provided for backwards compatibility.
  - **Faster Version of SoundEx** - Based on the metaphone family of
    algorithms and runs faster than Enhanced SoundEx routine.

**NOTE**: Both Custom Sound Ex Function options result in similar
matches.

Index Batch Size

Displays number of records that are indexed at one time.

On large tables (hundreds of thousands to millions of records), the
system generally does not have enough resources to index all the records
at one pass. Records are indexed in batches of the specified size until
there are no more records to index. On a system with limited resources,
keep the Index Batch Size value low (less than 10,000).

Default value is 1000.

Bulk Duplicate Detection

Duplicate Detection Batch Size

Displays number of records queued up in the duplicate detection process.
This field allows a subset of large files to be processed and at the
same time, limits the resources required.

Duplicate Detection Require Columns

If enabled, a duplicate detection match must have at least one word for
each searched column. Duplicate detection builds a keyword search string
based on words from search columns in a given record. Key words are then
used to find similar records. Regardless of this setting, a threshold is
still applied.

Create Tables

Click to create the work tables required by the bulk duplicate detection
process. This button is disabled after the tables are created.

Drop Tables

Click to remove the work tables from the database.
