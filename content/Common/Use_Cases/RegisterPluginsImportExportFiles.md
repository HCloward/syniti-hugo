# Register Plugins to Import and Export Files

In order to use the Excel import/export adaptors, the following plugins
must be registered as business or validation rules on the page using the
Excel adaptor:

  - Import: RAD.Excel: ExcelImportAdapter

  - Export: RAD.Excel: ExcelExportAdapter

These shared plugins are registered to the Common WebApp and can be used
across other WebApps.
