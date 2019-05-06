# SQL View/Function/Procedure Design

Non-schema object design is the next most important thing above table
design when creating a WebApp. When lightweight and efficient, even
complex functions, views, and procedures can be implemented with little
overhead.

<span style="font-weight: bold;">NOTE</span>: Avoid Global Operators.
Any SQL procedures or functions that have to enumerate or parse full
sets of table data are dangerous due to their inability to scale
efficiently.

This section contains these topics:

  - [View and Stored Procedure Naming
    Conventions](View_and_Stored_Procedure_Naming_Conventions.htm)
  - [Partition Logic Semantically](Partition_Logic_Semantically.htm)
