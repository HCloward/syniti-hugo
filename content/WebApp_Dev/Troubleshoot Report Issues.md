+++
title = 'Troubleshoot Report Issues'
solution = 'Platform'
+++

# Troubleshoot Report Issues

### Error Messages

If an error occurs, begin troubleshooting by determining which pages are
involved. For example, if the *Customers* page links to the **Orders**
page, and the *Orders* page links to the **Order Details** page, then
the error may have occurred on any of these pages. Dynamic views can
change which links appear on a given page.

Once the pages have been identified, determine which views are being
used to build the report. The page can have a report view and that view
overrides the *Horizontal* or *Vertical* View. Reporting honors dynamic
views. From within SQL Server Query Analyzer or Management Studio, test
the views by selecting all the records from each view.

If a page has a report view, ensure that it contains all the necessary
columns. An error can occur if the page has an Order By statement that
references a column that is not in the report view. Refer to [Create
Report Views](Create%20Report%20Views) for more information.

### Performance

Reporting is resource intensive. Almost by definition, reports contain
more data than any given Dynamic page. This is why DSP® has two separate
properties to control the maximum number of records per page, one for
Dynamic pages and one for Report pages. These parameters are
configurable on the
*[Parameters](../Sys_Admin/Page_Desc/Parameters_All_TabsSysAdmin)*
page on the Search Options tab. The default display limit is 1000; the
default report limit, 10,000. Consider lowering these values from their
defaults.

In addition to the data set size, the number of sub-requests issued by
the report generator can create a bottleneck. The report generator
interacts with DSP® in much the same way as clicking links. However, it
typically makes many more requests than a user in a shorter time span.

A page can contain hundreds of records and each record can link to
another page, resulting in hundreds of requests built to a single
report. If the down-level page then links to another page, thousands of
requests can be required to get the data. Requests are serial. If each
request takes a second, then generating the final report can take
minutes or hours.

One way to bypass this situation is to take links out of the equation.
Instead of using links, build a single report view and register it at
the top-level page. Use report groups to organize the data. Instead of
issuing hundreds or thousands of small requests, the report generator
issues one request. Issuing one request that retrieves and organizes a
large data set is usually much faster than issuing many small requests.

Finally, it may not be possible to generate a report for a thousand
customers that include all customer orders and order line items. For
situations like this, consider disabling page level reports (i.e.,
disable the Support Report page property). Use the boaReport or Link To
Report features to allow users to generate record-level reports. This
practice allows users to generate a report for individual customers
rather than a report that contains all customers.
