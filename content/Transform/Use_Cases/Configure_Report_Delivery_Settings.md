# Configure Report Delivery Settings

In Console on the *[Parameters](../../Console/Page_Desc/Parameters.htm)*
page, review the **Report File Generation Mode ID**field on the
Transform tab and set it as needed for Report Delivery.

Options are:

  - **Automatic** — No reports are delivered through the Report Delivery
    pages.
  - **Custom** — At the Object or Target level, if the report is
    published, Transform uses the report-level Publish setting to
    determine whether or not to deliver a report through the Report
    Delivery pages. If the report is not published at the target or
    object level, no reports are delivered through the Report Delivery
    pages. If a report is processed directly (at the report level),
    Transform uses the Publish setting to determine whether or not to
    deliver the report through the Report Delivery pages.
  - **On Demand** — All reports for the object and target are published
    on Report Delivery pages, regardless of the publish setting at any
    level.

For Report Delivery to work, the Report Cache Data Source ID must be set
for each client on site, and determines where report data is cached.
Because reports could be in development at any time, Transform does not
display live data on reports, but stores a cached version of the last
run of the report to display on Report Delivery pages.

Define the data source in Console on the *Parameters* page on the
Transform tab for all objects, Define the data source for a specific
object on the [Process Area:
Object](../../Console/Page_Desc/Process_Area_ObjectH.htm) page.
