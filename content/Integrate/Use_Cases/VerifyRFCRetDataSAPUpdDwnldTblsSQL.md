# Verify the RFC Retrieved Data from SAP and Updated the Download Tables in SQL

<span id="Post Data using an RFC Steps" class="popUpLink">\>Review the
steps in the process. </span>

<span style="font-weight: bold;">NOTE:</span> This use case provides an
example of posting using the **RFC BOA/ZRFC\_READ\_TABLE – External
access to R/3 tables via RFC**, but does not supply comprehensive
instructions to suit all RFCs.

To access the download tables to verify the data retrieved from SAP:

1.  Log in to SQL Management Studio.

2.  Locate the database.

3.  Locate the following tables:
    
    tt\*\_Fields\_Download
    
    tt\*\_Output\_Structure\_Download
    
    tt\*\_Data\_Download

For each QUERY\_TABLE entered in the primary loop and included in the
Posting (in the example, T001W and KNA1):

4.  Verify the download tables were updated with data from SAP.
5.  Verify that the **PostingID** column is populated.
6.  Verify that the **ParentID** column in each table is populated with
    a unique number for each QUERY\_TABLE.
7.  In the **tt\*\_Data\_Download-Data\_Wa** column, verify that data is
    delimited by |.
8.  Determine and make note of the record count for each QUERY\_TABLE in
    the tt\*\_Fields\_Download table (in the example, T001W – 62; KNA1 –
    165).
9.  Determine and make note of the record count for each QUERY\_TABLE in
    the tt\*\_Data\_Download table.

To verify the data in SAP:

1.  Enter **SE11** in the **Command** field and press Enter.

2.  Enter the QUERY\_TABLE name. In the example, the user entered KNAI.
    
    ![Description:
    ABAPDictionary](../../../Resources/Images/image008.png)

3.  Click **Display**.

4.  Verify that the record count in SAP (minus the .Include and .Append
    records) equals the record count in the tt\*\_Fields\_Download
    table.

5.  Compare some of the fields in SAP and SQL and verify that the
    information is identical.

6.  Enter **SE16** in the **Command** field in SAP.

7.  Enter the QUERY\_TABLE name.  In the example, the user entered KNAI.

8.  Press **Enter**.

9.  Click **Number of Entries**.

10. Verify that the number of entries is equal to the record count in
    the tt\*\_Data\_Download table.

11. Compare some of the data in the tt\*\_Data\_Download-Data\_Wa field
    with the data in SAP and verify that the information is identical.
