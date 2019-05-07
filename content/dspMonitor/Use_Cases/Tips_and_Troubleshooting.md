+++
title = 'Tips and Troubleshooting'
solution = 'Data Quality'
+++

# Tips and Troubleshooting

This section outlines common error messages that display in dspMonitor™
and a solution to work around the error.

It contains the following sections:

  - [Change Frequency of User
    Workflows](#Change_Frequency_of_User_Workflows)
  - [Enable Metric Data
Information](#Enable_Metric_Data_Information)

## <span id="Change_Frequency_of_User_Workflows"></span>Change Frequency of User Workflows

**Issue:** When the Group Schedule ID and Workflow Schedule ID for
Groups are set to run more frequently than the Workflow Schedule ID set
at the Report level, the following message displays:

*Workflow has been requested more frequent than when reports is process.
Workflow will only be sent when the report has been executed.*

**Solution:** Set the **Workflow Schedule ID** on the *Groups* page or
the **Workflow Schedule ID** on the *User (Reports)* page to **Send Upon
Completion**. Otherwise, the Workflow Schedule ID  fields must be set to
a lower
frequency.

## <span id="Enable_Metric_Data_Information"></span>Enable Metric Data Information

**Issue:** If the **Report Metric Data Build** check box is enabled on
the *Repository Reports* page and the **Report Columns** are not
configured, the following error message displays:

*Metric Data Options is turned on but no columns have been selected.*

**Solution:** Users have enabled the Metric Data feature, but have not
selected columns. There is no negative impact to dspMonitor™. Click
**Report Columns** to select columns. The **Report Metric Data Build**
setting is ignored until columns are selected.
