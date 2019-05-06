# Run Interface Events Sequentially

In most cases, events run sequentially according to the event’s
priority, with the lowest priority executing first. However, a user may
need to force sequential events if the preceding event submitted a
background job, as performed in Collect. The validation would have to
determine if the background job had finished before the next event would
start.

To run Interface events sequentially in Automate:

1.  Create a validation view in the Data Source ID used for the
    interface.

2.  Select **Interfaces** in the *Navigation* pane.

3.  Click the **Events** icon for the desired interface.

4.  Click the **Validations** icon for the event that needs to wait
    until the previous event is done.

5.  Click **Add**.
    
    [View the field description for the Interface Event (Validations)
    page](../Page_Desc/Interface_Event_Validations.htm)

6.  Enter a value in the **Priority** field.

7.  Select **View** from the **VALIDATION TYPE** list box.

8.  Select **Validation** from the **VALIDATION PURPOSE** list box. This
    means that if the view returns a value, then the validation has
    failed.

9.  Select **Pre** from the **VALIDATION WHEN** list box to indicate the
    validation runs before the event runs.

10. Select **Retry** from the **DISPOSITION** list box to indicate that
    if the validation fails, the interface waits and retries running the
    validation.

11. Click **Save**; the *Vertical* View displays.
    
    [View the field description for the Interface Event (Validations)
    page’s Vertical
    View](../Page_Desc/Interface_Event_Validations.htm#InterfaceEventValidationsV)

12. Enter a descriptive comment in the **Comment** field.

13. Click **Save**.

14. Return to the [*Interface
    Events*](../Page_Desc/Interface_Events.htm) page.

15. Click **Vertical View** for the event.

16. Click **Retry Parameters** to expand the section.

17. Click **Edit**.
    
    [View the field description for the Interface Event page’s Vertical
    View](../Page_Desc/Interface_Events.htm#InterfaceEventsV)

18. Enter **10** in the **Retry Interval** field to indicate the stored
    procedure will retry 10 times.

19. Enter **60** in the **Maximum Retry Interval** field.

20. Select **Seconds** from the **Retry Interval UOM** list box.
    
    **NOTE:** This means that when the stored procedure fails, the DSP
    will try to run it again in 60 seconds for 10 times and then stop.

21. Click **Save**.
