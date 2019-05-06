# Monitor Posts

Integrate allows a user to monitor process posts, whether submitted in
the background or foreground, for success or failure; view messages
returned from the target system; and view each process post’s data
exactly as it was sent to the target system.

The *Post Monitor* page displays the current posting status for all
posts.

To monitor posts on the *Post Monitor* page:

1.  Select **Post Monitor** from *Navigation pane* to view details about
    every process post.
    
    Or
    
    Access the *Post Monitor* page for a specific process post by
    selecting **Monitor** on the *Process Post* page *Horizontal* View.

2.  Click **Vertical View** for a process post to view additional
    details about the post, including a message returned from the target
    system regarding post status, the status of the current template,
    and audit information.  In the case of process posts based on User
    Defined templates, a link to the file Integrate created also
    displays.

3.  Click Templates.
    
    **NOTE**: The *Post Monitor: Template* page provides details about
    each template in the process, including the number of records
    posting for each template and the status of the template posting.

4.  Click **Files**.
    
    **NOTE**: The *Post Files* page lists each file that was posted to
    the target system for the post process. Multiple files represent
    batches of data set by the **Batch Size** on the *Process Post*
    page’s *Vertical* View on the **Advanced** tab. This page also
    display statuses for the file, including posting status and remote
    system status, and provides a link to download the file that was
    created in the case of a process post based on  User Defined
    template. This page does not display data for a process post based
    on a BDC Script, GUI Script, or BAPI/RFC template.

To monitor complicated background posts to ensure they ran as scheduled
(and override the schedule and post immediately if necessary), use the
*Post Engine* and *Post Adapter* pages.

5.  Select **Advanced \> Post Engine** from *Navigation pane*.
    
    **NOTE**: The *Post Engine* page lists details about the background
    posting, including the template in the process post that is
    currently being processed, and the time the posting began.

6.  Click **Post Adapter** to view the data as it was submitted for the
    process post, and to submit the post again using one of the posting
    methods. Refer to [*<span style="color: #0000ff;">Posting
    Methods</span>*](Posting_Methods.htm) for more information.
