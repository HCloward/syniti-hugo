# Control Display and Limit Possible Candidates

With the results of Duplicate Detection validation, the primary key in
the Duplicate Detection Validation fields and any fields for which
Duplicate Detection has been enabled display. To include or exclude
specific columns, create a view containing the primary key columns and
any additional columns that should display to the user.

**NOTE**: When performing Duplicate Detection against an index of
another table, the view must contain the primary key columns as defined
at the index level. If there are no keys defined at the index level,
then the view must contain the source table’s primary keys.

Once created, the view needs to be registered in DSP®.

To register the view:

1.  Click **Admin \> WebApps** on the *Navigation* pane.
2.  Click the **Pages** icon for a webapp.
3.  Click the **Events** icon for a page.
4.  Click the **Validation Rules** icon for an event.
5.  Click **Vertical View** for a rule.
6.  Click **Edit**.
7.  Select view from **Duplicate Detection View** list box.
8.  Click **Save**.

When the Duplicate Detection Validation is triggered, the columns in the
view display rather than the default columns selected by DSP®. In
addition to controlling which columns display to the user, the Duplicate
Detection view can be used to filter out records. This filtering process
allows the developer to control which records are candidates for
Duplicate Detection.

By way of example, an index may contain customer records from around the
world, but only checking for Duplicate Detection in the United States is
necessary. A Where Clause can be added to the Duplicate Detection view.
The Where clause selects only those customers located in the United
States by performing an Inner Join to the Duplicate Detection view at
runtime. Therefore, any records not present in the view are, by
definition, excluded from the validation result set.
