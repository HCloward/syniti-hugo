+++
title = 'Target Report Segments'
solution = 'Migration'
+++

# Target Report Segments

An Administrator can identify a field on the report to use for creating
report segments. For each unique value in that field, Transform creates
a subdirectory and a report in the File Location indicated on the
*Vertical* View of the [Target
Reports](../Page_Desc/Target_Reports_H.htm), [Target Source
Reports](../Page_Desc/Target_Source_Reports_H.htm) and [Target Data
Services Reports](../Page_Desc/Target_Data_Services_Reports_H.htm)
pages.

Business users must be assigned to a segment to view the segment
reports.

This topic contains the following sections:

  - [Create Target Report Segments](#Create_Target_Report_Segments)
  - [Assign a User to a Target Report
    Segment](#Assign_a_User_to_a_Target_Report_Segment)

## <span id="Create_Target_Report_Segments"></span>Create Target Report Segments

To create target report segments for Target, Target Source and Target
Data Services reports in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.
2.  Click the **Reports** icon for a target.

OR

1.  Click the**Targets** icon on the *Process Area Launch* page.
2.  Click the **Sources** icon for a target.
3.  Click the **Reports** icon for a source.

OR

1.  Click the **Targets** icon on the *Process Area Launch* page.
2.  Click the **Data Services Reports** icon for a target.

After accessing the report:

1.  Click **Vertical View** for the report on the [Target
    Reports](../Page_Desc/Target_Reports_H.htm), [Target Source
    Reports](../Page_Desc/Target_Source_Reports_H.htm) and [Target Data
    Services Reports](../Page_Desc/Target_Data_Services_Reports_H.htm)
    pages.

2.  Click **Edit**.

3.  Select an option from the **Segment by Field** list box.

4.  Click **Save**.
    
    **NOTE:** If the field has values that have returned records, the
    number of segments for the selected report displays on the Segments
    icon.

5.  Click the **Segments** icon to view the
segments.

## <span id="Assign_a_User_to_a_Target_Report_Segment"></span>Assign a User to a Target Report Segment

Business users must be assigned to a segment to view the segment
reports.

To assign a user to a report segment in Transform:

1.  Click **Vertical View** for a report on the [Target
    Reports](../Page_Desc/Target_Reports_H.htm), [Target Source
    Reports](../Page_Desc/Target_Source_Reports_H.htm) or[Target Data
    Services Reports](../Page_Desc/Target_Data_Services_Reports_H.htm)
    pages.
    
    **NOTE:** In order to assign a user to a Target report segment,
    **Segment By Field** must be populated. If it is not populated,
    refer to [Create Target Report
    Segments](#Create_Target_Report_Segments) for more information.

2.  Click the **Business User Settings** tab.

3.  Click the **Business User Segment Assignment** icon.

4.  Select a segment from the *[Target Report
    Segments](../Page_Desc/Target_Reports_Segments.htm)* page.

5.  Select the user(s) to assign to the segment.

6.  Click the **Add User**icon.
    
    **NOTE:** A check mark displays under the IS MEMBER column for each
    user name selected.
    
    **NOTE:** A user can be assigned to a report segment but not have
    access to the report. In this case, no segments are displayed.
