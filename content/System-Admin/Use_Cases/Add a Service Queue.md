# Add a Service Queue

A System Administrator can add a service queue to have a separate queue
to allow for processing of a specific set of tasks.

To add a service queue:

1.  Select **Admin \> Configuration \> Service \> Service Providers** in
    the *Navigation* pane.

2.  Click the **Queues** icon for a service provider.

3.  Click **Add**.
    
    [View the field descriptions for the Service Queues
    page](../Page_Desc/Service%20Queues.htm)

4.  Enter a priority in the **PRIORITY** field.
    
    **NOTE**: The priority sets the display order on the page.

5.  Select a queue ID from the **QUEUE ID** list box.
    
    **NOTE**: Values are:
    
      - **Background Events** — Queue for running the standard
        background processing events
      - **Service Pages** — Queue for executing pages defined as Service
        Pages on the schedule they are assigned
      - **General** — All foreground events will run by default in the
        General Queue
      - **Indexing** — The general indexing service page

6.  Enter a maximum number of threads in the **MAXIMUM THREADS** field.
    
    **NOTE**: The Administrator can specify how many parallel processes
    can be actioned on the queue at any one time. The user must
    understand the underlying server architecture to set the number of
    queues based on the number of processor cores and threads available.
