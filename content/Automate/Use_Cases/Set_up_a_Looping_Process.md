# Set up a Looping Process

Looping is a powerful function that can be used with the FileIterator
event to:

  - Copy files from a source folder to a target folder
  - Run a batch job against those same files individually
  - Run a stored procedure against the same files

A few notes about looping:

  - Before setting up looping events, add Logical Paths and File
    Operations. Refer to [Add Logical Paths](Add_Logical_Paths.htm) and
    [Add File Operations](Add_File_Operations.htm) for more information.
  - Looping must be enabled for all events for the @filename to be
    populated with the most current Path/File.  If Looping is not
    enabled on any succeeding events (by clicking the Loop check box on
    the *[Interface Events](../Page_Desc/Interface_Events.htm)* page,
    only the last value of the @filename will be available to that
    event.
  - Looping is not needed on a FileIterator when there is no other
    process that needs to run individually against the files.

To enter content in the Field, type the field name in the list box and
click Use this Value for it to be added to the list box. The following
is an example of how looping can be set up:

**Event \#1:** Copy files from a source folder to a target folder, then
delete the files from the source folder.

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click the **Events** icon for the desired interface.

3.  Click **Add**.
    
    [View the field description for the Interface Events
    page](../Page_Desc/Interface_Events.htm)

4.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** The PRIORITY field indicates the order in which the
    interface event runs.

5.  Select **WebApp** from the **EVENT TYPE** list box.

6.  Select **InterfaceServer: File Operations** from the **PAGE ID**
    list box.

7.  Click the **LOOP** check box to enable it, indicating the event will
    be processed multiple times based on input.

8.  Enter a descriptive comment in the **COMMENT** field.

9.  Click **Save**; the *Vertical* View displays.
    
    [View the field description for the Interface Events page’s Vertical
    View](../Page_Desc/Interface_Events.htm#InterfaceEventsV)

10. Select **FileIterator** from the **Event** list box.

11. Click **Save**.

12. Click the **Web App Parameters** icon.

13. Click **Add**.
    
    [View the field description for the WebApp Event
    page](../Page_Desc/WebApp_Event.htm)

14. Enter the **@filename** in the **Field** combo box.
    
    **NOTE:** “filename” includes the complete path/filename of the
    copied file. Any “field” parameters that start with an “@” is an
    output parameter, which means that the files copied during this
    event can be referenced as “filename” in the next event.

15. Leave the **Value** field blank.

16. Click **Save**.

17. Enter **Operation** in the **Field** combo box.

18. Enter the name of a File Operation that was created on the [File
    Operations](../Page_Desc/File_Operations.htm) page in **Value**
    field.

19. Click **Save**.

**Event \#2**: Run a batch job against the same files individually where
the FileName is passed to a batch job

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click the **Events** icon for the desired interface.

3.  Click **Add**.
    
    [View the field description for the Interface Events
    page](../Page_Desc/Interface_Events.htm)

4.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** The PRIORITY field indicates the order in which the
    interface event runs.

5.  Select **WebApp** from the **EVENT TYPE** list box.

6.  Select **InterfaceServer: Parameters** from the **PAGE ID** list
    box.

7.  Click the **LOOP** check box to enable it, indicating the event will
    be processed multiple times based on input.

8.  Enter a descriptive comment in the **COMMENT** field.

9.  Click **Save**; the *Vertical* View displays.
    
    [View the field description for the Interface Events page’s Vertical
    View](../Page_Desc/Interface_Events.htm#InterfaceEventsV)

10. Select **CommandExec** from the **Event** list box.

11. Click Save.

12. Click the **Web App Parameters** icon.

13. Click **Add**.
    
    [View the field description for the WebApp Event
    page](../Page_Desc/WebApp_Event.htm)

14. Enter **commandname** in the **Field** combo box.

15. Enter **“c:\\test\\dirlist.bat” \#file1\#** in the **Value** field.
    
    **NOTE:**  The text within the quotes is the name of the batch job
    and the text between the \# signs is a parameter set up for this
    event. In this case, it is the @file parameter that is populated
    from the @filename parameter, which is configured for the
    FileIterator event. The text between the \#s must match the field
    name exactly, including the case. In this example, if the
    commandname stayed the same and a new parameter was added as File1,
    the interface job would fail because it would not have a value for
    \#file1\#.

16. Click **Save**.

17. Enter **file1in** the **Field** combo box.

18. Enter **@filename** in the **Value** field.
    
    **NOTE:** Any “field” (value) parameters that start with an “@” is
    an input parameter.

19. Click **Save**.

20. Enter **WAIT** in the **Field** field.

21. Leave the **Value** field blank.

The WAIT parameter makes the interface wait for the batch job to finish
before it goes to the next job. If the job fails and the WAIT parameter
is not set, the interface appears as Successful.

**Event \#3:** Run a stored procedure against the same files.

A stored procedure can be created to accept parameters. In the case of
the File Iterator Loop, if a stored procedure is part of the loop, the
filename needs to be one of the parameters of the stored procedure.

When adding a stored procedure as an event, the parameters in the stored
procedure are automatically created for the event. Click the Parameters
icon to see all the parameters sent to the stored procedure. One of
these parameters is the Field to which the @filename is passed.

For example, if an UpdateLog stored procedure that has a parameter named
“Description” is added after a File Iterator event, @filename is passed
to the “Description” field.

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click the **Events** icon for the desired interface.

3.  Click **Add**.
    
    [View the field description for the Interface Events
    page](../Page_Desc/Interface_Events.htm)

4.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** The PRIORITY field indicates the order in which the
    interface event runs.

5.  Select **StoredProcedure** from the **EVENT TYPE** list box.

6.  Click the **LOOP** check box to enable it, indicating the event will
    be processed multiple times based on input.

7.  Enter a descriptive comment in the **COMMENT** field.

8.  Click **Save**; *Vertical* View displays.

9.  Click **Save**.

10. Click the **Stored Procedure Parameters** icon to open the *[Stored
    Procedure](../Page_Desc/Stored_Procedure.htm)* page.
    
    **NOTE:** When adding a stored procedure as an event, the parameters
    in the stored procedure are automatically created for the event.
    Click the Stored Procedure Parameters icon to view all parameters
    sent to the stored procedure.

11. Enter the **filename** in the **Field** combo box.
    
    **NOTE:** “filename” is the name of the parameter in the stored
    procedure to which the filename is passed.

12. Enter **@filename** in the **Value** field.

13. Click **Save**.
