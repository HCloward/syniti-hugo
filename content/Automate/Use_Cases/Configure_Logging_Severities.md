+++
title = 'Configure Logging Severities'
solution = 'Platform'
+++

# Configure Logging Severities

Logging allows users to examine how an interface was executed and why it
behaved as it did. Log entries are grouped in Tasks to provide a summary
of the steps involved in executing an interface.

Log severities assign a severity level to each task, such as debug,
notice, and error. An image is associated with each severity level,
which displays on the log. Refer to [View Logs for an
Interface](View_Logs_for_an_Interface) for more information on
accessing an interface’s log.

Automate is delivered with the following defined severities:

  - **80 – Fatal–** Production, fatal application error, application
    cannot continue, e.g., the database is down.

<!-- end list -->

  - **70 – Error–** Production, application error/exception, but the
    application can continue. Part of the application is not working
    properly.

<!-- end list -->

  - **60 – Warning–** Production, simple application error or unexpected
    behavior, but the application can continue, e.g., a bad login
    attempt or unexpected data import during jobs.

<!-- end list -->

  - **50 – Notice–** Production, notice information

<!-- end list -->

  - **40 – Info–** optionally, course grained (rarely written
    information), used to print that a configuration is initialized or
    that a long running import job is starting and ending.

<!-- end list -->

  - **30 - SQL–** statements and results

<!-- end list -->

  - **20 - Trace–** Program executions

<!-- end list -->

  - **10 - Debug –** Variables

Users may want to configure the image or the HTML tags for severities
and have HTML tags that display in the interface’s log, but it is not
essential. In order to configure the image, users must have access to
System Administration.

To configure a logging severity in Automate:

1.  Select **Configuration \> Logging \> Severities** in the
    *Navigation* pane.

2.  Click **Vertical View** for the desired Image.

3.  Click **Edit**.
    
    [View the field description for the Logging Severities page’s
    Vertical
    View](../Page_Desc/Logging_Severities#LoggingSeveritiesV)

4.  Select an image from the **Image Name** list box.
    
    **NOTE:** Images are added and configured on the Images page in
    System Administration. Refer to the [Add an Image to the
    DSP](../../Sys_Admin/Use_Cases/Add%20an%20Image%20to%20the%20DSP)
    for more information.

5.  Enter an HTML preformat tag in the **Html Pre Tag** field.

6.  Enter an HTML postformat tag in the **Html Post Tag** field.
    
    **NOTE:** These HTML tags configure the log message in the Automate
    *[Log](../Page_Desc/Log)* page. For example, the default
    messages for Notice severities display in a green font and Error
    messages display in red.

7.  Click **Save**.
