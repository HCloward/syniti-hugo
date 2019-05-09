+++
title = 'Full Construction and Enrichment Construction'
solution = 'Migration'
+++

# Full Construction and Enrichment Construction

Construct allows users to efficiently construct missing data and
provides a location to rapidly develop web pages for gathering
information.

Users enter data in construct pages that is not available in source
(legacy) systems. Such missing values could be:

  - A field or two from a particular Object, such as Material UOM or
    Vendors Fax Number, that are required by the Target system, but do
    not exist in the legacy system (and the values in these fields
    cannot be inferred).
  - Entire Objects in the Target system that have no legacy data and the
    data is required for a business process to run within that Target
    system. For example, a legacy system may not support required data
    such as BOMs or Routings.

Web pages can be automatically generated for use with either Full
Construction or Enrichment Construction.

When a Construct Source is generated using either Full Construction or
Enrichment Construction, the tables in Construct (stored in the Default
Data Source that is applied at the Wave Process Area level in Console)
are the tables used for the data collection process (for example, the
data entered in to the Construct page). Once the construction is
complete (as in, the number of completed records for the Target is equal
to the estimated records), these tables become the Source to one or more
Targets to be mapped, automatically generated, used for rules and
reports, and exported to be loaded to a Target system.

By default, Construct tables are stored in the Construct WebApp where
code is auto-generated, and where the pages, the views that underlie the
pages, and table schemas are stored. The default Source data source,
sdbDSPConstruct, is a database delivered with the installation that is
used to contain a snap shot of the Source system for the first Wave. As
a best practice, create a new sdbDSPConstruct\* for each Wave so that
the snapshot can occur independently from timelines of different Waves.

The Construct WebApp and Source data source can be changed in Console
for custom WebApps. For example, a client may require that
data-sensitive content be added to a WebApp called ConstructHR. This
data will not be tracked for construction completion status. Refer to
[Update the WebApp and Source Data Source for
Construct](../../Console/Use_Cases/Update_Construct_WebApp_and_Data_Source)
for more information.

**NOTE**: Construct pages can also be created manually without using
auto-generation. However, metrics are not tracked for manually added
pages. Refer to [Build a Construction Page
Manually](../../../Platform/Common/Use_Cases/Build_a_Construction_Page_Manually)
for more information.  

<span style="font-weight: bold;">NOTE</span>: New custom pages and
existing custom pages created with Full Construction and Enrichment
Construction can use [Excel
Integration](../../../Platform/Excel_Int/Use_Excel_Integration) and
[Bulk
Execution](../../../Platform/Sys_Admin/Use_Cases/Configure_Bulk_Execution_Overview).

Refer to [Enrichment Construction](Enrichment_Construction) and
[Full Construction](Full_Construction) for more information.
