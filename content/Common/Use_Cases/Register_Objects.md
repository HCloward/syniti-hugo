# Register Objects

Objects are views or tables that contain data analyzed for duplication.

To register an object:

1.  Select **Common \> Analyze** in the *Navigation* pane.
    
    **NOTE**: The *[Analyze](../Page_Desc/Analyze.htm)* page displays
    data sources registered in System Administration that are not added
    to the *[Ignore Data Sources](Ignore_Data_Sources.htm)* page and to
    which the logged in user has security to view. Data sources are
    analyzed for database object changes, table statistics and duplicate
    records.

2.  Click **Duplicates** for DATA SOURCE ID.
    
    **NOTE**: If no records exist, the page automatically displays in
    add-mode. Otherwise, click Add.
    
     *[View the field descriptions for the Objects
    page](../Page_Desc/Objects_H_Common.htm)*

3.  Enter an object name in **Object** field.

4.  Select a view from <span style="font-weight: bold;">View Name</span>
    list box. This is the view created in [Create Object
    Views.](Create_Object_Views.htm)

5.  Update **Search ID** field if default value is not applicable.
    
    **NOTE**: The Search ID is the name of the search table that
    controls which record pairs in the source data are stored as a
    duplicate. The DSP® is delivered with a default search table,
    DSPCommon.ttDuplcate, that has been set up for the BDD process.
    
    **NOTE**: If a search table other than DSPCommon.ttDuplicate is to
    be used, it must be set up in System Administration.

6.  Update **Non Searchable Characters** field if default value is not
    applicable.
    
    **NOTE**: The Non Searchable Characters field controls characters
    excluded from the duplicate detection search.

7.  Select ID from **Stop List Id** list box to control list of words
    ignored during duplicate detection process.
    
    **NOTE**: The Stop List ID field indicates a list of words ignored
    during the duplicate detection search. Stop Lists are managed in
    System Administration.

8.  Update **Search Threshold** field if default value is not
    applicable.
    
    **NOTE**: The Search Threshold field controls the level to ignore
    false positives.

9.  Update **Duplicate Detection Threshold** field if default value is
    not applicable.
    
    **NOTE**: The Duplicate Detection Threshold field controls the
    weight percent of the calculated value for matched words. Words that
    match carry more weight than words that sound alike.

10. Update **Synonym Weight** field if default value is not applicable.
    
    **NOTE**: The Synonym Weight field controls the weight value of
    synonym matches.

11. Update **Sound Ex Weight** field if default value is not applicable.
    
    **NOTE**: The Sound Ex Weight field controls the
    <span style="background: #ffffff;">percentage of combined calculated
    value for words found within the search (number of words found plus
    the number of words that sound alike divided by the total number of
    words). Words that match carry more weight than words that sound
    alike.</span>

12. Select ID from **Custom Sound Ex Function ID** list box if a custom
    SQL Server Sound Ex function is used.
    
    **NOTE**: Update Index Batch Size field if default value is not
    applicable. The Index Batch Size field controls the number of
    records to process in one pass through the data

13. Update **Duplicate Detection Batch Size** field if default value is
    not applicable.
    
    **NOTE**: The Duplicate Detection Batch Size field controls
    the number of records queued up in the duplicate detection process.
    This field allows a subset of large files to be processed and at the
    same time, limits the resources required.

14. Update **Word Ratio Threshold** field if default value is not
    applicable.
    
    **NOTE**: The Word Ratio Threshold field controls the number of
    words in each duplicate pair. A value less than 50% marks a
    duplicate value for removal.

15. Click **Remove Blank Lines** check box to enable it, removing blank
    lines from the HTML formatted output, which displays on the
    Candidates page.

16. Click **Unicode Separate Characters** check box to indicate Unicode
    characters (double-byte) are included.

17. Click **Save**.
