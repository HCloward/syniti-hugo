# Configure Project Distribution Filters

Filters are customized at the project distribution level to limit data
contained in rules. Project Distribution filters apply to all rules that
include the specified field(s).

For example, a distribution level filter could be configured to send a
sales report to all plants at a summary level, while another filter
could be configured to send a report with data for a specific plant.

User filters are AND combined with project distribution filters. When
multiple user or project distribution filters are applied across
different columns, these filters are AND combined. If multiple user or
project distribution filters are applied to the same column, these
filters are OR combined. If a user filter and a distribution filter are
applied to the same column, the two filters are AND combined instead of
OR combined. A validation warning will trigger in the corresponding
filter page if this scenario would occur.

To define a filter for a project distribution:

1.  Click<span style="font-weight: bold;"> Information Steward
    Accelerator \> </span>**Project Summary** in the *Navigation* pane.

2.  Click **Distributions** for a project.

3.  Click <span style="font-weight: bold;">Filters</span> for a
    distribution.

4.  If no records exist, the page displays in add mode. Otherwise, click
    Add.
    
    *[View the field descriptions for the Project Distribution Filters
    page](../Page_Desc/Project_Distribution_Filters.htm)*

5.  Enter a filter field in **FIELD** field.
    
    **NOTE:** Users in the project distribution will receive reports
    with data restricted by this filter setting.

6.  Select a value for the comparison operator from **OPERATOR** list
    box.

7.  Enter the value to be compared to Field using Operator in
    **CONSTANT** field.

8.  Click **Save**.
