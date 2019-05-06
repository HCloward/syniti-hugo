# Set Date, Time, and Decimal Formats

In Target Design, on the
<span style="font-style: italic;">[Targets](../Page_Desc/Targets_H_Design.htm)</span>
page’s <span style="font-style: italic;">Vertical</span> View, users
define formats for date, time, and decimal fields. This functionality
allows the Target Design fields to be set to a data type of NVARCHAR as
an open standard to allow all data to flow through the migration. The
validation rules written in Data Services check that the Target data is
in the correct format to load in to the Target system.

The Data Services AutoGen process uses the specifications defined in
Target Design on the <span style="font-style: italic;">Target</span>
page’s <span style="font-style: italic;">Vertical</span> View to define
the validation in Data Services if the field is identified as a field
requiring this format validation checking. The user can enter any ISO
standard Date or Time definition and specify whether the decimal
separator is a ‘.’ or ‘,’.

Refer to [Data Services
AutoGen](../../Data_Services_AutoGen/Data_Services_Automation.htm) for
more information.

Field formats are set at the Target level. There can be one date, time,
or decimal format per Target.

<span style="font-weight: bold;">NOTE</span>: These formats can be
updated from within Data Services AutoGen on the
<span style="font-style: italic;">[Target Data Services Rule Global
Variables](../../Transform/Page_Desc/Target_DS_Rule_Global_Variables.htm)</span>
page. Refer to [Configure Target Data Services Rule Global
Variables](../../Transform/Use_Cases/Configure_Target_DS_Rule_Global_Var.htm)
for more information.

There are two steps to applying a format to Target fields:

1.  Define the format on the
    <span style="font-style: italic;">Targets</span> page.
2.  Set the Field format for a field on the
    <span style="font-style: italic;">Target Fields</span> page.

To define the field format to be used in Data Services validation rules
in Target Design:

1.  Select <span style="font-weight: bold;">Design</span> in the Context
    bar.

2.  Click the <span style="font-weight: bold;">Targets</span>icon on the
    *[Design](../Page_Desc/Design.htm)* page.

3.  Click the <span style="font-weight: bold;"> Vertical View</span>
    icon for a Target.

4.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Targets page’s Vertical
    View](../Page_Desc/Targets_H_Design.htm#Targets_V)

5.  Enter the format for date fields in the
    <span style="font-weight: bold;">Date Format</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: Any ISO standard Date
    format is allowed.

6.  Enter the format for time fields in the
    <span style="font-weight: bold;">Time Format</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: Any ISO standard Time
    format is allowed.

7.  Specify the separator (either “.” or “,”) for decimal fields in the
    <span style="font-weight: bold;">Decimal Format</span> field.

8.  Click <span style="font-weight: bold;">Save</span>.

To set the field format for a field in Target Design:

1.  Select <span style="font-weight: bold;">Design</span> in the Context
    bar.

2.  Click the <span style="font-weight: bold;">Targets</span>icon on the
    *Design* page.

3.  Click the <span style="font-weight: bold;">Fields</span> icon for a
    Target.

4.  Click the <span style="font-weight: bold;">Vertical View</span> icon
    for a field.

5.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Target Fields page’s Vertical
    View](../Page_Desc/Target_Fields_H_Target_Design.htm#Target_Fields_V)

6.  Select the format (Date, Time, or Decimal) in the
    <span style="font-weight: bold;">Field Format</span> list box.

7.  Click <span style="font-weight: bold;">Save</span>.
