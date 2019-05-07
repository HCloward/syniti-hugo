+++
title = 'Posting Methods'
solution = 'Platform'
+++

# Posting Methods

When posting data to SAP using a process post, select the posting
method, which determines when and how Integrate sends the process post
to SAP. 

The posting methods are Foreground Post and Background Post.

## Foreground Post

This post method immediately posts data in the foreground. 

To use this method, either,

  - Click **Post** on the *[*Process
    Post*](../Page_Desc/Process_Post_H.htm)* page
  - Click **Post** in the Page toolbar on the *Vertical* View of the
    *Process Post* page
  - Click **Foreground Post** on the Posting tab of the *Process Post*
    page's *Vertical* View.

## Background Post

This post method schedules a post to run at a later date and time and in
the background. 

Use a Background Post when there is too much data to post in the
foreground without timing out the session, and to avoid putting too much
stress on the system.

**NOTE**: If posting a large number of records, schedule the post to run
during off-hours avoid causing performance issues.

To use this method on the *Vertical* View of the *Process Post* page on
the **Posting** tab:

1.  Enter a start time in **Post Start Time** to schedule the post to
    run at a later date.
    
    Or
    
    Click Calendar to select a date and time.  

2.  Click **Save**.

3.  Click Background Post.

**NOTE**: If no date and time are entered, the process post is posted in
the background almost immediately.
