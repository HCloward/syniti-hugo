# Configure the Business Value Dashboard

For data to appear on the Business Value dashboard, the cost of the
failure must be set at the report level. Update the currency at the
WebApp level if the default of US dollars is not applicable.

Once configuration is complete, the cost per failure is calculated and
displays on dspMonitor™ pages in the Error Cost field.

To configure currency (if other than US dollars):

1.  Select **Configuration \> Parameters** in the *Navigation* pane.

2.  Click the **Metric Parameters** tab.

3.  Click **Edit**.
    
    [View the field descriptions for the Parameters
    page](../Page_Desc/Parameters.htm)

4.  Select the currency from the **Currency** list box.
    
    **NOTE:** If the currency is changed, the cost per failure is not
    calculated automatically. A user must manually update each report.

5.  Click **Save**.

To set the cost of failure:

1.  Select **Configuration \> Report Repositories** in the *Navigation*
    pane.

2.  Click the **Reports** icon.

3.  Click **Vertical View** for a report.

4.  Click **Edit**.
    
    [View the field descriptions for the Repository Reports
    page](../Page_Desc/Repository_Reports_H.htm)

5.  Enter the amount that an error on the report costs in the **Cost Per
    Failure** field.

6.  Click **Save**.
