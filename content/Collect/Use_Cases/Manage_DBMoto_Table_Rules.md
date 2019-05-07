+++
title = 'Manage DBMoto® Table Rules'
solution = 'Platform'
+++

# Manage DBMoto® Table Rules

DBMoto® rules remove the leading zeros using a script built into Collect
package build process. These entries can be made active or inactive.
Entries can be added for custom SAP tables or tables not in the DSP®
supplied list (Administrative \> DBMoto Table Rules where DSP Supplied
is enabled).

To run DBMoto® Table Rules:

1.  Select **Administrative \> DBMoto Table Rules** in *Navigation*
    pane.

2.  Click **Add**.
    
    [View the field descriptions for the DBMoto Table Rules
    page](../Page_Desc/DBMoto_Table_Rules.htm)

3.  Enter source table in **TABLE** field.

4.  Enter column name to include in rule in **COLUMN** field.

5.  Enter function to apply to rule in **DB MOTO FUNCTION** field.

6.  Verify **ACTIVE** check box is enabled, allowing Collect to include
    the field in the build package process.

7.  Click **Save**.
