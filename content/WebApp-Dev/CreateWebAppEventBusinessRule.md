# Create a WebApp Event Business Rule

A WebApp Event allows you to execute an event that already exists on a
different page. For instance, you can create a button in a custom app
that runs the same event as the Refresh Table button in Collect. Since
the functionality for refreshing a table already exists in Collect, this
allows you to call it from anywhere without duplicating the code.

Refer to [Business Rule Guidelines](Business_Rule_Guidelines.htm) for
general information.

To create a WebApp Event Business Rule for a field in DSP Application
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

7.  Verify the **ACTIVE** check box is checked.

8.  Select **WebApp Event** from the **PROCEDURE TYPE** list box.

9.  Click **Save**; the *Vertical* View displays.

10. Select the name of the event on the page from the **Event Name**
    list box.

11. Select the view name from the **Parameter View** list box, if
    needed.
    
    **NOTE:** This view contains extra columns to map to parameters to
    send to the other event. This view will be executed as part of the
    event, pulling in an associated record to the executing record, and
    assigning the other column data to mapped parameters. This parameter
    view allows another view to provide more data to an event without
    putting all the columns in the horizontal or vertical view on the
    page.

12. Enter text describing what the stored procedure does in the
    **Comment** field.
    
    **NOTE:** This comment is a description of the event; it does not
    display to the end user.

13. Click the **Advanced Properties** label to expand the label set.

14. Verify the **Run On Validate** check box is checked.

15. Click **Save**.
    
    **NOTE:** Business Rules run only after all validation rules on the
    page are processed without error.
