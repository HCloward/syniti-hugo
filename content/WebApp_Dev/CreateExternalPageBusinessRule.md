+++
title = 'Create an External Page Business Rule'
solution = 'Platform'
+++

# Create an External Page Business Rule

An External Page rule allows you to execute a plugin as the event action
to determine whether the associated record is valid. The validation
fails if a non-zero result is returned.

Refer to [Business Rule Guidelines](Business_Rule_Guidelines) for
general information.

To create an External Page Business Rule for a field in DSP Application
Development:

1.  Select **Admin \> WebApps** in the *Navigation* pane.
2.  Click the **Pages** icon for the WebApp.
3.  Click the **Events** icon for the page.

OR

1.  Access the WebApp page.

2.  Click the **Change Settings** icon on the Site toolbar.

3.  Click **Design**.

4.  Click the **Events** icon for the page.

5.  Click the **Business Rules** icon for the event.
    
    **NOTE:** If no record exists, the page displays in ad mode.
    Otherwise, click **Add**.

6.  Enter a value in the **PRIORITY** field to determine execution
    order.
    
    **NOTE:** CranSoft attempts to wrap all procedures within a single
    SQL transaction. To avoid deadlocks, all pending transactions are
    committed before executing an external process. As a result, mixing
    external processes and SQL stored procedures can result in errors
    which cannot be completely rolled back. To minimize the effect,
    consider placing all external processes after SQL stored procedures
    by giving them a higher priority.

7.  Verify the **ACTIVE** check box is checked.

8.  Select **External Page** from the **PROCEDURE TYPE** list box.

9.  Click **Save**; the *Vertical* View displays.

10. Select the name of the plugin that executes when the event fires
    from the **Web App Plugin Type Code** list box.

11. Enter text describing what the stored procedure does in the
    **Comment** field.
    
    **NOTE:** This comment is a description of the event; it does not
    display to the end user.

12. Click the **Advanced Properties** label to expand the label set.

13. Verify the **Run On Validate** check box is checked.

14. Click **Save**.
    
    **NOTE:** Business Rules run only after all validation rules on the
    page are processed without error.
