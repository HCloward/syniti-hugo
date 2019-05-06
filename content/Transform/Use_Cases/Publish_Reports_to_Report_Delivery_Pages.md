# Publish Reports to Report Delivery Pages

When a report is published it is visible on the Business user’s Report
Delivery pages (accessed from **My Reports** in the *Navigation* pane).

Actionable reports are error reports with a non-zero record count.
<span id="Report Type" class="popUpLink">Report types</span> for error
reports are Error, Target Readiness and Business Readiness.

By default, reports are not published.

A user can publish all reports in an object, target, or target source,
by checking the **PUBLISH** check box on the
*[Objects](../Page_Desc/Objects_HTransform.htm)*,
*[Targets](../Page_Desc/Targets_H.htm)*, *[*Target
Sources*](../Page_Desc/Target_Sources_H.htm)* pages.

A user can also publish an individual report.

**NOTE:** If the PUBLISH check box is enabled at the parent level on the
*Targets*, *Objects*, and *Target Sources* pages, DSP® evaluates the
publish setting for each report for the object, target and source to
determine if the report will be published. If the PUBLISH check box is
not enabled at the parent level, then the publish setting for each
report is ignored and none of the reports beneath the parent level are
published. When processing a report directly, Transform uses the
report-level publish setting to determine whether to publish a report to
the Report Delivery pages.

**NOTE:** To avoid publishing an invalid report while that report is
under development, turn off publishing for the object on the *Objects*
page.
