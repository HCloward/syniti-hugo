# Create Instructions

An *instruction* is a single unit of work to be performed by the engine.
Some examples of instructions are: create a table, add a column to a
table, update data and create a view. Common is delivered with a set of
instructions that may be used; additional instructions can be created to
fit the customer’s needs.

To create an instruction:

1.  Select **Automation Engine \> Automation Instructions** in
    *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Automation Instructions
    page](../Page_Desc/Automation_Instructions.htm)

3.  Enter the name of the instruction in **NAME** field.

4.  Enter a brief description of the instruction in **DESCRIPTION**
    field.

5.  Click **Save**.

6.  Click **SQL** for the instruction to add the SQL code.

7.  Click Edit.
    
    <span style="font-weight: bold;">NOTE:</span> If DSP SUPPLIED is
    enabled for the Automation Instructions, the instructions cannot be
    edited.
    
    [View the field descriptions for the Automation Instruction – SQL
    page](../Page_Desc/Automation_Instruction_SQL.htm)

8.  Enter SQL code used to determine if the SQL execution should precede
    in **Pre Check SQL** field if a pre check is needed.
    
    **NOTE:** The automation engine executes the **Pre Check SQL** and
    if one or more records are returned, the statement in the **SQL**
    field is not executed. This pre check allows a user to provide
    checks and control if SQL is run.

9.  Enter SQL code to perform the instruction in **SQL** field.

10. Click **Save**.
