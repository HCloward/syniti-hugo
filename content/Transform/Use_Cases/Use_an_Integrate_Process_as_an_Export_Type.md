# Use an Integrate Process as an Export Type

This task is performed by a Migration Developer, or any user who has
access to the Wave and Process Area.

Before registering a Target export with an Export Type of Integrate, the
Target export view must be manually created in SQL server along with the
Target export tables. The view must be named using the naming convention
set in Common on the *[Parameters –
Integrate](../../../Platform/Common/Page_Desc/Parameters_Integrate.htm)*
page. The default naming convention is tx\*int.

In Integrate, the process must use this target export view stored in the
\*.dsw database.

Transform does not load data into an ERP system; it stages data for
export. Target exports are the last sets of rules to move the Target
data to a location so that it can be staged for an ERP system using a
loading tool such as Integrate.

An Integrate process, or a series of posting steps:

  - Defines how Integrate takes data from the platform and transfers it
    to SAP
  - Serves to link the data in a column in a view with a field on a
    template assigned to the process

Refer to [Manage
Processes](../../../Platform/Integrate/Use_Cases/Manage_Processes.htm)
for more information.

To use an Integrate process as an Export Type in Transform:

1.  [Access Transform](../Config/Access_Transform.htm).

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the <span style="font-style: italic;">[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)</span> page.

3.  Click the <span style="font-weight: bold;">Exports</span> icon for a
    Target.

4.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Target Exports
    page.](../Page_Desc/Target_Exports_H.htm)

5.  Enter a sort value in the
    <span style="font-weight: bold;">PRIORITY</span> field.
    
    **NOTE:** If multiple exports exist for the Target, the Priority
    determines the order the export is processed.

6.  Select a value from the
    <span id="Status" class="popUpLink">STATUS</span> list box.

7.  Select a Target from the <span style="font-weight: bold;">TARGET
    EXPORT</span> list box.
    
    **NOTE:** This is the manually created view in SQL server.

8.  Select <span style="font-weight: bold;">Integrate</span> from the
    **EXPORT TYPE** list box.

9.  Select **Integrate** from the <span style="font-weight: bold;">LOAD
    TYPE</span> list box, if applicable.
    
    **NOTE:** This field is for documentation purposes only.

10. Click <span style="font-weight: bold;">Save</span>; the
    <span style="font-style: italic;">Vertical</span> View displays.

11. Select an Integrate process from the
    <span style="font-weight: bold;">Export Name</span> list box.
    
    **NOTE**: For Integrate processes to display in this list box, they
    must be named using the naming convention set in Common on the
    *Parameters – Integrate* page. The default naming convention
    tx\*int.

12. Click <span style="font-weight: bold;">Save</span>.

13. Close the <span style="font-style: italic;">Vertical</span> View.

14. Click <span style="font-weight: bold;">OK</span>.
    
    **NOTE:** If a process takes less than 0.5 seconds to run, the
    duration in the DURATION field is 0.

15. Click <span style="font-weight: bold;">Integrate</span> in the
    Context bar.

16. Click the <span style="font-weight: bold;">Processes</span> icon for
    a category to access the process used to load data.
