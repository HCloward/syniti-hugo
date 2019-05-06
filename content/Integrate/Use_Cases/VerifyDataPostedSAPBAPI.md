# Verify the Data was Posted in SAP for the BAPI

<span id="Post Data using a BAPI Steps" class="popUpLink">\>Review the
steps in the process. </span>

**NOTE:** This use case provides an example of posting using the
BAPI\_MATERIAL\_SAVE DATA, but does not supply comprehensive
instructions to suit all BAPIs.

To verify that records were posted:

1.  Log in to the SAP instance where the data was posted.

2.  Enter <span style="font-weight: bold;">SE16</span> in the
    <span style="font-weight: bold;">Command</span> field and press
    <span style="font-weight: bold;">Enter</span>.

3.  Enter a table name and press
    <span style="font-weight: bold;">Enter</span>. In the example, MARA
    was used.
    
    ![Description:
    databrowserinitialscreen](../../../Resources/Images/image001.png)

4.  Enter the data noted on the *Messages* page. In the example, enter
    the **Material Number From** and **Material Number To**.
    
    ![Description: databrowser](../../../Resources/Images/image002.png)

5.  Click **Execute**.
    
    The posted records that displayed on the *Message* page in Integrate
    display on the *Data Browser: Table \[table name\] Select Entries*
    screen in SAP.

6.  Navigate back to the <span style="font-style: italic;">Data Browser:
    Initial Screen</span>.

7.  Enter other table names, and follow the steps above to verify that
    the posted records display correctly for these tables as well. In
    the example, the user also verifies tables such as MARC, MVKE, and
    MBEW.

To verify the data posted in the records:

1.  Enter **MM03** in the **Command** field and press
    <span style="font-weight: bold;">Enter</span>.

2.  Enter a value that was created during the post process and displayed
    on the *Messages* page and press
    <span style="font-weight: bold;">Enter</span>. In the example, the
    user entered a Material Number.
    
    ![Description:
    DisplayMaterial](../../../Resources/Images/image004.png)

3.  Select all views.
    
    ![Description: SelectViews](../../../Resources/Images/image005.png)

4.  Press <span style="font-weight: bold;">Enter</span>.

5.  Populate **Organizational Levels** and press
    <span style="font-weight: bold;">Enter</span>.
    
    ![Description: orglevels](../../../Resources/Images/image006.png)

6.  Navigate to <span style="font-weight: bold;">Additional Data</span>.

7.  Confirm the posting data displays. In the example, **Description**
    and **Units of Measure** were verified.
    
    ![Description: Descriptions](../../../Resources/Images/image007.png)

8.  Navigate through each view and verify the data.

To verify the data downloaded from SAP:

1.  Log in to SQL Management Studio.
2.  Access the database.
3.  Open a download table that corresponds to an Upload table that was
    populated.
4.  Verify the download table was updated with the data returned from
    SAP.
