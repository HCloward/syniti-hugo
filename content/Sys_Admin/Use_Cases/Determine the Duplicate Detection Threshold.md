+++
title = 'Determine the Duplicate Detection Threshold'
solution = 'Platform'
+++

# Determine the Duplicate Detection Threshold

The Search Threshold is used when users perform a search on a page. In
contrast, the Duplicate Detection Threshold is used when searching the
index for duplicate records.

If the duplicate detection process finds a match for a record whose
quality is below the cut-off threshold (expressed as a percentage
value), the match is not stored in the \#Duplicate table.

Both are set on the *[Index
Specifications](../Page_Desc/Index%20Specification%20H.htm)* page. Refer
to [Configure an Index](Configure%20an%20Index.htm) for more information
about setting thresholds.

In general, the Duplicate Detection Threshold should be set higher than
the Search Threshold. The higher the number, the less likely false
positives display. The fewer false positives, the more accurate the
results are.

The number of columns used to construct the Duplicate Detection search
string should affect the threshold setting. If Duplicate Detection has
been enabled on one or two columns, then the default value of 50.00% is
appropriate. The more columns searched, the longer the search string and
the lower the threshold setting. If Duplicate Detection has been enabled
on five columns, a rank of 20.00% may be more effective.

The number of words used to construct the duplicate detection search
string affects the Duplicate Detection Threshold. If duplicate detection
is enabled on five columns, but three of the columns are usually NULL
when the record is created, then the default value of 50.00% may still
be effective. In contrast, if duplicate detection is enabled on two
columns that normally contain ten words each, then the lower value may
be necessary.
