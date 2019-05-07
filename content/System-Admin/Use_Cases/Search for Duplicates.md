+++
title = 'Search for Duplicates'
solution = 'Platform'
+++

# Search for Duplicates

Duplicate records are searched the same way a key word is searched. The
only difference is the search string is constructed with Duplicate
Detection.

To build the search string, the DSP® extracts the values from each of
the columns that have been enabled for Duplicate Detection. The words
are concatenated together and separated by the OR logical operator. The
search is then performed with this search string just as if it had been
manually entered.

For example, assume a record is being added to the Customers table.
Duplicate Detection has been enabled for the CompanyName column. The
user supplies a company name of Eastern Vacuum Mart. The system converts
the company name to the search string Eastern OR Vacuum OR Mart. All
records matching this search string with a rank higher than the
Duplicate Detection Threshold value is returned. The record itself is
explicitly excluded and the user cannot see the recently-added record
(Eastern Vacuum Mart).

Refer to [Determine the Duplicate Detection
Threshold](Determine%20the%20Duplicate%20Detection%20Threshold.htm) for
more information.
