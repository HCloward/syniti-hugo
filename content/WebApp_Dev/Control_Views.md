+++
title = 'Control Views'
solution = 'Platform'
+++

# Control Views

Run Time Control Views (RTCV) provide a way to define column control at
run time based on the data. This view type defines standard DSP® control
statuses for columns on a page. These columns are based on data rather
than a column property.

Control statuses are:

  - **0** – Disabled
  - **1** – Enabled
  - **2** – Hidden

In addition, select BOA™ Reserved Columns can be defined in a RTCV, for
example, boaAdd, boaEdit and boaDelete.

Types of RTCVs are:

  - [Data Control View (DCV)](Data_Control_Views) – Defines control
    based on what is known about the data on the page.
  - [Page Control View (PCV)](Page_Control_View) – Defines control
    based on what is known about the page as a whole, including the
    parent page.
  - [User Control View (UCV)](User_Control_Views) – Defines control
    based on what is known about the user.

When designing the control view hierarchy for a page, design the views
in a way to minimize duplicating logic in multiple views.

Also, put control views at the appropriate level (e.g., a Data Control
View conforms to the BOA reserved word functionality thereby allowing a
boaUserID column to be added to the view). Using the boaUserID filter in
a DCV, it could emulate the same functionality as a UCV. This strategy
should not be implemented; rather, put user-centric logic in the UCV and
control logic based on data in the DCV.

When a page loads, DSP® uses the following approach to determine page
and column control:

  - WebApp Security Group
  - Page Properties
  - Page Column Properties
  - UCV
  - PCV
  - DCV

In this hierarchy, the most restrictive prevails. Once the control
status of a column has been limited, it cannot be made less strict. For
example, if one of the controls on a page sets a column to hidden (2),
the column is hidden even if another RTCV or property sets the column to
enabled (1).

In terms of DSP®:

  - Hidden always wins
  - Disabled beats enabled
  - If nothing hides or disables the column, the column is enabled.
