+++
title = 'Add DBMoto Functions'
solution = 'Platform'
+++

# Add DBMoto Functions

Use the *[DBMoto Function
Setup](../Page_Desc/DBMoto_Function_Setup.htm)* page to add a DBMoto
global script function. Users can also write their own function in the
replication script that the global script can call in. DBMoto supports
Visual Basic and C\#.

The following is an example of a global script function:

using System;

using System.Data;

using DBMotoPublic;

using DBMotoScript;

namespace DBRS

{

public class ReplicationScript : IReplicationScript

{

public override void Record\_onAfterMapping(DBMotoPublic.IRecord
recSource, DBMotoPublic.IRecord recTarget, ref bool AbortRecord)

{

GlobalScript.AddLog("The current record has been inserted", 0);

}

}

}

To add a DBMoto Function in Common:

1.  Navigate to **Configuration \> Modules \> DBMoto Function Setup** in
    the *Navigation* pane.
2.  Enter the name of the function in the **FUNCTION NAME** text box.
3.  Enter the global script function in the **FUNCTION SCRIPT** text
    area.
4.  Click **Save**.
