+++
title = 'Configure Columns'
solution = 'Platform'
+++

# Configure Columns

Once the object is registered in Common, the way in which columns
display on the *[Results](../Page_Desc/Results)* page can be
configured, such as bolding a field name or adding a page break.

To configure view columns:

1.  Click **Analyze** in the *Navigation* pane.

2.  Click **Duplicates** for Data Source ID.

3.  Select an object.

4.  Click **Columns** on Page toolbar.
    
    **NOTE:** All columns are pulled in by the duplicates view. The
    Order is determined in the view.

5.  If records display on the page, the page opens in Add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Object Columns
    page](../Page_Desc/Object_Columns_H)
    
    **NOTE:** The **KEY** check box is enabled for the key column of the
    table.

6.  Click **DUPLICATE DETECTION** check box for up to five columns.
    
    **NOTE:** If more than five columns are required for duplicate
    detection, use a view to concatenate some columns from the source
    table together to create only five duplicate detection columns. For
    example, to fit an address with a phone number into five columns,
    combine City, Region and Zip into a single field called
    CityStateZip.

7.  Configure how the data displays in the
    <span style="font-style: italic;">[Results](../Page_Desc/Results)</span>
    page using the following settings:
    
      - **Show Name** – Displays the column name.
      - **Bold** – Displays the column in bold. It is recommended that
        only the main column (name, material description, etc.) is bold.
      - **Line Break** – Places a line break after the column. This
        feature allows the five fields to be formatted to fit nicely in
        the
        <span style="font-style: italic;">[Results](../Page_Desc/Results)</span>
        page. For example, a line break would appear after the Name and
        Address fields, but not after the City and Region fields. The
        later fields are typically displayed on the same line in an
        address (City State Zip).

8.  Click **Vertical View** for a column to configure further.

9.  Click **Edit** on Page toolbar.
    
    [View the field descriptions  for the Object Columns page's Vertical
    View](../Page_Desc/Object_Columns_H)

10. Select a value from the **Dictionary ID** list box to associate a
    dictionary (that contains a list of words and synonyms) with the
    column, if applicable.

11. Click **Save**.

12. Configure the sensitivity of duplicate detection matches using the
    following settings:
    
      - **Must Match** – Requires two records to match exactly in order
        to be considered a duplicate, regardless of the boaRank, which
        is the match value returned by the bulk duplicate detection.
        **Must Match** is only available if **Duplicate Detection** is
        enabled for the column.
      - **Allow Synonym** – Indicates that two records may be duplicates
        if the field is not an exact match, but instead is a match based
        on a field dictionary synonym, for example, ST = STREET. The
        **Allow Synonym** check box is only available if a dictionary
        for the column is specified and if **Must Match** is enabled.
    
    **Allow Soundex** – Indicates that two records may be a duplicate if
    the field is a Soundex match rather than an exact match. (A Soundex
    match is a coding standard used for indexing words by sound.)

**NOTE:** Any duplicate pair that does not match (either exactly, as a
synonym or as a Soundex) is not a duplicate detection candidate.
