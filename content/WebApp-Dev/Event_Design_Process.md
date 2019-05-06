# Event Design Process

Below is a list of questions to ask to ensure an event is fully
implemented with all available and relevant features.

Refer to [Create Events](Create_Events.htm) for general information.

**NOTE:** When creating an event, a key column property must be set if
the page is based on a view or if the page doesn’t have a primary key.
For example, a user creates a background event that runs on a *Vertical*
View, but the parameter, the primary key, only displays on the
*Horizontal* View.

The user must either:

  - Include the primary key as one of the arguments in the stored
    procedure (since it should be in both the *Horizontal* and
    *Vertical* View) and then, in the stored procedure, run a select
    statement to get another column's value from the *Vertical* View
    using the primary key.
  - Include the column in the *Horizontal* View and hide it via a column
    property with the Horizontal View type. Refer to [Set Column Control
    Status](Set_Column_Control_Status.htm) for more information.

**NOTE:** The options below are set on the *[Page
Events](../Sys_Admin/Page_Desc/Page_Events_H.htm)* page (**Admin \>
WebApps\> Pages \> Events**).

  - **Is this a large or long-running process best suited for the
    background? Does it need user-session-level context?**Any event
    running for more than several seconds must be run in the background.
    If the process takes fewer than several seconds to run, or if the
    process needs user-session-level context, set it to run in the
    foreground. A Foreground event runs on the Web Server, which can
    give plugin code access to specific users and runtime information
    from the web session. A Foreground event can also provide immediate
    feedback to the user, such as reloading the page and displaying
    post-event messages. Configure this option using the EVENT PROCESS
    TYPE ID list box on the *Page Events* page.

  - **Should the user be warned before executing the event?** If so,
    include a Pre Message, which prompts the user with an OK or Cancel
    option for continuing the execution of the event. Most actions that
    are not easily reversible should include a Pre Message to ensure the
    user does not accidently disrupt a process when executing an event.
    Enter the message in the Pre Message field on the *Page Events*
    page’s *Vertical* View.

  - **Should a Post Message be included?** Post Messages display at
    different times depending on whether the event is foreground or
    background. A Background event displays the message as a Minor
    Notification immediately after the job has been queued. In this
    case, it is a good idea to use the Post Message to indicate to the
    user that the work will be run at a certain time (for example, “The
    package will be processed shortly.”). Foreground events display
    their message after execution. Post Messages for Foreground events
    are useful when executing plugin code that does not always write out
    a message, or when executing non-plugin Business rules. The Post
    Message ensures that the user always receives a confirmation that
    their action has completed. Enter the Post Message in the Post
    Message field on the *Page Events* page’s *Vertical* View.

  - **Should the Transaction Method be changed from the default
    (Disabled)?** The options are:
    
      - **Disabled Transaction Method** – Business rules stop running on
        exception. This option provides the least likeliness of a
        deadlock as well as fastest execution time. However, when
        running a series of procedures, an error in one will not result
        in a rollback of the previous procedures. This could potentially
        leave the database in an unstable state, if these procedures are
        not idempotent.
    
      - **Enabled Transaction Method** – Encapsulates the Business rules
        in a database transaction. This option provides the
        functionality of rolling back in the event of an error. This
        rollback is applied per Execution Groups, which are formed by
        sequential sets of stored procedures. For example:
        
        1.  Three stored procedures run.
        2.  An External Page runs.
        3.  Three more procedures run.
        
        This results in two Execution Groups (first three, and last
        three). In the event a procedure within one of the Execution
        Groups fails, any other procedure that has been run within that
        group is undone. This setting carries the highest potential of
        deadlock. A failure within an Execution Group does not cause any
        other execution groups to roll back.
    
      - **Serialized Transaction Method** – Only allows one instance of
        the page’s event to run at a time. For example, if User A and
        User B are attempting to execute the event (even against
        different records), one event has to complete before the other
        one starts.This option is similar to Enabled, with the added
        locking at the Page Event level. When this option is chosen,
        each event invocation will ensure exclusive execution of the
        underling Page Events rules. This option reduces the number of
        procedure related deadlocks occurring, but can lead to event
        lock related timeouts if several users are attempting to execute
        the same event simultaneously.
        
        **NOTE:** This option must **not** be used if the column
        property supports multi-row actioning.
    
    Set the Transaction Method on the *Page Events* page’s *Vertical*
    View on the Advanced Properties tab.

  - **At what “Event Level” should this event execute?**The default and
    most commonly used Event Level is Row, which passes the row
    information to the event. The Page Event Level is commonly used for
    toolbar buttons defined from the Toolbar view for the page. The Page
    Event Level does not pass row-level information to the event. If a
    toolbar button is set to a Page-level event, the user can click the
    button to run the event when there are no records on the page. Set
    the Event Level on the *Page Events* page’s *Vertical* View on the
    Advanced Properties tab.

  - **Should a post event “Function” be utilized?** This modifier allows
    the page designer to force the user either to be navigated back to
    their previous page or to the page’s *Vertical* View. For example,
    if the page designer selects Back, the user may be expected to
    navigate to a second page, click a particular button, and then be
    sent back to the previous page where that event has affected the
    previous record. The Vertical option can be used when an action on
    the Horizontal View requires that the user access the *Vertical*
    View, where additional information or required fields for a record
    display. Set the Function on the *Page Events* page’s *Vertical*
    View on the Advanced Properties tab.
