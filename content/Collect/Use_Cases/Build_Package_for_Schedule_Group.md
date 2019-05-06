# Build Package for Schedule Group

To build a package for a schedule group:

1.  Click **Targets** in
    *<span style="font-size: 11.0pt;">Navigation</span>* pane.

2.  Click **Sources** for Target.

3.  Click **Schedule Groups** for Source. 

4.  Select the Schedule Group.
    
    **NOTE:** If building a group with a DBMoto® package the following
    applies:   
    if Schedule Group is set to NO GROUP, both Download and Mirror
    package will be built as an individual replication in DBMoto®.   
    If Schedule Group is set to AUTO and if it is a Download package,
    the replication will be part of a group named
    \<GroupPrefix\>\_Downloads. Otherwise, if it is a Mirror package the
    replication will be part of a group called
    \<GroupPrefix\>\_\<number\> where number is an incremental value to
    count the number of groups. Groups cannot contain more than
    \<Group\_Size\> replications.   
    If Schedule Group is set to "existing group name" with no
    restriction to the \<Group\_Size\> parameter the replication is
    built into that group. 
    
    **NOTE:** The Replication Mode must be consistent with the
    Replication Group Mode (e.g a download package cannot be grouped
    with a mirror package).

<!-- end list -->

1.  Click **Build Package** on Page toolbar; a confirmation message
    displays.

2.  Click **Ok**.
    
    **NOTE:** If no package exists, a package is immediately scheduled
    to be built and the table is refreshed. If a package exists, the
    table is refreshed.
