+++
title = 'Configure an Index'
solution = 'Platform'
+++

# Configure an Index

When creating an index, the default search engine index settings serve
as a guideline for general purpose searching and foreground duplicate
detection. An Administrator can optimize the settings for bulk duplicate
detection to improve performance and accuracy.

**NOTE**: If both search and duplicate detection are used, the user can
enable a validation as a page event that runs in the foreground to check
for duplicates when a single record is added.

Before performing this task, [Create an Index](Create%20an%20Index.htm).

Refer to [Build Indices for a Data
Source](Build%20Indices%20for%20a%20Data%20Source%20for%20Search%20and%20Duplicate%20Detection.htm)
for general information.

**NOTE**: The following steps outline search engine indexing parameters
that are available when tuning the index for Bulk Duplicate Detection.
If any of the parameters are changed, the index must be rebuilt by
dropping and creating the tables on the *Vertical* View of the *[Index
(Specification)](../Page_Desc/Index%20Specification%20H.htm)* page.

To configure an index:

1.  Select **Admin \> Data Sources** in the *Navigation* pane.

2.  Click the **Index** icon for a data source.

3.  Click **Vertical View** for an index.

4.  Enter characters to omit during a search in the **Non Searchable
    Characters** field.
    
    **NOTE**: Non-searchable characters are stripped from column values
    during the index process and are not stored in the index. This
    process decreases the index size, which in turn, reduces size
    requirements for the index table and improves performance.
    
    By default, the list of non-searchable characters contains
    punctuation and numbers. Such characters may not be optimal when
    performing duplicate detection against some types of data.
    
    For instance, if the search engine index contains street addresses
    and P.O. Boxes, more accurate results may be achieved if numbers
    from the list of non-searchable characters are removed. Removing
    numbers increases the size of the index and decreases performance of
    the Bulk Duplicate Detection process.

5.  Select a stop list from the **Stop List ID** list box.
    
    **NOTE**: A Stop List is a list of words that is ignored during
    indexing and searching. Stop lists are generally used to strip out
    prepositions, conjunctions, adjectives, adverbs and other common
    words because these words increase the index size and add
    unnecessary items to the search results. Refer to [Create Stop
    Lists](Create_Stop_Lists.htm) for more information.

6.  Enter a percentage in the **Search Threshold** field.
    
    **NOTE**: Each match in the search results is assigned a similar
    percentage value. Records with a value beneath the Search Threshold
    do not display in the search results.

7.  Enter a percentage in the **Duplicate Detection Threshold** field.
    
    **NOTE**: If the duplicate detection process finds a match for a
    record whose quality is below the cut off threshold (expressed as a
    percentage value), the match is not stored in the \#Duplicate table.
    
    The Duplicate Detection Threshold can be used to adjust bulk
    duplicate detection. When a record is inserted or updated, lower
    quality matches at the bottom of the list can be ignored. When
    performing Bulk Duplicate Detection, the results may need to be
    trimmed by increasing the threshold to improve performance and to
    reduce the size of the \#Duplicate table.

8.  Enter a percentage in **Synonym Weight** field.
    
    **NOTE**: The search functionality supports synonyms, which are
    added to dictionary words. For example, the word "Street" could have
    the synonym "St." Generally speaking, a synonym match counts less
    than an exact match; Synonym Weight controls how much less. For
    example, if the Synonym Weight is set to 0.50, a synonym match
    counts for half of an exact match.

9.  Enter a percentage in **Sound Ex Weight** field.
    
    **NOTE**: Sound Ex Weight is the percentage of the combined
    calculated value for words found within the search. Words that match
    carry more weight than words that sound alike. Ranking is determined
    by the number of words found (ranking 1) plus the number of words
    that sound alike (less than 0.5, for example) divided by the total
    number of words.

10. Select a value from **Custom Sound Ex Function** list box.
    
    **NOTE**: Options are:
    
      - **Enhanced SoundEx routine** – Based on the metaphone family of
        algorithms and is provided for backwards compatibility.
      - **Faster Version of SoundEx** – Based on the metaphone family of
        algorithms and runs faster than Enhanced SoundEx routine.
    
    **NOTE**: Both Custom Sound Ex Function options result in similar
    matches. The built in SQL Server SOUNDEX() function is based on the
    original Russel-Odell algorithm. This algorithm has weaknesses with
    pluralizations and character sequences. The alternative algorithms
    provided here improve accuracy, but consequently slows down
    performance.

11. Enter a number in the **Index Batch Size** field.
    
    **NOTE**: The Index Batch Size controls the number of records that
    are indexed at one time. On large tables (hundreds of thousands to
    millions of records), the system generally does not have enough
    resources to index all the records at one pass. Records are indexed
    in batches of the specified size until there are no more records to
    index. On a system with limited resources, keep the Index Batch Size
    value low, less than 40,000.

12. Click **Save**.

Continue with [Add a Column to an
Index](Add%20a%20Column%20to%20an%20Index.htm).
