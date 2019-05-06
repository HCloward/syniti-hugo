# Configure Target Data Services Rule Global Variables

For each of the Data Services Jobs, the global variables needed to pass
parameters into Data Services are automatically populated. The global
variables are passed to the Data Services Job at runtime and the Job is
executed based on parameters specified in the global variables.

The global variables (date formats, time formats, etc.) are populated
from the object level Target where they were specified. The global
variables can be updated on the *[Target Data Services
Rules](../Page_Desc/Target_Data_Services_Rules_H.htm)* page’s *Vertical*
View, if needed. Do not change the Wave, Process Area, object or Target
global variables because they are hardcoded values that tie specifically
to the GUIDs of those elements.

**NOTE:** Do not edit the values for the Wave, Process Area, Object or
Target variables.

To configure Target Data Services rule global variables in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the **Data Services Rules** icon; the *Target Data Services
    Rules* page displays.

3.  Click the **Vertical View** icon for the Data Services rule; the
    <span style="font-style: italic;">Target Data Services Rules</span>
    page's <span style="font-style: italic;">Vertical</span> View
    displays.

4.  Click the **Global Variables** icon; the *[Target Data Services Rule
    Global Variables](../Page_Desc/Target_DS_Rule_Global_Variables.htm)*
    page displays.

5.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the Target Data Services Rule Global Variables
    page.](../Page_Desc/Target_DS_Rule_Global_Variables.htm)

6.  Enter a name for the variable in the
    <span style="font-weight: bold;">Name</span> field.

7.  Enter the constant value for the variable in the
    <span style="font-weight: bold;">Constant</span> Field.

8.  Click **Save**.
