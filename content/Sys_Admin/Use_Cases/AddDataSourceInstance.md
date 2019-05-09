+++
title = 'Add a Data Source Instance'
solution = 'Platform'
+++

# Add a Data Source Instance

The data source instance is the logical platform "instance" (for
example, Dev, QA, or Production) that this physical instance of the DSP
represents. Before moving items between instances via the CTS process,
the source and target instances must be indicated in the DSP. The DSP is
delivered with DEV, PROD and QA instances set up. Refer to [Set Up
Instances](Set_up_Instances) for more information.

In Multi-Instancing (multiple application servers), code is not promoted
between DSP environments; multiple DSP instances manage “different”
parts of the migration, quality or governance processes.

Use multiple instances to address performance issues (for example heavy
data construction usage), volume issues or to separate waves to make
managing them easier.

When determining whether to use multiple instances in a migration
scenario, consider the number of concurrent waves, the number of users
and WebApps, data volumes and testing cycles.

HCM and HR data almost always requires an additional DSP instance. It is
a best practice to isolate HR data to its own server set.

To add a data source instance in System Administration:

1.  Click **Data Sources** in the *Navigation* pane.

2.  Click the **Instances** icon.

3.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    *[View the field description for the Data Source Instances
    page](../Page_Desc/DataSourceInstancesH)*

4.  Select an instance from the **INSTANCE** list box. The options are
    DEV, PROD and QA.

5.  Click **Save**; the *Vertical* View displays.

6.  If needed, enter a path for the data source instance in the **Path**
    text box.

7.  Click the **Advanced Properties** tab.

8.  Click the **Protected** check box if you want the data source to be
    read only.
    
    **NOTE:** If checked, data source features that make changes to the
    data source are hidden/disabled (for example, Recompile Objects,
    Append System Columns, building System Views, indexing, auditing,
    encryption, and building WebApps).

9.  Click **Save**.
