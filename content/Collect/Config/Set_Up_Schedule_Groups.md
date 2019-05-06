# Set Up Schedule Groups

Tables that do not have a Schedule Group set up run multi-thread limited
to the number of jobs set in the general queue. The general queue is
used for non-DSP event processing.

Schedule Groups are used for scheduling a subset of tables and/or to
download tables in a single thread. Consider downloading using a single
thread when downloading very large tables. While downloading many small
tables all together using multi-thread may run efficiently, downloading
several large tables together can result in database contention on the
data file. In this case, it is more efficient to download the large
tables in a sequence using a single thread.

Downloading in a single thread downloads each table completely, in
sequence, which allows the user to run post-load rules.For example, the
user might download KNA1 followed by KNB1, and then all of the data
needed to run post-load update rules to the Customer App tables are
available.

Tables are often divided among business teams. Schedule Groups can also
be used for business needs to split tables into business teams. The user
can use schedule groups to specify the order in which to download
tables. This makes sense in a business team scenario where a team is
doing a customer load and must refresh the configuration and customer
tables, run the rules in Transform and then perform the post-validate
process. Because the team does not need to wait for the material tables
to download they can be scheduled to download after the configuration
and customer tables.

To create a Schedule Group in Collect:

1.  Select **Administrative \> Schedule Groups** in the
    *<span style="font-size: 11.0pt;">Navigation</span>* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Schedule Groups
    page](../Page_Desc/Schedule_Groups.htm)

3.  Enter a unique name in the **SCHEDULE GROUP** field.
    
    **NOTE:** If building a group with a DBMoto®package, the following
    applies:   
    If Schedule Group is set to NO GROUP, both Download and Mirror
    package will be built as an individual replication in DBMoto®.   
    If Schedule Group is set to AUTO and if it is a Download package,
    the replication will be part of a group named
    \<GroupPrefix\_Downloads. Otherwise, if it is a Mirror package, the
    replication will be part of a group called    
    If Schedule Group is set to "existing group name" with no
    restriction to the \<Group\_Size parameter the replication is built
    into that group. 
    
    **NOTE:** The Replication Mode must be consistent with the
    Replication Group Mode (e.g a download package cannot be grouped
    with a mirror package).  

4.  Enter a brief group description of the schedule group in the
    **DESCRIPTION** field.

5.  Click **Save**.

Once this is completed, continue with Assign Schedule Group to a Table.

<span id="Assign_Schedule_Group_to_a_Table."></span>

## Assign Schedule Group to a Table.

Schedule Groups are used for scheduling a subset of tables and/or to
download tables in single thread. Schedule Groups can also be used for
business needs to split tables into business teams.

Once the schedule group has been defined, assign the group to a table.

To assign a schedule group to a table:

1.  Click **Tables** in *Navigation* pane.

2.  Click **Vertical View** for Table.

3.  Click **Advanced Settings** tab.

4.  Click **Edit**.
    
    [View the field descriptions for the Tables page's Vertical
    View](../Page_Desc/Tables_H.htm)

5.  Select a group from **Schedule Group** list box.

6.  Click **Save**.
