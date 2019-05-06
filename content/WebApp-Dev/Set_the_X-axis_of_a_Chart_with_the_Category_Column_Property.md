# Set the X-axis of a Chart with the Category Column Property

The Category column property allows the user to define which column in
the web\*Chart view corresponds to the X-axis. This column property can
be used for most data types; the exception is binary data types. As with
list boxes, a non-string key column can be used as the underlying value
and a display value can replace what is shown.

There are two types of categories: Primary and Secondary. Each
combination of Primary and Secondary Category values must be unique to
ensure a proper rendering of the dataset.

A **Primary** Category column corresponds to the field whose data is
rendered on the X-axis. If there is only one Category column defined (by
definition, it must be Primary), each value row’s primary column field
is rendered on the X-axis. There must be one Primary Category column per
non-tabular chart.

A **Secondary** Category, which is optional, allows for the definition
of an implicit number of virtual Value columns for a data set. If a
Secondary column is configured, there must be exactly one Value column.
Secondary Category columns allow for multiple data points to be rendered
per Primary Category value. For example, if the user can configure *n*
number of statuses and wants to create a chart to visualize an
Object/Status Count, they could define a view that returns data as
outlined in the following table:

|        |         |       |
| ------ | ------- | ----- |
| Object | Status  | Count |
| **A**  | Status1 | 1     |
| **A**  | Status2 | 2     |
| **B**  | Status1 | 3     |
| **B**  | Status2 | 4     |

**NOTE:** All combinations of Object and Status are unique.

The configuration outlined in the above table ensures that as new
Statuses are added, they are automatically taken into account when the
chart renders by treating them as a Value column. When this chart is
rendered, the X-axis will have two tick marks: A and B. Within those
tick marks will be two series: Status1 and Status2. If this was a Bar
chart, there would be two bars for A and two bars for B. If a Status is
not included, it is assumed to be NULL. If a user wants non-existence to
equate to zero, this must be written into the view logic.
