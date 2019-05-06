# Add the Request Details Data Visualization Page to the Content WebApp

The Request Details Data Visualization Page provides a visual
representation of an active request’s process through the workflow,
including which roles have been completed for the request. A Designer
can add this page in the Content WebApp for users to access.

The diagram displays the:

  - Request status for the request selected on the
    *[Request](../Page_Desc/Request.htm)* page
  - Scenario to which the request belongs
  - Roles in the scenario
  - Status of each role (i.e., Finished or Not finished)
  - Tasks assigned to each role and if those task were rejected

Information about creating a WebApp, registering stored procedures to
events, and building pages in the platform is included in the *DSP®
Application Development Guide*. 

**NOTE**: The user who adds this page must have permission to create and
copy files on the web server where the DSP® is installed.

To add the page:

1.  Add
    the./B9FF453E-D5BB-4A58-8CFF-E9620CEE0E1C/English/DGERequestDetails.aspx
    file as the static source for a new ‘Request Details’ static page to
    the Content WebApp.

2.  Add 'Boa.Dsp.DGE.RequestDetailsPlugin' as an external page business
    rule to the OnLoad event for the static page created in step 1.

3.  Add an Image or Button Column on the Content WebApp's Request page
    that includes the static page created in step 1 as the 'Link to
    Page' value (Admin \> WebApps \> Pages for the Content WebApp \>
    Column Properties  \> Vertical View). It is recommended to use
    Cransoft.Control.Image.
    
    **NOTE:** A user clicks this image to open the
    <span style="font-style: italic;">Request Details Data
    Visualization</span> page.

<!-- end list -->

1.  Enter either RequestId or RequestID (whichever column name is used
    in the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Request</span>
    page's *Horizontal* and *Vertical* View) to the Shared Field Names
    field on the *Page Column Links Vertical* View (Admin \> WebApps \>
    Pages for the Content WebApp \> Column Properties \> List Source
    link).
