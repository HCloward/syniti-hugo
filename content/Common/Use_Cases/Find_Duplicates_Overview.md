+++
title = 'Find Duplicates Overview'
solution = 'Platform'
+++

# Find Duplicates Overview

Common provides a quick and easy method to identify and resolve
duplicate data.

**NOTE:** There is a distinction between Duplicate Detection, configured
in System Administration, and Bulk Duplicate Detection performed in
Common. Bulk Duplicate Detection is an extension of the Duplicate
Detection capability. The Duplicate Detection validation rule runs as a
foreground event, triggered when:

  - A record is created or modified on a page where Duplicate Detection
    is enabled for a column(s)
  - A user manually triggers an event that contains the validation rule

Bulk Duplicate Detection is a background event that detects duplicates
for each record in a table. An Administrator or Designer runs the Bulk
Duplicate Detection process in Common.

This use case covers the following topics:

  - [Configure Duplicates
    Parameters](Configure_Duplicates_Parameters)
  - [Create Object Views](Create_Object_Views)
  - [Register Objects](Register_Objects)
  - [Configure Columns](Configure_Columns)
  - [Find Duplicates](Find_Duplicates)
  - [Run Post Duplicate Detection
    Process](Run_Post_Duplicate_Detection_Process)
  - [Resolve Duplicate Candidates](Resolve_Duplicate_Candidates)
  - [View
    Results](../../../Migration/Construct/Use_Cases/View_Results)
  - [Review Duplicate Records](Review_Duplicate_Records)
  - [Review Non Duplicate Records](Review_Non_Duplicate_Records)

 

**NOTE:** To allow business users to see the results of the Duplicate
Detection process:

1.  Add the business user to the Common WebApp, then add the user to the
    Analyze WebApp Group. Refer to [Assign Users to WebApp
    Groups](../../Sys_Admin/Use_Cases/Assign_Users_to_WebApp_Groups)
    in System Administration for more information.
2.  Assign a user-specific security definition to each business user.
    Add the Analyze data source(s) that are used in the Duplicate
    Detection process as a key to each user’s security definition. Refer
    to [Establish User-specific Security
    Definitions](../../Sys_Admin/Use_Cases/Establish_UserSpecific_Security_Definitions)
    in System Administration for more information.
