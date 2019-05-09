+++
title = 'Configure Filters in the DSP®'
solution = 'Platform'
+++

# Configure Filters in the DSP®

Filtering a result set refers to the process of limiting the number of
records processed by the DSP®. A filter removes records from the page
that do not meet the user-defined criteria, which limits the number of
records displayed or downloaded. Filters can be applied to the
*Horizontal* View for dynamic pages, report pages, columns with a
control type of List Box or Text Box, and downloads.

Filtering a record set produces noticeable performance improvements and
limits the amount of data transferred between the SQL Server and the web
server. This limitation decreases the processing time for the request
and the size of the active web page. Filtering makes large data sets
more manageable by excluding unwanted records from the results.

By default, any DSP® page displaying a horizontal grid can be filtered.
To launch the Filter View, click the Filter button on the Toolbar. The
Filter button is active for all pages that contain records.

The Filter View displays a row for each column that can be filtered in
the *Horizontal* View. Reserved columns, such as the Edit, Validation
and Delete, are excluded from the filter.

The column control types used on the Filter View are not always the same
as those used on the *Horizontal* View. Instead, the Filter View
determines the appropriate filter control based on the default column
property. If a default column property is not defined, then the DSP®
overrides the control type from the underlying SQL data type of the
column.

Refer to [Filter Controls]() for more information.

An Administrator can:

  - [Hide Columns on a Page’s Filter
    View](Hide%20Columns%20on%20a%20Pages%20Filter%20View)

  - [Display Fields as List
    Boxes](Display%20Fields%20as%20List%20Boxes%20on%20a%20Pages%20Filter%20View)

  - [Set the Wildcard Character for a
    Filter](Set%20the%20Wildcard%20Character%20for%20Filters)
