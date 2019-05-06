# Manage Target Sources

A Target Source is a record of the relationship between a source table
and a Target table. Rules and reports can be built against a Target
Source to process specific source tables for specific Target tables.
Multiple Sources can be registered to a single Target and processed
individually.

Transform contains the Target Sources assigned to Targets in Target
Design along with the source tables corresponding to these Target
Sources. Additional source tables can be assigned to a Target in
Transform.

Refer to [Assign Additional Target
Sources](Assign_Additional_Target_Sources.htm) for more information.

To manage Target Sources, use Transform to:

  - [Add Target Source Rules](Add_Target_Source_Rules.htm)
  - [Add Source Audit Rules](Add_Source_Audit_Rules.htm)
  - [Add Target Source Reports](Add_Target_Source_Reports.htm)

On the *[Target Sources](../Page_Desc/Target_Sources_H.htm)* page, a
user can also:

  - View all data for the source by clicking the
    <span style="font-weight: bold;">View Source</span>icon

  - Monitor any background processes running in the queue for the
    selected Target Source by clicking the
    <span style="font-weight: bold;">Queue</span> icon

  - Process the selected Target Source by clicking the
    <span style="font-weight: bold;">Process</span> icon in the Page
    toolbar to run the entire Target Source in the background by
    importing all data from all Sources and running all source rules and
    source reports
    
    <span style="font-weight: bold;">NOTE:</span> If the selected source
    is inactive, the Process icon is disabled.
    
    **NOTE:** Access the Process Information tab on the *Target Sources*
    page’s *Vertical* View to only process Sources, rules, and reports
    for the Target Source.

  - Reset the processing status if any processing failed for Target
    Sources, Target Source reports or Target Source rules by clicking
    <span style="font-weight: bold;">Reset</span>
