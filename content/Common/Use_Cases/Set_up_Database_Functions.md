+++
title = 'Set up Database Functions'
solution = 'Platform'
+++

# Set up Database Functions

Generic database functions can be used by the Post Action Rule Table
feature, i.e., run after a table is downloaded. Common is delivered with
a set of database functions; additional functions can be added if
needed.

To register database functions:

1.  Select **Configuration \> Modules \> Database Function Setup** in
    *Navigation* pane.

2.  Click **Add.**
    
    [View the field descriptions for the Database Function Setup
    page.](../Page_Desc/Database_Function_Setup)

3.  Enter a database function name in **DATA BASE NAME** field.

4.  Enter a SQL script in **DATA BASE RULE** field.  To include the name
    of the current column in the rule, use **\#boaColumn\#** dynamic
    replacement placeholders in the rule.

5.  Click **Save**; the function is now available to be registered to a
    Post Action Rule Table record.
