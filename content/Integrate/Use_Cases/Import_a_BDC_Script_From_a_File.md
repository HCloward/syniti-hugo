# Import a BDC Script From a File

<span id="Post Data using a BDC Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

A BDC script can be uploaded (if the script has been created in SAP
using the SHDB transaction). It is preferable to upload a script when:

A script was already recorded in SAP using the SHDB transaction (as
there is no need to re-record it).

A browser other than Internet Explorer is used.

The client security policy restricts recording.

Outside of Integrate, the user can navigate to the SHDB transaction in
SAP and perform the BDC recording directly in SAP, save the recording as
a flat file, and then upload and import it into the template.

**NOTE**: A user can also record a script using Integrate. Refer to
[*<span style="color: #0000ff;">Record a BDC
Script</span>*](Record_a_BDC_Script.htm) for more information.

**NOTE**: Begin template creation on the *Template* page in *Horizontal*
View. Refer to [Create a Basic Template](Create_a_Basic_Template.htm)
for more information.

To upload and import a BDC script from a file on the *Vertical* View of
the *Template* page:

1.  Enter the SAP transaction code in **Transaction Code** field.

2.  Click **Save**;

3.  Click **File Import** to expand the section.

4.  Click **Upload** next to File Name.

5.  Browse to the file.

6.  Click **Open**.

7.  Click **Import**; a confirmation message displays.

8.  Click **Yes**.
    
    **NOTE**: The BDC screen and field data is created based on the file
    and the metadata for the script gathered from SAP.

9.  Click **Configuration** tab.

10. Click the **Enable Loop** check box to enable looping, if
    applicable.
    
    **NOTE**: Once this check box is enabled, BDC Screens can be put
    into and taken out of loops. Looping is a posting mechanism that
    processes multiple child keys for one parent key. It allows for
    multiple headers with infinite details to be posted. Looping can be
    enabled during template creation or after recording. Refer to
    [Configure Template Loops for a BDC Script
    Template](Configure_Template_LoopsBDC.htm) for detailed
    information. 

11. Click **BDC Screen** to view all screens captured in the recording.

For each of the BDC Screens, add, edit or delete the conditionals and
subsequent actions by selecting *Vertical* View for a record, then
clicking the **Conditionals** button. Refer to
[*<span style="color: #0000ff;font-style: normal;">Configure a
Conditional for a BDC Screen</span>*](ConfigureConditionalBDCScrn.htm)
for more information. 

**NOTE:** The default records created should suffice for most instances;
however, they can be modified or deleted as necessary. Refer to
[*<span style="color: #0000ff;font-style: normal;">Manage BDC Screens
and Fields</span>*](Manage_BDC_Screens_and_Fields.htm) for detailed
information.
