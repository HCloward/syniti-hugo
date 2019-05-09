+++
title = 'Register Reports to a Report Repository'
solution = 'Data Quality'
+++

# Register Reports to a Report Repository

Reports are registered to a report repository and then to a group for
individual users (group members) to view.

To register a report:

1.  Select **dspMonitor \> Configuration \> Report Repositories** in
    *Navigation* pane.

2.  Click **Reports** for Repository.

3.  Click **Add**.
    
    [View the field descriptions for the Repository Reports page's
    Vertical View](../Page_Desc/Repository_Reports_H)

4.  Select a report from **Report** list box.

5.  Select an opportunity view from the **Opportunity View** list box.
    
    **NOTE:** An opportunity view is only applicable to Error reports.

6.  Select a type from **Report Type** list box.
    
    A Report Type helps users organize output reports. There are three
    options:
    
      - **Error –** Indicates an error in the report must be fixed.
      - **Info –** Indicates the report contains general,
        information-only data.
      - **Metrics** – Includes metric data to measure business or
        dspMonitor™ reporting.

7.  Enter text in **Implication** field.
    
    **NOTE:** The Implication field describes the consequence of the
    error, as in, what the report means to the business.

8.  Enter a report description in **Comment** field.

9.  Enter a user-friendly report name in **Title** field.

10. Select a categorization from **Quality Dimension** list box.
    DSP-supplied values are:
    
      - **Accuracy** – The degree to which data correctly describes the
        "real world" object or event being described.
    
      - **Completeness –** The proportion of stored data against the
        potential of 100% complete.
    
      - **Consistency –** The absence of difference, when comparing two
        or more representations of a thing against a definition.
    
      - **Validity –** Data is valid if it conforms to the syntax
        (format, type, range) of its definition.
    
      - **Timeliness –** The degree to which data represent reality from
        the required point in time.
    
      - **Uniqueness –** No thing is recorded more than once based upon
        how that thing is identified.
    
    **NOTE:** Additional Quality Dimensions can be added. Refer to
    [Register Quality
    Dimensions](Populate_Configuration_Tables#Register_Quality_Dimensions)
    for more information.

11. Update **Status** field if default value is not applicable. Values
    are:
    
      - **Approved** – Report has been approved by the business user.
      - **Not Approved** – Report has not been approved by the business
        user.
    
    **NOTE:** Only reports with a status of Approved are available to
    group members and are processed based on the configured schedule.

12. Verify **Allow Manual Run** check box is enabled to permit the
    report to be manually run.
    
    **NOTE:** Disable this feature if the report can only be run on a
    schedule.

13. Update **Output File Type** list box if default value is not
    applicable.
    
    **NOTE:** There are two Output File Type options: File Excel and
    File Delimited. File Excel refers to Excel 2003 (xls files). To use
    Excel 2007 (xlsx files), enable the **Build Xlsx Reports** check box
    under Configuration \> Parameters.  Use File Delimited to generate a
    text file, which is much smaller than an Excel file.

14. Update **Output File Delimiter** list box if default value is not
    applicable.
    
    **NOTE:** The Output File Delimiter determines how the columns in
    the report are separated.

15. Enter a sort order in **Report Order By** field. Do not include
    “ORDER BY” in the sort order.
    
    **NOTE:** The Output File Delimiter determines how the columns in
    the report are separated. The Report Order By field is used to build
    the final report file. dspMonitor dynamically rebuilds the SQL code
    to support User Filters and then applies this parameter to sort the
    data in the final output.

16. Select data quality scoring thresholds from the **Threshold ID**
    list box. (optional)
    
    **NOTE:** If no threshold is selected the threshold ID set on the
    *[Parameters](../Page_Desc/Parameters)* page is used in the data
    quality score status calculation. Refer to [Register Data Quality
    Score
    Thresholds](Populate_Configuration_Tables#Register_Data_Quality_Score_Thresholds)
    for more information.

17. Click **Metric Data Information** tab.

18. Click **Report Metric Data Build** check box to track and maintain
    metric data.
    
    **NOTE:** Metric data can be tracked in order to determine how long
    an error exists in a report. Refer to [Track Error Records on
    Reports](Track_Error_Records_on_Reports) for detailed
    information.

19. Click **Save**.
