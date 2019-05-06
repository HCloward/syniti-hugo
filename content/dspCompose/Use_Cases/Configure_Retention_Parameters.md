# Configure Retention Parameters

Retention Parameters control how many days a request is retained before
it is archived.

The retention interval is configured within a
<span id="dspCompose Request Status" class="popUpLink">request
status</span> on the *Request Status* page (accessible by clicking
**Configuration \> Request Status** in the *Navigation pane*).

This status is copied into each template when the template is created;
however, it can be modified per template.

**NOTE**: To modify a retention parameter, the template must not be
active or must be in Developer Mode. Refer to [Modify an Active Template
in Developer Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for
more information.

To configure retention parameters for a template:

1.  Click **Team** in the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Vertical View** for a template.

4.  Click **Configuration** tab.

5.  Click **Retention Params**.

6.  Click **Edit** for a request status.
    
    *[View the field descriptions for the Template (Request Retention)
    page.](../Page_Desc/Template_Request_Retention.htm)*

7.  Enter a value in **RETENTION INTERVAL** field.
    
    **NOTE**: The RETENTION INTERVAL is the number of days a request in
    the selected status is retained before it is archived.

8.  Click **Save**.

Refer to [Archive Requests](Archive_Requests.htm) for more information.

Request statuses used by active requests are:

  - <span style="font-weight: bold;">Request in Process</span> – The
    request has been created, but has not yet been posted by the Post
    role.
  - <span style="font-weight: bold;">Posting Scheduled –</span> The
    request is scheduled to be posted using the Schedule Post posting
    option. Refer to [Post Request Data to the Target ERP
    System](Post_Request_Data_to_a_Target_ERP_System.htm) for more
    information.
  - <span style="font-weight: bold;">Posting</span> – The request is
    currently being posted to the Target ERP system.
  - <span style="font-weight: bold;">Posted</span> – The request has
    been posted successfully to the Target ERP system.
  - <span style="font-weight: bold;">Posted with Errors</span> – At
    least one record in the request has not posted successfully to the
    Target ERP system. Refer to [Correct and Post Failed
    Records](Correct_and_Post_Failed_Records.htm) for more information.
  - <span style="font-weight: bold;">Finish Processing</span> – The
    posting process for the request is finished. The Post role has
    clicked the Finish button for the request on the
    <span style="font-style: italic;">Request (Roles)</span> page after
    it has posted. The tables from the Target ERP system with the data
    changed by the request is in the process of being downloaded from
    the source database.
  - <span style="font-weight: bold;">Finish Failed</span> – The posting
    process for the request is finished. After the Finish button for the
    Post role has been clicked to initiate the download process, the
    download of tables encountered an error during the process.

Request statuses used by inactive requests are:

  - <span style="font-weight: bold;">Finished</span> – The posting
    process for the request is finished. The Post role has clicked the
    <span style="font-weight: bold;">Finish</span> button for the
    request on the <span style="font-style: italic;">Request
    (Roles)</span> page after it has posted. <span> </span>The tables
    from the Target ERP system with the data changed by the request have
    been downloaded from the source database.
  - <span style="font-weight: bold;">Cancelled</span> – The request has
    been cancelled. <span>A cancelled request can be archived, but
    cannot be reset. Refer to [Change Request
    Status](Change_Request_Status.htm) for more information.</span>
  - <span style="font-weight: bold;">Deleted</span> –
    <span style="font-family: Arial, sans-serif;">The request has been
    deleted and cannot be reset. The data entry records for the deleted
    request cannot be archived and are deleted from the Data database
    once the Service (Archive Requests) runs.</span><span> Refer to
    [Change Request Status](Change_Request_Status.htm) for more
    information.</span>
