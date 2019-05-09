+++
title = 'Use a Custom WebApp with dspCompose™'
solution = 'Data Quality'
+++

# Use a Custom WebApp with dspCompose™

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

To use the custom WebApp:

1.  [Create all tt Tables and Views to Support the Pages in the Custom
    WebApp](Create_all_tt_Tables_and_Views_to_Support_the_Pages_in_the_Custom_WebApp)
2.  [Create rt Tables From the tt Tables and Create Views for the Custom
    WebApp](Create_rt_Tables_From_the_tt_Tables_and_Create_Views_for_the_Custom_WebApp)
3.  [Create Pages and Views in Custom
    WebApp](Create_Pages_and_Views_in_Custom_WebApp)
4.  [Create a Custom Template for use with the Custom
    WebApp.](Create_a_Custom_Template_for_Use_with_the_Custom_WebApp)
