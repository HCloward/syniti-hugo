# Add Logical Paths

Logical Paths is a configuration setting required for the FileIterator
event, which copies files from a source folder to a target folder, then
deletes the files from the source folder. Refer to [About Automate
Events](About_Automate_Events.htm) for more information.

A logical path points to a folder (a local or networked file system
mapped with a drive letter) or an FTP site where files are either
created or to where files are copied.

A logical path has no concept of source or destination outside the
context of a File Operation, so in some cases it is a target destination
and sometimes it is a source destination.

To add a logical path in Automate:

1.  Select **IO Config \> Logical Paths** in the *Navigation* pane.

2.  Click **Add**.
    
    *[View the field description for the Logical Paths
    page](../Page_Desc/Logical_Paths.htm)*

3.  Enter a file path of the folder or the FTP site in the **LOGICAL
    PATH** field.
    
    **NOTE:** This is where files are either created or to where files
    are copied. It is a good idea to name logical paths descriptively,
    for example, if a logical path is only used as a source and not a
    target, indicate this in the name of the logical path.

4.  Select a value to determine how files are moved from the **TRANSPORT
    TYPE** list box. Options are:
    
      - **Local** – Local File System, which means the files are in
        folders to which that the DSP can read/write.
    
      - **FTP** – File Transfer Protocol (FTP), which means the files
        are located in an FTP address. FTP is a standard network
        protocol used to copy a file from one host to another over a
        TCP/IP-based network. All transmissions are in clear text; user
        names, passwords, FTP commands and transferred filed can be read
        by anyone on the network.

5.  Select a modification from the **FILE MODIFICATION** list box.
    Options are:
    
      - **Batched** – When the files are copied to the destination, they
        are broken into files with the amount of records noted in the
        **Batch Size** field (configured on the *Vertical* View of the
        [*Logical Paths*](../Page_Desc/Logical_Paths.htm#LogicalPathsV)
        page).
        
        **NOTE**: Excel libraries may need to be installed on the DSP
        application server if Batched is used when copying Excel files.
    
      - **Segmented By Field** – When the files are copied to the
        destination, a file is created for each unique value in the
        **Segment By Field** field (configured on the *Vertical* View of
        the *[Logical
        Paths](../Page_Desc/Logical_Paths.htm#LogicalPathsV)* page).
        
        **NOTE**: Excel libraries may need to be installed on the DSP
        application server if Segment By Field is used when copying
        Excel files.
    
      - **None** – File is not modified. This is the recommended
        selection when moving files from one folder to another.
        
        **NOTE:** The FILE MODIFICATION field is only taken into
        consideration on Logical Paths designated as a source or an
        input.

6.  Select a format from the **FILE FORMAT** list box. Options are:
    
      - **Delimited** – For each record in each file, fields are
        separated by a delimiter (configured in the **Delimiter** field
        on the *Vertical* View of the *[Logical
        Paths](../Page_Desc/Logical_Paths.htm#LogicalPathsV)* page). In
        a comma-separated values (CSV) file, the data items are
        separated using commas as a delimiter, while in a tab-separated
        values (TSV) file, the data items are separated using tabs as a
        delimiter. Column headers are sometimes included as the first
        line, and each subsequent line is a row of data.
    
      - **Excel** – Each file is an Excel file. When performing a
        straight copy of Excel files, the version does not matter. Excel
        libraries may need to be installed on the DSP application server
        if Segment By Field or Batched are used when copying Excel
        files.
    
      - **Fixed Width** – Each field is specified by column widths, pad
        character and left/right alignment.

7.  Click **Save**; the *Vertical* View displays.
    
    **NOTE:** The fields available depend on the File Modification and
    the File Format selected.
    
    *[View the field description for the Logical Paths page’s Vertical
    View](../Page_Desc/Logical_Paths.htm#LogicalPathsV)*

8.  If the FILE MODIFICATION is Batched, enter a value in the **Batch
    Size** field to control the number of records written to each file.

9.  If the FILE FORMAT is Delimited, enter the value of the delimiter
    used between each field in a record within the file in the
    **Delimiter** field.

10. If the FILE FORMAT is Delimited, populate the **Text Qualifier
    field** with a character used to enclose text strings. For example:
    if the Delimiter is set to ;, the Text Qualifier is set to “ and
    this string exists in a record: Test;”test one;”;”test two”;None.
    The second field in the record would be test one;. The ; in the
    double quotes would be considered part of the field and not
    evaluated as the delimiter.

11. Click the **Contains Header** check box to enable it, if there is a
    header record in the file that must be ignored. Enabling this field
    is useful when the FILE MODIFICATION is set to Segment by Field.

12. If the FILE MODIFICATION is SegmentByField, enter the name of the
    field being segmented in the **Segment by Field** field.
    
    **NOTE:** Segment by Field displays the field in the file used to
    produce one output file for each unique value in the field. For
    example, given a file of Customers named Customers.txt, entering a
    “State” in the Segment by Field produces one output file for each
    unique value found in the state column, e.g., CustomersMA.txt,
    CustomersNY.txt, CustomersTX.txt. This field only displays when
    SegmentByField is selected in the FILE MODIFICATION field on the
    *Horizontal* View.

13. Click **Save**.

14. Click the **Instances** icon for the desired logical path.

15. Click **Add**.
    
    *[View the field description for the Logical Path (Instance)
    page](../Page_Desc/Logical_Path_Instance.htm)*
    
    **NOTE:** Depending on the Transport Type, different fields display.

**If the Transport Type is FTP**

1.  Select an environment from the **INSTANCE** list box.
    
    **NOTE:** The instance configured must match the instance selected
    on the *[Parameters](../Page_Desc/Parameters.htm)* page in Automate.
    If the instances do not match, the file processing will not work
    correctly.

2.  Enter the hosting server name in the **HOSTNAME** field.

3.  Enter a value on which the server listens to the FTP connections in
    the **PORT** field. The default value is 21.

<!-- end list -->

1.  Enter an FTP path in the **PATH** field.
    
    **NOTE:** Do not include a ftp.// destination or a port number; only
    a server name or an IP address is required.

2.  Populate the **User ID** field.

3.  Populate the **Password** field.
    
    **NOTE:** The User ID and Password fields are used to control access
    to the FTP site.

**If the Transport Type is Local:**

1.  Select an environment from the **Instance** list box.
    
    **NOTE:** The instance configured must match the instance selected
    on the *[Parameters](../Page_Desc/Parameters.htm)* page in Automate.
    If the instances do not match, the file processing will not work
    correctly.

2.  Enter the complete path of where the files will be read or written
    in the **Path** field.

*[View the field description for the Logical Path (Instance) page’s
Vertical
View](../Page_Desc/Logical_Path_Instance.htm#LogicalPathInstanceV)*

16. Click **Save**; the *Vertical* View displays.

17. Click the **Can Read** check box to enable it, which grants read
    access to the folder.

18. Click the **Can Write** check box to enable it, which grants write
    access to the folder.

19. Click the **Can Delete** check box to enable it, which grants delete
    access to the folder.

20. Click **Save**.

21. Click the **Test** icon to test the connection to the path field.
    
    **NOTE:** When the record is saved, the access privileges at the
    location specified by the Logical Path instance are tested. Results
    display on the *Vertical* View.

22. Click the **Browse** icon browse the FTP site or the path for other
    folders or files, and change the FTP site or path if necessary.
    Refer to [Browse FTP Site or Path](Browse_FTP_Site_or_Path.htm) for
    more information.
