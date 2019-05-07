+++
title = 'Configure Business Value Parameters'
solution = 'Master Data Management'
+++

# Configure Business Value Parameters

A Designer can set the values that are used to calculate the information
displayed on the business value dashboard charts. Refer to [View
Business Value Dashboard](View_Business_Value_Dashboard.htm) for more
information about the dashboard.

Before performing this task, the Designer must set the currency symbol
that represents the currency being used by the organization if the
currency symbol is other than the default. The designer must also select
the calendar to be used for the working hours calculations if the
calendar is other than the default dspConduct calendar. Refer to [Set
Currency Display Label](../Config/Set_Currency_Display_Label.htm) and
[Set Calendar Used For Business Value
Calculations](../Config/Set_Calendar_Used_For_Business_Value_Calculations.htm)
for more information.

To track business value the Designer enters a baseline of the number of
working hours that it took to complete a business process manually
<span style="color: #ff0000; font-weight: bold;">before the process was
automated</span> using dspConduct. In addition, the Designer enters a
baseline cost value for the average per hour of all costs associated
with completing the business process, including fixed costs **before the
process was automated**, using dspConduct. These values are used to
calculate business value as follows:

  - **Hours Saved** = Baseline Hours - Actual Hours for a Request
    
    **NOTE:** Actual Hours are calculated as the number of hours between
    the time the first request role began and the time the last request
    role was finished based on the calendar (that is set on the
    *_[Parameters](../Page_Desc/Parameters_dspConduct.htm)_* page).

  - **Total Hours Saved** = Sum of Previous Request Total Hours Saved +
    Current Request Hours Saved

  - **Cost Saved** = Average Cost Per Hour \* Hours Saved for a Request

  - **Total Cost Saved** = Sum of Previous Requests Total Dollars Saved
    + Current Request Dollars Saved.

To configure business value parameters:

1.  Select **dspConduct \> Design** in the *Navigation* pane.

2.  Click the **Business Processes** icon for the category on the
    *Category* page.

3.  Click the **Vertical View** icon for the business process.

4.  Click **Edit**.
    
    [*View the field descriptions for the Business Process page’s
    Vertical
    View*](../Page_Desc/Business_Process_H.htm#Business_Process_V)

5.  Enter the baseline hours in the **Baseline Hours** field.
    
    **NOTE:** Enter working hours in whole units. Partial hours
    (decimals) are not allowed.

6.  Enter the average cost per hour in the **Average Cost Per Hour**
    field.
    
    **NOTE:** Enter the average cost per hour based on the **Current
    Application Currency** field. The application currency is set on the
    *[Parameters](../Page_Desc/Parameters_dspConduct.htm)* page. Refer
    to [Set Currency Display
    Label](../Config/Set_Currency_Display_Label.htm) for more
    information.

7.  Click **Save**.

Continue with [Add a Scenario to a Business
Process](Add_a_Scenario_to_a_Business_Process.htm).
