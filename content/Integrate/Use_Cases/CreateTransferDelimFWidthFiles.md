# Create and Transfer Delimited or Fixed Width Files

<span id="Post Data Using UDF or Fixed Width Steps" class="popUpLink">Review
the steps in the process. </span>

During the file creation process, Integrate generates flat files in the
format as defined by the User Defined Template Type using the data as
configured by the Auto Generated Database Objects feature and the data
entered for the views in SQL.

**NOTE**: A process must be active to create files.

To create files and transfer them to the data source (a remote FTP
server):

1.  Click the **Postings** icon for the process.

2.  Click **Vertical View f**or the process post.

3.  Click **Edit**.
    
    *[View the field descriptions for the Process Post page’s Vertical
    View.](../Page_Desc/Process_Post_H.htm#Process_Post_V_All_Tabs)*

4.  Click **Advanced** tab.

5.  Select <span style="font-weight: bold;">StandardSAPPosting</span>
    from <span style="font-weight: bold;">BDC Post Method</span> list
    box.

6.  Click the **Transfer Files to Data Source** check box to enable it
    if it is not enabled.
    
    **NOTE**: If this check box is enabled, Integrate creates the flat
    file and transfers the file to the server set on the *Vertical* View
    of the *Template Process* page in the **Data Source ID** list box.
    If the check box is disabled, Integrate creates the file but leaves
    it on the application server. 

7.  Enter the **Batch Size**, if applicable.
    
    **NOTE**: The **Batch Size** determines how many records are to be
    included in each file. The file name is determined by the number of
    batches Integrate creates, \[Process Name\] \[Template
    Name\]\_\[Batch Number\].

8.  Click **General** tab.

9.  Click <span style="font-weight: bold;">View Primary Loop
    Data</span>.
    
    **NOTE**: The data as it will be created in the first record in the
    flat file displays.

10. Close the *Process Post* page.

11. Click **Post** on the Page toolbar, or close *Vertical* View and
    click **Post** for the process post on the *Horizontal* View.
    
    **NOTE**: Integrate displays a detailed message about the post
    status, including how many files were successfully created and
    transferred and how many records failed be created or transferred.

12. Click **View Messages** for the process post.
    
    **NOTE**: The *Messages* page displays one record for each file that
    Integrate created, and one record for each file that Integrate
    transferred.

13. Click **File** for a record for a created file.
    
    **NOTE**: The *Message File* page displays the path and file name of
    the file created on the application server. Integrate stores the
    file in the default folder configured on the **Posting Default
    Folder** field in **Common \> Configuration \> Modules \> Integrate
    \> Parameters – Integrate**. Within the folder, the file is saved as
    **\[Process Name\] \[Template Name\]\_\[Batch Number\]**.

14. Click **Download** to view the file Integrate created.
    
    **NOTE**: The downloaded file should display in the correct format
    as defined by the template and with the data as entered in the SQL
    tables. 
    
    **NOTE**: If the **Transfer Files to Data Source** check box was
    enabled for the process post, Integrate also attempted to transfer
    the file to the data source as configured on the *Vertical* View of
    the *Process Templates* page. Integrate created a folder on the FTP
    server with the process name.

15. Navigate to the *Post Monitor* page.
    
    **NOTE**: Either select **Post Monitor** from the *Navigation pane*,
    or click **Monitor** for the process post on the *Process Post
    Horizontal* View.

16. Click **Vertical View** for the process post.
    
    **NOTE**: The **Template Status** displays the status of the
    creation and transfer of the file to the remote server.

17. Click the hyperlink to access a page to download the file that was
    transferred to the FTP data source and that has been created on the
    remote server.

18. Click the download icon to download the file.
