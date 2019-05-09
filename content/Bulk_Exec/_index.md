+++
title = "Bulk Execution Overview"
weight = 3
layout = "single"
tips = "bulk"
+++

# Use Bulk Execution

Bulk Execution is the ability to run an OnValidate event in the
foreground on a DSP® page for all records or a subset of those records
via a simple, guided user experience.

A Page Designer must enable Bulk Execution on a Construct page or a page
in a custom WebApp. Refer to [Enable Bulk Execution for a
Page](../Sys_Admin/Use_Cases/Enable_Bulk_Execution_for_a_Page) for
more information. These pages, deployed at customer sites by technical
power users, are used by business users, SMEs, and other data
contributors. Sometimes, data contributors need to validate all records
or a subset of records on a page. After Bulk Execution completes, the
results allow users to direct their efforts to those records that failed
the validations.

Certain DSP pages are [delivered with Bulk Execution
enabled](../Sys_Admin/Use_Cases/DSP_Pages_Delivered_with_Bulk_Execution_Enabled).

Without Bulk Execution, the user would need to click each record
individually to validate it. Typically, a construction page or custom
application page has hundreds or thousands of records. Given the record
volumes, the ability to validate all records is required to facilitate a
viable user experience.

Once Bulk Execution is started, the process runs in the background and
the panel remains visible. The user can navigate away and work on other
pages while Bulk Execution is running. To use the Bulk Execution panel
again after navigating to another page, click the **Return to Page**
icon on the Control Panel tab. The page where Bulk Execution is being
performed displays, and the panel displays with the settings and filters
applied.

If the user refreshes the browser or the session times out while Bulk
Execution is running, the panel restores with the tab that was active,
and with the options that were selected. If the user refreshes the
browser or the session times out after Bulk Execution has completed, the
Results tab displays.

Results are stored in the database for 6 hours after completion of the
Bulk Execution process.

If the user closes the browser or the panel after Bulk Execution
completes, the results no longer display. The process must be run again.

This section includes the following topics:

  - [Filter the Record Set Before Performing Bulk
    Execution](Filter_the_Record_Set)
  - [Perform Bulk Execution](Perform_Bulk_Execution)
  - [View Bulk Execution Results](View_Bulk_Execution_Results)
