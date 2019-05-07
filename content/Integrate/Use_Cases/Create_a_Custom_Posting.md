+++
title = 'Create a Custom Posting'
solution = 'Platform'
+++

# Create a Custom Posting

Integrate supports custom process posts and is designed to support
posting with any custom component without the need for plugin or
external page development.

**NOTE:** To perform these steps, a process must exist in Integrate, and
the user must understand how to create a page view in the platform.

To create a custom *Process Post* page that uses Integrate as its
posting tool:

1.  Create a page view (*Horizontal* or *Vertical*) with an event. The
    view must have these columns to post an Integrate post process:
    
      - **Process ID** – The ID of the Integrate process to use for the
        post
    
      - **Posting ID** – The unique identifier for the post
        
        **NOTE**: If using the table ttProcessPost for the view,
        inserting records into that table automatically generates a new
        PostingID value.
        
        The following columns are optional in the view.
        
        <table>
        <tbody>
        <tr class="odd">
        <td><p>Field</p></td>
        <td><p>Description</p></td>
        </tr>
        <tr class="even">
        <td><p>BackgroundPostingQueueID</p></td>
        <td><p>Displays the platform queue in which background posting requests are scheduled.</p></td>
        </tr>
        <tr class="odd">
        <td><p>BatchSize</p></td>
        <td><p>Displays the number of records to be posted at one time. If a value is not entered, Integrate uses the default of 100 records. This field can be used with process posts that use the StandardSAPPosting method only. </p></td>
        </tr>
        <tr class="even">
        <td><p>BDCPostMethod</p></td>
        <td><p>Displays the method Integrate uses when posting. If no method is selected, Standard SAP Posting is used.</p>
        <p>Methods available for a process post based on a single BDC Script template include:</p>
        <p>BOAFileCreation – Creates files on the web server that can be used in the /BOA/ZBDCPROCESS program in SE38.</p>
        <p>BOAPosting – Posts immediately using the BOA Function Module.</p>
        <p>BOAPostingWithErrorSessionCreation – Posts immediately using the BOA Function Module and creates an SM35 session with any errors. The error session contains only the records that failed to post; successful transactions are not included.</p>
        <p>BOASessionCreation – Uses the BOA Function Module to create an SM35 session containing all of the data in the process post, but does not post the data to SAP.</p>
        <p>StandardSAPPosting – Posts using the standard SAP Function Modules.</p>
        <p>All other process posts use the StandardSAPosting option.</p></td>
        </tr>
        <tr class="odd">
        <td><p>Comment</p></td>
        <td><p>Displays information entered about the process post. Integrate includes this text with every record of the process post in the ttMessage table. If no comment is entered, Integrate uses an empty string.</p></td>
        </tr>
        <tr class="even">
        <td><p>ContinueOnCommit</p></td>
        <td><p>If set to true, the script continues with processing after a commit has occurred. Whether this option is used depends on the transactions being played back in the BDC recording. If no value is passed, Integrate uses False. This field can be used with process posts that use any BDC Post Methods except StandardSAPPosting.</p></td>
        </tr>
        <tr class="odd">
        <td><p>CreateErrorSessions</p></td>
        <td><p>If set to true, Integrate creates an error session. If no value  is passed, Integrate uses False. This field can be used with process posts that use BDC Post Methods BDCPostingWithErrorSessionCreation and BDCSessionCreation.</p></td>
        </tr>
        <tr class="even">
        <td><p>CreateGUIDebugScript</p></td>
        <td><p>If set to true, Integrate creates a copy of the GUI script run against SAP and writes it to the ttMessage table along with the results of the post. This field can be used with process posts that use the StandardSAPPosting only.</p></td>
        </tr>
        <tr class="odd">
        <td><p>CreateSessionFilesOnly</p></td>
        <td><p>If set to true, Integrate creates files for importing using the custom BOA Function Module. If no value is passed, Integrate uses False. This field can be used with process posts that use BDC Post Methods BDCPostingWithErrorSessionCreation and BDCSessionCreation.</p></td>
        </tr>
        <tr class="even">
        <td><p>FileSplitInterval</p></td>
        <td><p>Displays an interval to indicate the number of transactions in each file created during the posting process. This field can be used with process posts that use BDC Post Method BOAFileCreation only. Integrate uses 5000 by default.</p></td>
        </tr>
        <tr class="odd">
        <td><p>GroupName</p></td>
        <td><p>Displays the name that appears in the Group Name column of the SAP SM35 session.If the field is blank, Integrate uses &gt;BOA. This field can be used with process posts that use any BDC Post Method except StandardSAPPosting.</p></td>
        </tr>
        <tr class="even">
        <td><p>KeepSession</p></td>
        <td><p>If set to true, the session is saved in an SAP SM35 session even after a successful post. Saving a session is useful if it must be rerun. This option is used with the BDC Post Method BOASessionCreation and BOAPostingWithErrorSessionCreation. If no value is passed, Integrate uses False.</p></td>
        </tr>
        <tr class="odd">
        <td><p>NoDataSymbol</p></td>
        <td><p>Displays a symbol to represent “no data” in the post. If the field is blank, Integrate uses an empty string to represent no data.</p></td>
        </tr>
        <tr class="even">
        <td><p>PostingID</p></td>
        <td><p>Displays a unique ID to identify the specific post, used to determine which messages to process from the ttMessage table.</p></td>
        </tr>
        <tr class="odd">
        <td><p>PostStartTime</p></td>
        <td><p>Displays the date and time by which posting begins if using a Schedule Post.</p></td>
        </tr>
        <tr class="even">
        <td><p>SessionFilePath</p></td>
        <td><p>Displays the location on the web server where Integrate creates files to usein the /BOA/ZBDCPROCESS program in SE38. This field can be used with process posts that use the BDC Post Method BOAFileCreation only.</p></td>
        </tr>
        <tr class="odd">
        <td><p>SessionFileName</p></td>
        <td><p>Displays the name of the file to create.This field can be used with process posts that use the BDC Post Method BOAFileCreation only.</p></td>
        </tr>
        <tr class="even">
        <td><p>WebAppID</p></td>
        <td><p>Displays the WebAppID containing the data to post. If no ID is passed, the WebAppID of the page that has the post button is used.</p></td>
        </tr>
        <tr class="odd">
        <td><p>WhereClause</p></td>
        <td><p>Displays the Where Clause to apply to the post. If no Where clause is passed, Integrate uses an empty string.</p></td>
        </tr>
        <tr class="even">
        <td><p>SuppressReturnMessages</p></td>
        <td><p>If set to true, after Integrate has successfully posted data, no messages display to the user. If set to false, the default setting, messages display. If the column is not included in a view, Integrate uses the default setting and displays messages regarding successful postings to the user.</p></td>
        </tr>
        </tbody>
        </table>

2.  Register the **Integrate: Integrate stored credentials posting
    adapter** public plugin as an event to the page, if applicable. The
    public plugins available for Integrate posting are:
    
      - **Integrate foreground posting adapter** - Plugin assigned to
        any page  to post via Integrate in the foreground.
      - **Integrate Background Posting Adapter** – Plugin assigned to
        any page to post via Integrate to a background queue
    
    **NOTE:**:   The *Process Post* page in Integrate was created using
    the posting plugins available to all components and can serve as an
    example.
    
    **NOTE:**: The *Process Post* page uses the table ttProcessPost.
    Inserting records into that table automatically generates a new
    PostingID value.
    
    **NOTE:**: Business Rules can be registered to a page that call any
    of the Integrate posting plugins. Any page that calls the Integrate
    posting plugins must provide ProcessID and PostingID as inputs.

3.  Write a message cleanup procedure. When a posting is
    finished,<span> </span> messages are written to the ttMessages
    table. The table must be manually maintained to clean out the
    messages returned from SAP. As a recommendation, the PostingID can
    be used to filter records to delete for a specific post.

4.  Write a procedure that inserts a record into the
    ttProcessPostConnection table for every process template in the
    process that specifies the ProcessTemplateID, the PostingID and the
    ConnectionID. The ConnectionID is the DataSourceID from the
    dspCommon ttDataSourceRegistry table. Records in this table must be
    manually maintained. As a recommendation, the PostingID can be used
    to filter records to delete for a specific post.
