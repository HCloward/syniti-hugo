+++
title = 'Parameters – Profile'
solution = 'Platform'
+++

# Parameters – Profile

<div class="use">

Use this page to [Configure Profile
Parameters](../Use_Cases/Configure_Profile_Parameters.htm).

</div>

To access this page, click <span style="font-weight: bold;">Common \>
Configuration \> Modules \> Parameters – Profile</span> in the
*Navigation* pane.

Field

Description

Application Information

Version

Displays current release version of the component, Profile.

Date

Displays date when the component version was released.

Processing Settings

Profile Queue ID

Displays type of background queue to use as the default when profiling
objects. The recommended value is Background Event. Consult with the
on-site System Administrator for the best queue to be used on the
project. 

Blank Threshold

Displays the threshold to enable the Interesting setting. When the
percentage of blank field values is less than the Threshold, the
Interesting setting is enabled, marking the fields that still need to be
profiled.

Unique Cache Row Limit

Displays the number of unique values that are stored per column.

Big Table Settings

Big Table Split Size

Displays the number of rows in the table that will determine whether the
table runs in multi- or single-thread. Tables run in a single thread if
the Big Table Split Size is less than or equal to the number of rows in
the table.

Big Table Sub Query

Displays the number of records used to determine initial sampling size
of large tables.
