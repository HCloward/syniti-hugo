# Create a WebApp Event (Private) Business Rule

A WebApp Event (Private) allows you to execute an event that already
exists on the page.

Private events are like public events, but only events on the same page
can call that event. The use of private events helps reduce code
duplication.

For example, a large event must run on a page after a few steps run. Add
a button that when clicked, runs these steps before calling that large
event. Set the large event to private, and have the last business rule
be this ‘private’ event.

Refer to [Business Rule Guidelines](Business_Rule_Guidelines.htm) for
general information.

To create a WebApp Event (Private) Business Rule for a field in DSP
Application Development:

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

8.  Select **WebApp Event (Private)** from the **PROCEDURE TYPE** list
    box.

9.  Click **Save**; the *Vertical* View displays.

10. Select the name of the event on the page from the **Event Name**
    list box.

11. Enter text describing what the stored procedure does in the
    **Comment** field.
    
    **NOTE:** This comment is a description of the event; it does not
    display to the end user.

12. Click the **Advanced Properties** label to expand the label set.

13. Verify the **Run On Validate** check box is checked.

14. Click **Save**.
    
    **NOTE:** Business Rules run only after all validation rules on the
    page are processed without error.
