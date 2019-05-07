+++
title = 'CTS Notes Specific to dspCompose™'
solution = 'Data Quality'
+++

# CTS Notes Specific to dspCompose™

When creating CTS archives to support dspCompose™ objects, if any
objects included in any Packing List reside in a data source/database
that does not exist on the target system, manually create that database
in the target system before the archive can be successfully imported
into the target. The WebApp for the objects should also already exist on
the target system.

**NOTE**: Prior to running the CTS process for dspCompose™ objects, a
separate CTS process must be run. This process must establish the data
source and WebApp ID in the target instance for the database that stores
dspCompose™ data and customizations (by default, dspCompose\_Data). The
data source and WebApp ID must be identical in the target and source
environments. Setting these values must be performed via CTS and not
performed manually.

This use case includes the following topics:

  - [Shippable Items in Detail](Shippable_Items_in_Detail.htm)

  - [Supporting Objects for
    Templates](Supporting_Objects_for_Templates.htm)

  - [Include DSP® Pages Listed on Template (Objects)
    Page](Include_DSP_Pages_Listed_on_Template_Objects_Page.htm)
