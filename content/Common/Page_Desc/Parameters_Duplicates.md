+++
title = 'Parameters – Duplicates'
solution = 'Platform'
+++

# Parameters – Duplicates

<div class="use">

Use this page to [Configure Duplicates
Parameters.](../Use_Cases/Configure_Duplicates_Parameters.htm)

</div>

To access this page, click <span style="font-weight: bold;">Common \>
Configuration \> Modules \> Parameters – Duplicates</span> in the
*Navigation* pane.

Field

Description

Application Information

Version

Displays current release version of the component, Duplicates. .

Date

Displays date when the component version was released.

Default Values

Search ID

Displays ID associated with the duplicate search table
(DSPCommon.ttduplicate ).

Duplicate Detection Threshold

Displays weight percent of the calculated value for matched words. Words
that match carry more weight than words that sound alike.

Word Ratio Threshold

Displays number of words in each duplicate pair. A value less than 50%
marks a duplicate value for removal. For example, if A has 10 words and
B has 1 word, which matches on one of A’s words, then A-B matches 10%
but B-A matches 100%. This 100% is the false positive; the Word Ratio
will remove this as a potential match

Stop list ID

Displays ID for list of words ignored during the duplicate detection
process.

Remove Blank Lines

Click to remove blank lines from the HTML formatted output on the
*[Candidates](Candidates.htm)* page. This action makes each object block
smaller as white space is removed. When comparing objects with multiple
lines, such as address data, multiple lines may cause the data to not
line up on the page. If needed, the Remove Blank Lines check box can be
disabled and the object can be re-built.
