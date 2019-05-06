# Encrypt Columns

Before performing this task, [Register Tables to
Source](Register_Tables_to_Source.htm).

Encrypt source table columns to mask values when the table is
downloaded.

To encrypt columns in a source table:

1.  Create encryption key in **Common \> Configuration \> Modules \>
    Keys**. Refer to [Add Keys](../../Common/Use_Cases/Add_Keys.htm) for
    detailed information.

2.  Return to Collect.

3.  Click **Tables** in
    *<span style="font-size: 11.0pt;">Navigation</span>* pane.

4.  Click **Vertical View** for a table.

5.  Click **Advanced Settings** tab.

6.  Click **Encrypted Columns**; all columns for the table are listed.

7.  Click **Edit**.
    
    [View the field descriptions for the Target Source Table Column
    Encryption
    page](../Page_Desc/Target_Source_Table_Column_Encryption.htm)

8.  Select a key from **Encryption Key** list box to control the
    algorithm used to encrypt the column.

9.  Click **Save**.

10. Click **Action** tab.

11. Click **Build Package** icon so the columns marked for encryption
    are encrypted; a confirmation message displays.

12. Click **Ok**.

13. Verify new column(s) was added to the table.

To remove encryption from a column:

<span style="font-weight: bold;">NOTE</span>: If encryption is turned
off for a column, the package will need to be rebuilt for the table. The
package can be rebuilt with the Build Package Icon under the Action tab
in the vertical view of the table.

1.  Remove the encryption key for the column(s).
2.  Build the package so the columns where encryption has been removed
    are decrypted.

**NOTE:** Before building the package, verify **Delete Target Table On
Build** is enabled for the Source or manually delete the encrypted table
from the database. Build the package by clicking the Build Package on
the Vertical View on the *Tables* page. Refer to [Build Package for
Table](Build_Package_for_Table.htm) for more information.

**NOTE:** When encryption is removed from a table, the table structure
is reverted to the original structure.

Continue with [Configure RFC Options](Configure_RFC_Options.htm).
