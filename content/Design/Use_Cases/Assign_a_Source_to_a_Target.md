+++
title = 'Assign a Source to a Target'
solution = 'Migration'
+++

# Assign a Source to a Target

In Target Design, a Migration Developer can add a Source with a Source
type of:  

  - <span style="font-weight: bold;">Add Row -</span> A Source database
    that contains the data from the Source system to be moved to the
    Target. A Source database name begins with "sdb." A Source’s System
    Type determines the database schema, or table definitions, for the
    Source.
  - <span style="font-weight: bold;">{Full Construction} -</span> A
    Source that is manually created using Construct. This option is set
    by default when a user selects {Full Construction} from the SOURCE
    DATA SOURCE list box. This option is not available for any other
    Source data sources.
  - <span style="font-weight: bold;">External Source -</span> An Update
    Row Source that is external to the  system used in the Add Row
    Source when establishing a relationship.

When a Source is added to a Target and the Source data source is {Full
Construction}, the zSource of FullConstruct is automatically added to
the
<span style="font-style: italic;">[zSource](../../Construct/Page_Desc/Z_Source.htm)</span>
page in Construct, and the user does not need to manually enter the
zSource. Refer to [Set Up
zSource](../../Construct/Config/Set_up_ZSources.htm) and [Full
Construction](../../Construct/Use_Cases/Full_Construction.htm) for more
information.

**NOTE**: A Source can be added to a Target only if the Target is in a
Design Status of In Design.

<span style="font-weight: bold;">NOTE</span>: A Utility Target cannot
use {Full Construction} as a Source data source.

When a field mapping’s action is set to ManualConstruction, the Source
associated with the field is automatically added to the
<span style="font-style: italic;">zSource</span> page in Construct, and
the user does not need to manually enter the zSource. Refer to [Set up
 zSources](../../Construct/Config/Set_up_ZSources.htm) and [Enrichment
Construction](../../Construct/Use_Cases/Enrichment_Construction.htm) for
more information.

When a Source is added to a Target, the Source’s columns are loaded into
the Target Source schema for the Source table. A field in the schema may
then be locked, preventing it from being reset if a Target Source is
reset. If the Source is updated to a new Source for the Target (for
example from MARA to MARC), columns from the incorrect Source table (in
this case MARA) are removed from the Target Source schema and columns
from the correct table (MARC) are loaded. In this case, locked fields in
MARA are not removed from the Target Source schema.

Sources with other Source types can be added in Map. Refer to [Work with
Sources](../../Map/Use_Cases/Work_with_Sources.htm) for more
information.

To assign a Source to a Target in Target Design:

1.  Select **Design** in the *Navigation* pane.

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Design](../Page_Desc/Design.htm)* page.

3.  Click the **Sources** icon for a Target.

4.  Click **Add**.
    
    *[View the field descriptions for the Target Sources
    page](../Page_Desc/Target_Sources_H_Design.htm)*

5.  Select a Source from the **SOURCE DATA SOURCE** list box.
    
    **NOTE:** These data sources have been registered in Common. Refer
    to [Register a Data Source in
    Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.

6.  Click the **+** icon in this field to open the *[Data Source
    Registry](../../../Platform/Common/Page_Desc/Data_Source_Registry_H.htm)*
    page to add a data source if necessary.

7.  Select an option in the **SOURCE TYPE** list box.
    
    **NOTE**:Values are:
    
      - <span style="font-weight: bold;">Add Row</span> – The Add Row,
        or primary, Source for the Target.
      - <span style="font-weight: bold;">Full Construction</span> – A
        Source to be built manually in Construct and that only displays
        when the Full Construction Source data source is selected.
      - <span style="font-weight: bold;">External Source</span> – An
        Update Row Source that can be in a relationship with an Add Row
        Source, but uses a different Source system than the Add Row
        Source.
    
    **NOTE:** The options available in this list box depend on the
    Source data source selected.

8.  Click <span style="font-weight: bold;">Save</span>.

**NOTE:** A Source uses a System Type to store table, column, look-up
table and mapping information about the Source that is used throughout
the data migration. System Types can be loaded from databases created
from a Collect Target download or manually created. Refer to [System
Types](../../../Platform/Common/Use_Cases/System_Types_Overview.htm) for
more information.

**NOTE:** A Source’s System Type is assigned when the data source is
registered in Common. Refer
to<span style="font-size: 11.0pt;color: #0000ff;">[Register a Data
Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)</span>for
more information.

**NOTE:** A Source data source can be assigned to only one System Type
across all Targets. For example, the Source data source of sdbSAP has
been assigned to the System Type SAPLEGACY for the Target ttMARA. If the
Target ttMAKT also uses the data source of sdbSAP, it could not use a
different System Type such as SAP. The data source sdbSAP must use the
System Type SAPLEGACY. Refer to [Sync Source Data Source-System Types
Across all Targets](Sync_Data_Source_System_Types_Across_Targets.htm)
for more information.

**NOTE:** Once the Design Status is set to Design Finished or Complete,
this source is loaded into Map as Source fields that can be mapped on
the *Field Mappings* page. The Source is also loaded into Transform to
be used for rules and reports.

**NOTE:** Sources can have Developers and Business Contacts assigned.
Refer to [Add Developers and Business Contacts to a Target or
Source](Add_Developers_and%20Business%20Contacts.htm) for more
information.
