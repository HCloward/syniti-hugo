+++
title = 'Create System Type Groups from the Fetch Process'
solution = 'Platform'
+++

# Create System Type Groups from the Fetch Process

System Type groups are logical groupings of tables, such as Customer or
Vendor. Use System Type groups for source database systems where a large
number of tables must be created and downloaded.

Create these groups using one of these methods:

  - Create System Type groups from the Fetch process.
  - [Create System Type groups from source
    tables.](Create_a_System_Type_Group_from_Source_Tables)
  - [Create System Type groups manually in
    Common.](../../Common/Use_Cases/Add_System_Types_Groups)

To create groups from the fetch process:

1.  Select **Collect \>Targets** in the *Navigation* pane; the *Targets*
    and *Target Sources* pages display

2.  Click the **Sources** icon for a target.

3.  Click **Add** to add a source to the target.
    
    **NOTE:** Refer to [Register Sources to
    Target](Register_and_Use_Sources#Register_Sources_to_Target) for
    detailed information.

4.  Click <span style="font-weight: bold;">Save</span>.

5.  Test the connection by selecting the
    <span style="font-weight: bold;">Test Connection</span> icon in the
    <span style="font-style: italic;">Target Sources</span> toolbar.

6.  Click **Vertical View** icon for the SOURCE

7.  Select the <span style="font-weight: bold;">Action</span> tab.

8.  Click the <span style="font-weight: bold;">Fetch Tables</span> icon.

9.  Click <span style="font-weight: bold;">OK</span>.

A new System Type group is created automatically during the fetch
process for each schema owner with the naming convention of
\<source\>\_\<schemaowner\>.
