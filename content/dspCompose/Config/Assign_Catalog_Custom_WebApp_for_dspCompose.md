+++
title = 'Assign a Catalog to a Custom WebApp for Use with dspCompose™'
solution = 'Data Quality'
+++

# Assign a Catalog to a Custom WebApp for Use with dspCompose™

When dspCompose™ is installed, the WebApp dspCompose\_Data and its
database are also installed. dspCompose\_Data is the configured WebApp
and database where client customizations and data validations should be
created that will not be overwritten during an upgrade. In addition to
dspCompose\_Data, other custom WebApps and companion databases may be
created and used with dspCompose™.

**NOTE**: The number of custom WebApps that may be created is controlled
by client licensing.

When a custom WebApp is created, an Administrator must perform the
following tasks for the custom WebApp.

  - Create WebApp Groups
  - Define security
  - Define a WebApp catalog in order to perform translations

The catalog for the custom WebApp can be a new catalog added
specifically for the custom WebApp or the dspCompose\_Data catalog if no
specific catalog has been created and defined for the WebApp.

The dspCompose\_Data catalog may also be assigned to the WebApp even if
a specific catalog does exist for the custom WebApp. However, the
dspCompose\_Data catalog should be assigned to the WebApp with a higher
Priority number than the catalog specific to the custom WebApp.
