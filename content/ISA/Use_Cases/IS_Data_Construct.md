# Using IS Data Construct

ISA Construction provides the ability to rapidly create and maintain a
web-based user interface to manage cross reference table(s), and to
control parameters dynamically within the application rather than hard
code those values within the code of the SAP Information Steward Rule or
View. The IS Rule is built once. If the IS Rule requires updates (for
example, if parameters change or values need to be added) a business
user does not need a developer to change the underlying code of the IS
Rule. The business user can make changes directly in the web-based
application. These changes are fully auditable. To edit reports in ISA
Construction, users must be granted access to the application.

Often within a Passive data governance implementation, a
business-specific configuration is required that is not maintained
within the system of record. For example, a system may deliver over 150
valid units of measure, yet only 5 –10 of these values are business
allowable values for the Base Unit of Measure of a Material. The
remaining units of measure are used for Packaging, Weight, Volume,
Sales, or Purchasing; conversion factors; or other needs and therefore
should not be options for Base Unit of Measure.

ISA Construction allows the developer to create fully auditable web
pages for a business user to maintain this configuration through the
user interface of the DSP® so that the developer does not have to change
the underlying code of the IS Rule. This process not only enables saving
on IT costs, but also directly enables the business to make the
necessary changes as they are needed and identified by the business,
with no development involvement, estimates, budgets, or funding.

**NOTE**: Knowledge of Information Steward, such as how to add a view or
make a rule, is required to use IS Data Construct.

At a high level, the process for using IS Data Construct is:

1.  Combine a table in the IS Data Construct database with another table
    or view in IS.

2.  Make a rule using parameters to join the lookup or join to the
    table.
    
    **NOTE:** A view could also be created in SQL when looking for
    keywords or performing a regular expression check.

3.  Create a page in the DSP accessible in IS Data Construct to display
    data in the table or to allow users to input values for the rule’s
    parameters.

The following example illustrates how to use a rule to reference a
table. 

**NOTE**: This is a basic example of one rule and is not meant to be
comprehensive. A user can create any rule or view that works with the
table’s data.

The rule Material above Minimum Stock by Color of Interest validates
that the stock level of a material for a particular color is greater
than the minimum stock level. If the stock level is less than the
Minimum Stock, the validation fails. These failed records display on a
report that is sent to users through the ISA.

Using a page created in the platform and accessible in IS Data
Construct, users can add more parameters for the rule (i.e., additional
colors and minimum stock levels for that color).

To create the rule:

1.  Add an Information Steward Connection to the configuration database
    (i.e., dspMonitor\_Config) in the CMC.
    
    **NOTE:** The Connection’s Purpose should be set to For data
    profiling.

2.  Create a table in the configuration database using SQL.
    
    Here is the table definition for this
    rule.
    
    ![](../../../Resources/Images/IS%20Data%20Config%20Table%20Definition%20Example.png)

3.  Add the table to the project in IS where the rule will be created.

4.  Add a rule in the IS project with the following
    parameters.
    
    ![](../../../Resources/Images/IS%20Data%20Config%20rule%20parameters.png)

5.  Create the rule in IS that uses the proper look up for the table
    passing in the
    parameters.
    
    ![](../../../Resources/Images/IS%20Data%20Construct%20Rule%20Example%20close%20up.png)

6.  Create a page in the platform.

![](../../../Resources/Images/IS%20Data%20Config%20Example%20page.png)

Below is the horizontal view in SQL for the
page.

![](../../../Resources/Images/IS%20Data%20Construct%20Horizonal%20View%20Example.png)

Once the user saves a new record on the
<span style="font-style: italic;">Safety Stock by Color</span> page, the
rule must be run again in IS.

For the new rule to be visible in ISA the tables must be refreshed in
Collect to bring in the rule metadata.

**NOTE:** The Collect process does not need to be executed when a rule
is run as the failed data is directly accessible to the ISA.

Add the rule to a project distribution so that users can receive reports
based on the data that failed the rules (i.e., materials with a color
that has fallen below the count for minimum safety stock). Refer to [Add
Rules to a Project
Distribution](Add_Rules_to_a_Project_Distribution) for more
information.
