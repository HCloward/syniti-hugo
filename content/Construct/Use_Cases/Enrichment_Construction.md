+++
title = 'Enrichment Construction'
solution = 'Migration'
+++

# Enrichment Construction

Use Enrichment Construction when a field or a few fields should be
constructed.

Enrichment Construction begins in Map, when a user maps a Target Source
field using a Construction action. When submitted, the following Objects
are created:

  - The Construct page with the Key fields, along with the field(s)
    mapped with an Action of Construct in Map.
    
    **NOTE:** Key fields are set as hard required on the
    *[Construct](../Page_Desc/Construct_Page)* page and required
    fields are set to soft required.

  - A CranPort package associated with the Collect Target Source table
    registration

  - The Collect Target registration (if it doesn’t already exist)

  - The Collect Source registration (if it doesn’t already exist)

  - The Collect Target Source table registration

The Source for Enrichment Construction is added as an Update Row Source,
and the relationship join to the Add Row Source is added automatically.
The joins can be viewed in Map on the *[Relationship
Joins](../../Map/Page_Desc/Relationship_Joins_H)* page. As with any
mapping, the Construction mapping must go through the Approvals process.
The developer assigned to the Target-Source reviews the Construct page
to approve or reject it. Refer to [Approve or Reject
Mappings](../../Map/Use_Cases/Approve_or_Reject_Mappings) for more
information.

Once approved, a construction page is created that contains only the
mapped field, not all active fields for the Target. This page has the
same number of records as in the Source.

<span style="font-weight: bold;">NOTE</span>: New custom pages and
existing custom pages created with Enrichment Construction can use
[Excel
Integration](../../../Platform/Excel_Int/Use_Excel_Integration) and
[Bulk Execution](../../../Platform/Bulk_Exec/Use_Bulk_Execution).
